---
title: Exchange EWS を使用して別のユーザーのフォルダーのアクセス許可を設定します。
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7eb81676-a780-4c56-b4f2-c4ed2697107d
description: Exchange で EWS マネージ API または EWS を使用して、フォルダーのアクセス許可レベルを設定する方法について説明します。
ms.openlocfilehash: 5bf570612d6349628e7f3abf858daa33daa13745
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759062"
---
# <a name="set-folder-permissions-for-another-user-by-using-ews-in-exchange"></a>Exchange EWS を使用して別のユーザーのフォルダーのアクセス許可を設定します。

Exchange で EWS マネージ API または EWS を使用して、フォルダーのアクセス許可レベルを設定する方法について説明します。
  
フォルダー レベルのアクセス許可によって、ユーザーは、他のユーザーのメールボックスの 1 つ以上のフォルダーにアクセス可能になります。フォルダーのアクセス許可は代理人アクセスに似ていますが、次のような相違点があります。  
  
- フォルダーのアクセス許可は、ユーザーに「代理送信」または「送信者」別のユーザーを有効にできません。 これらには、フォルダーへのアクセスのみ有効にします。 ユーザーはこれらのフォルダーにアイテムを作成することができますが、それらを送信することはできません。
    
- メールボックスの任意のフォルダーで、フォルダーのアクセス許可を設定できますが、代理人を追加できるのは、予定表、連絡先、受信トレイ、履歴、メモ、タスクのフォルダーのみです。
    
- いくつかの[特定のフォルダーに対するアクセス許可](#bk_folderperms)を設定することができます。 代理人を追加するときは、 [5 つのアクセス許可レベル](delegate-access-and-ews-in-exchange.md#bk_delegateperms)のみのいずれかを割り当てることができます。
    
- 匿名ユーザーと既定のユーザーに対して、フォルダーのアクセス許可を設定できます。メールが有効なアカウントだけに代理人アクセスを許可できます。
    
アクセス制御エントリ (ACE) と随意アクセス制御リスト (DACL) に精通していれば、ユーザーが各フォルダーのアクセス許可のセットを 1 つだけ持てることをご存じでしょう。ユーザーにアクセス許可のセットを追加しようとすると、そのユーザーがアクセス許可のセットを既に持っている場合、エラーが返されます。フォルダーのアクセス許可を追加、削除、更新する場合、現在の DACL を取得し、任意の ACE を追加するか削除し、更新した DACL を送信します。同じユーザーに対して複数の ACE を追加することはできません。EWS マネージ API を使用してアクセス許可を更新する場合、ユーザーの現在の ACE を削除し、新しい ACE をコレクションに追加する必要があります。EWS を使用している場合は、以前の ACE のセットを新しいセットに置き換えるだけです。
  
1 つのフォルダーで複数のアクセス許可を変更する場合は、追加、削除、更新をバッチ処理することができます。複数のフォルダーでユーザーの更新をするときには、バッチ処理はできないことに注意してください。1 つのフォルダーのアクセス許可を取得するために、1 回の呼び出しが必要です。そのフォルダーに対するアクセス許可を更新するには、2 番目の呼び出しが必要です。ユーザーのアクセス許可を追加、削除、更新する場合、各タスクで、同じ 2 つのメソッド呼び出しまたは操作を使用します。
  
**表 1 です。EWS のマネージ API のメソッドおよびフォルダーのアクセス許可を設定するための EWS の操作**

|目的…|使用する EWS マネージ API メソッド|使用する EWS 操作…|
|:-----|:-----|:-----|
|フォルダーのアクセス許可の有効化、削除、更新  <br/> |[Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx)の後に <br/> |[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)の後に <br/> |
|フォルダーの作成、フォルダーのアクセス許可の定義  <br/> |[Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
   
## <a name="folder-permissions"></a>フォルダーのアクセス許可
<a name="bk_folderperms"> </a>

特定のフォルダーにフォルダーのアクセス許可を設定する場合、多くのオプションがあります。ユーザーごとにフォルダーのアクセス許可レベルを設定できます。そのレベルで DACL に対する事前定義された個別のアクセス許可のセットを追加するか、フォルダーの個別アクセス許可を設定できます。しかし、それらを混在させたり、合わせたりすることはできません。
  
次の個別アクセス許可を使用できます。
  
- 作成可能
- サブフォルダー作成可能    
- フォルダーの所有者になる    
- フォルダーを表示可能    
- 連絡先フォルダーにする    
- アイテムの編集    
- アイテムの削除    
- アイテムの参照
    
さらに、次のアクセス許可レベルは、個々 のアクセス許可と、値のサブセットを定義する表 2 に示すように。
  
- なし    
- Owner (所有者)    
- PublishingEditor (出版編集者)    
- Editor (編集者)    
- PublishingAuthor (出版著者)    
- Author (著者)    
- NoneditingAuthor (非編集著者)    
- Reviewer (校閲者)    
- Contributor (投稿者)   
- カスタム ・ アプリケーションでは、この値を設定することはできません。 サーバーは、アプリケーションには、個々 のアクセス許可のユーザー設定のコレクションが含まれている場合にこの値を設定します。    
- FreeBusyTimeOnly - これのみ設定できます予定表フォルダーにします。   
- FreeBusyTimeAndSubjectAndLocation - これのみ設定できます予定表フォルダーにします。
    
次の表は、アクセス許可レベルに基づき、既定で適用される個別アクセス許可を示しています。
  
**表 2 になります。アクセス許可レベルでの個々 のアクセス許可**

|アクセス許可レベル|アイテム作成可能|サブ フォルダー作成可能|フォルダーの所有者になる|フォルダーを表示可能|連絡先フォルダーにする|アイテムの編集|アイテムの削除|アイテムの参照可能|
|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|:-----|
|None (なし)  <br/> |False  <br/> |False  <br/> |False  <br/> |False  <br/> |False  <br/> |なし  <br/> |なし  <br/> |なし  <br/> |
|Owner  <br/> |True  <br/> |True  <br/> |True  <br/> |True  <br/> |True  <br/> |すべて  <br/> |すべて  <br/> |FullDetails  <br/> |
|PublishingEditor (出版編集者)  <br/> |True  <br/> |True  <br/> |False  <br/> |True  <br/> |False  <br/> |すべて  <br/> |すべて  <br/> |FullDetails  <br/> |
|Editor (編集者)  <br/> |True  <br/> |False  <br/> |False  <br/> |True  <br/> |False  <br/> |すべて  <br/> |すべて  <br/> |FullDetails  <br/> |
|PublishingAuthor (出版著者)  <br/> |True  <br/> |True  <br/> |False  <br/> |True  <br/> |False  <br/> |Owned (所有)  <br/> |Owned (所有)  <br/> |FullDetails  <br/> |
|Author (著者)  <br/> |True  <br/> |False  <br/> |False  <br/> |True  <br/> |False  <br/> |Owned (所有)  <br/> |Owned (所有)  <br/> |FullDetails  <br/> |
|NoneditingAuthor (非編集著者)  <br/> |True  <br/> |False  <br/> |False  <br/> |True  <br/> |False  <br/> |None (なし)  <br/> |Owned (所有)  <br/> |FullDetails  <br/> |
|Reviewer (校閲者)  <br/> |False  <br/> |False  <br/> |False  <br/> |True  <br/> |False  <br/> |なし  <br/> |None (なし)  <br/> |FullDetails  <br/> |
|Contributor (投稿者)  <br/> |True  <br/> |False  <br/> |False  <br/> |True  <br/> |False  <br/> |なし  <br/> |なし  <br/> |なし  <br/> |
   
フォルダー レベルのアクセス許可の要求で非カスタムのアクセス許可レベルを指定する場合は個別のアクセス許可の設定を指定する必要はありません。 アクセス許可レベルを設定するときは、個別のアクセス許可を指定して場合、 **ErrorInvalidPermissionSettings**エラーに表示されます、応答します。 
  
## <a name="adding-folder-permissions-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してフォルダーのアクセス許可を追加する
<a name="bk_enableewsma"> </a>

次のコード例は、以下の目的で EWS マネージ API を使用する方法を示しています。  
  
- 新しいユーザー用の新しい[FolderPermission](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx)オブジェクトを作成します。 
    
- [Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx)メソッドを使用してフォルダーの現在のアクセス許可を取得します。 
    
- [Folder.Permissions](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx)プロパティには、新しい**FolderPermissions**を追加します。 
    
- 新しいアクセス許可をサーバーに保存するのには[Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx)メソッドを呼び出します。 
    
この例では**サービス**をそのメールボックス所有者の有効な[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトは、ユーザーが Exchange サーバーに認証されているとします。 
  
```cs
static void EnableFolderPermissions(ExchangeService service)
{
    // Create a property set to use for folder binding.
    PropertySet propSet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.Permissions);
    // Specify the SMTP address of the new user and the folder permissions level.
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
    
    // Bind to the folder and get the current permissions. 
    // This call results in a GetFolder call to EWS.
    Folder sentItemsFolder = Folder.Bind(service, WellKnownFolderName.SentItems, propSet);
 
    // Add the permissions for the new user to the Sent Items DACL.
    sentItemsFolder.Permissions.Add(fldperm);
    // This call results in a UpdateFolder call to EWS.
    sentItemsFolder.Update();
}
```

次のコードの行は、アクセス許可レベルを指定します。
  
```cs
    FolderPermission fldperm = new FolderPermission("sadie@contoso.com", FolderPermissionLevel.Editor);
```

カスタム アクセス許可レベルを使用する場合は、代わりに次のコードを使用します。
  
```cs
FolderPermission fldperm = new FolderPermission();
fldperm.UserId = "sadie@Contoso1000.onmicrosoft.com";
fldperm.CanCreateItems = true;
fldperm.CanCreateSubFolders = true;
…
```

カスタム アクセス許可レベルを持つ**FolderPermission**オブジェクトを作成するときは、書き込み可能な[FolderPermission のプロパティ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx)の一部またはすべてを設定できます。 ただし、 [FolderPermissionLevel](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx)が明示的に設定される**カスタム**アプリケーションでします。 **FolderPermissionLevel**は、 **FolderPermission**オブジェクトを作成し、個々 のアクセス許可を設定する場合にのみカスタムに設定されています。 
  
## <a name="adding-folder-permissions-by-using-ews"></a>EWS を使用してフォルダーのアクセス許可を追加する
<a name="bk_enableews"> </a>

次の EWS のコード例では、現在のアクセス許可を取得し、新しいアクセス許可の一覧を送信することによって、特定のフォルダーにアクセス許可を追加する方法を示しています。
  
最初のステップでは、 [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx)の値 (この例では [送信済みアイテム フォルダー) のアクセス許可を追加するフォルダーを指定して、 [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx)値には、フォルダー: PermissionSet が含まれています、 [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)要求を送信します。 この要求は、指定したフォルダーのアクセス許可の設定を取得します。 
  
EWS のマネージ API が[フォルダーのアクセス許可を追加](#bk_enableewsma)するのには**Bind**メソッドを呼び出すときに送信する XML 要求にもです。
  
```XML
  <?xml version="1.0" encoding="utf-8"?>
  <soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                 xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                 xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                 xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2007_SP1" />
    </soap:Header>
    <soap:Body>
      <m:GetFolder>
        <m:FolderShape>
          <t:BaseShape>IdOnly</t:BaseShape>
          <t:AdditionalProperties>
            <t:FieldURI FieldURI="folder:PermissionSet" />
          </t:AdditionalProperties>
        </m:FolderShape>
        <m:FolderIds>
          <t:DistinguishedFolderId Id="sentitems" />
        </m:FolderIds>
      </m:GetFolder>
    </soap:Body>
  </soap:Envelope>
```

**NoError**フォルダーが正常に取得されたことを示すは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値を含む[GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx)メッセージで**GetFolder**要求にサーバーが応答します。 [フォルダー Id](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx)と[ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx)の値は、読みやすくするために短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="CgAAAA=="
                          ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd1" />
              <t:PermissionSet>
                <t:Permissions>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Default</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                </t:Permissions>
              </t:PermissionSet>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

**UpdateFolder**操作を使用して、送信、更新された[PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx)、新しいユーザーの[アクセス許可](http://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx)を含む。 [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)操作にそれぞれのフォルダーの[SetFolderField](http://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx)要素を含めると、フォルダーに対するすべてのアクセス許可の設定が上書きされることに注意してください。 同様に、 **UpdateFolder**操作の[DeleteFolderField](http://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx)オプションも削除されます、フォルダーに対するすべてのアクセス許可の設定。 
  
EWS のマネージ API が[フォルダーのアクセス許可を追加](#bk_enableewsma)するのには**Update**メソッドを呼び出すときに送信する XML 要求にもです。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="CgAAAA=="
                      ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd1" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:PermissionSet" />
              <t:Folder>
                <t:PermissionSet>
                  <t:Permissions>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Default</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
                      </t:UserId>
                      <t:PermissionLevel>Editor</t:PermissionLevel>
                    </t:Permission>
                  </t:Permissions>
                </t:PermissionSet>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

次のコードの行は、アクセス許可レベルを指定します。
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress>sadie@contoso.com</t:PrimarySmtpAddress>
    </t:UserId>
    <t:PermissionLevel>Editor</t:PermissionLevel>
</t:Permission>
```

カスタム アクセス許可レベルを使用する場合は、代わりに次のコードを使用します。
  
```xml
<t:Permission>
    <t:UserId>
        <t:PrimarySmtpAddress> sadie@contoso.com </t:PrimarySmtpAddress>
    </t:UserId>
    <t:CanCreateItems>true</t:CanCreateItems>
    <t:CanCreateSubFolders>true</t:CanCreateSubFolders>
    <t:IsFolderOwner>false</t:IsFolderOwner>
    <t:IsFolderVisible>false</t:IsFolderVisible>
    <t:IsFolderContact>false</t:IsFolderContact>
    <t:EditItems>None</t:EditItems>
    <t:DeleteItems>None</t:DeleteItems>
    <t:ReadItems>None</t:ReadItems>
    <t:PermissionLevel>Custom</t:PermissionLevel>
</t:Permission>
```

**NoError**フォルダーが正常に更新されたことを示すは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値が含まれています[UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx)メッセージから**UpdateFolder**要求にサーバーが応答します。
  
## <a name="removing-folder-permissions-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してフォルダーのアクセス許可を削除する
<a name="bk_removeewsma"> </a>

次のコード例は、既定および匿名のアクセス許可を除く、特定のフォルダーのすべてのユーザーのアクセス許可を削除するために、EWS マネージ API を使用する方法を示しています。
  
1. **Bind**メソッドを使用してフォルダーの現在のアクセス許可を取得しています。 
    
2. **アクセス許可**のコレクションを反復処理して、個々 のユーザーに対してアクセス許可を削除します。 
    
3. 変更を保存するのには**Update**メソッドを呼び出しています。 
    
この例では、フォルダーのすべてのユーザー アクセス許可を削除します。特定のユーザーのアクセス許可のみを削除するようこの例を変更する場合、次のコードの行を変更して、ユーザーの表示名、または SMTP アドレスのいずれかを識別できるようにします。
  
```cs
if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
```

この例では**サービス**をそのメールボックス所有者の有効な[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトは、ユーザーが Exchange サーバーに認証されているとします。 
  
```cs
static void RemoveFolderPermissions(ExchangeService service)
{
    // Create a property set to use for folder binding.
    PropertySet propSet = new PropertySet(BasePropertySet.FirstClassProperties, FolderSchema.Permissions);
    // Bind to the folder and get the current permissions. 
    // This call results in a GetFolder call to EWS.
    Folder sentItemsFolder = Folder.Bind(service, new FolderId(WellKnownFolderName.SentItems, "primary@contoso.com"), propSet);
    // Iterate through the collection of permissions and remove permissions for any 
    // user with a display name or SMTP address. This leaves the anonymous and 
    // default user permissions unchanged. 
    if (sentItemsFolder.Permissions.Count != 0)
    {
        for (int t = 0; t < sentItemsFolder.Permissions.Count; t++)
        {
            // Find any permissions associated with the specified user and remove them from the DACL
            if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
            {
                sentItemsFolder.Permissions.Remove(sentItemsFolder.Permissions[t]);
            }
        }
    }
    // This call results in an UpdateFolder call to EWS.
    sentItemsFolder.Update();
}
```

## <a name="removing-folder-permissions-by-using-ews"></a>EWS を使用してフォルダーのアクセス許可を削除する
<a name="bk_removeews"> </a>

EWS の次のコード例は、既定および匿名のアクセス許可を除く、特定のフォルダーのすべてのユーザーのアクセス許可を削除する方法を示します。
  
最初に、 [DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx)の値は、アクセス許可 (この例では [送信済みアイテム フォルダー) を削除するフォルダーを指定し、 [FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx)れますフォルダー: PermissionSet [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)要求を送信します。 この要求は、指定したフォルダーの[PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx)を取得します。 
  
EWS のマネージ API が[フォルダーのアクセス許可を削除](#bk_removeewsma)するのには**Bind**メソッドを呼び出すときに送信する XML 要求にもです。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:PermissionSet" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="drafts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

**NoError**フォルダーが正常に取得されたことを示すは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値を含む[GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx)メッセージで**GetFolder**要求にサーバーが応答します。 **フォルダー Id**と**ParentFolderId**の要素の値は、読みやすくするために短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="EAAAAA=="
                          ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd5" />
              <t:ParentFolderId Id="CQAAAA=="
                                ChangeKey="AQAAAA==" />
              <t:FolderClass>IPF.Note</t:FolderClass>
              <t:DisplayName>Drafts</t:DisplayName>
              <t:TotalCount>0</t:TotalCount>
              <t:ChildFolderCount>0</t:ChildFolderCount>
              <t:EffectiveRights>
                <t:CreateAssociated>true</t:CreateAssociated>
                <t:CreateContents>true</t:CreateContents>
                <t:CreateHierarchy>true</t:CreateHierarchy>
                <t:Delete>true</t:Delete>
                <t:Modify>true</t:Modify>
                <t:Read>true</t:Read>
                <t:ViewPrivateItems>true</t:ViewPrivateItems>
              </t:EffectiveRights>
              <t:PermissionSet>
                <t:Permissions>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Default</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                    </t:UserId>
                    <t:CanCreateItems>false</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>false</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>None</t:EditItems>
                    <t:DeleteItems>None</t:DeleteItems>
                    <t:ReadItems>None</t:ReadItems>
                    <t:PermissionLevel>None</t:PermissionLevel>
                  </t:Permission>
                  <t:Permission>
                    <t:UserId>
                      <t:SID>S-1-5-21-1337771579-694202782-848329751-1535223</t:SID>
                      <t:PrimarySmtpAddress>sadie@Contoso.com</t:PrimarySmtpAddress>
                      <t:DisplayName>Sadie Daniels</t:DisplayName>
                    </t:UserId>
                    <t:CanCreateItems>true</t:CanCreateItems>
                    <t:CanCreateSubFolders>false</t:CanCreateSubFolders>
                    <t:IsFolderOwner>false</t:IsFolderOwner>
                    <t:IsFolderVisible>true</t:IsFolderVisible>
                    <t:IsFolderContact>false</t:IsFolderContact>
                    <t:EditItems>All</t:EditItems>
                    <t:DeleteItems>All</t:DeleteItems>
                    <t:ReadItems>FullDetails</t:ReadItems>
                    <t:PermissionLevel>Editor</t:PermissionLevel>
                  </t:Permission>
                </t:Permissions>
              </t:PermissionSet>
              <t:UnreadCount>0</t:UnreadCount>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

**UpdateFolder**操作を使用して送信する、更新された**PermissionSet**、削除されたユーザーの**アクセス許可**が含まれていません。 
  
EWS のマネージ API が[フォルダーのアクセス許可を削除](#bk_removeewsma)するのには**Update**メソッドを呼び出すときに送信する XML 要求にもです。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="EAAAAA=="
                      ChangeKey="AQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiRd5" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:PermissionSet" />
              <t:Folder>
                <t:PermissionSet>
                  <t:Permissions>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Default</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                    <t:Permission>
                      <t:UserId>
                        <t:DistinguishedUser>Anonymous</t:DistinguishedUser>
                      </t:UserId>
                      <t:PermissionLevel>None</t:PermissionLevel>
                    </t:Permission>
                  </t:Permissions>
                </t:PermissionSet>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

**NoError**更新が正常に完了したことを示すは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値が含まれています**UpdateFolderResponse**メッセージから**UpdateFolder**要求にサーバーが応答します。
  
## <a name="updating-folder-permissions-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してフォルダーのアクセス許可を更新する
<a name="bk_updateewsma"> </a>

EWS マネージ API を使用して、特定のフォルダーのフォルダーのアクセス許可を更新することもできます。アクセス許可を更新するには、次を行います。  
  
1. 旧式のアクセス許可では、[フォルダーのアクセス許可を削除する](#bk_removeewsma)は、 **Update**メソッドを (まだ)。 
    
2. [新規または変更されたユーザーのフォルダーのアクセス許可を追加](#bk_enableewsma)します。
    
3. 変更を保存するのには**Update**メソッドを呼び出します。 
    
以下の説明と共に**ServiceResponseException**エラーが発生する、同じユーザーのアクセス許可の 2 つのセットを追加しようとする場合:「指定されたアクセス許可セットには、重複するユーザー Id が含まれています」。 その場合は、現在のアクセス許可を**アクセス許可**のコレクションから削除し、**アクセス許可**のコレクションに新しいアクセス許可を追加します。 
  
## <a name="updating-folder-permissions-by-using-ews"></a>EWS を使用してフォルダーのアクセス許可を更新する
<a name="bk_updateews"> </a>

EWS を使用して、削除と追加のプロセスを組み合わせ、特定のフォルダーのフォルダーのアクセス許可を更新することもできます。アクセス許可を更新するには、次を行います。  
  
1. **GetFolder**操作を使用してフォルダーの現在のアクセス許可を取得します。 
    
2. **UpdateFolder**オペレーションを使用してアクセス許可の更新の一覧を送信します。 
    
これらは、EWS を使用して[有効にする](#bk_enableews)か、[アクセス権を削除](#bk_removeews)するを使用する 2 つの操作で同じです。 唯一の違いは、 **GetFolder**の応答が表示されたら、それが含まれている**アクセス許可**がユーザーの設定です。 だけで新しい**アクセス許可**要素では、その既存の**アクセス許可**要素を置換し、新しい**アクセス許可**の値または値を持つ**UpdateFolder**操作を送信します。 
  
同じユーザーのアクセス許可の 2 つのセットを追加しようとする場合は、 **ErrorDuplicateUserIdsSpecified**の**ResponseCode**の値を受け取ります。 場合は、要求からユーザーのアクセス許可の古い値を削除し、要求を再試行します。

## <a name="next-steps"></a>次の手順

ユーザーのアクセス許可を特定のフォルダーに設定した後、そのユーザーは代理人としてフォルダーにアクセスできます。詳細については、次のトピックをご覧ください。
  
- [EWS を使用して Exchange 内で代理人として電子メールにアクセスします。](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [EWS を使用して Exchange 内で代理人に予定表にアクセスします。](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用して代理人としてアクセス連絡先](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目

- [Exchange での代理人アクセスと EWS](delegate-access-and-ews-in-exchange.md)   
- [追加し、Exchange の EWS を使用して、デリゲートを削除します。](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [Exchange の EWS のフォルダーとアイテム](folders-and-items-in-ews-in-exchange.md)
    

