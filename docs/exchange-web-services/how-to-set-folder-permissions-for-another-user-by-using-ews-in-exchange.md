---
title: Exchange で EWS を使用して別のユーザーのフォルダーのアクセス許可を設定する
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7eb81676-a780-4c56-b4f2-c4ed2697107d
description: Exchange で EWS マネージ API または EWS を使用して、フォルダーのアクセス許可レベルを設定する方法について説明します。
ms.openlocfilehash: 5bf570612d6349628e7f3abf858daa33daa13745
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759062"
---
# <a name="set-folder-permissions-for-another-user-by-using-ews-in-exchange"></a>Exchange で EWS を使用して別のユーザーのフォルダーのアクセス許可を設定する

Exchange で EWS マネージ API または EWS を使用して、フォルダーのアクセス許可レベルを設定する方法について説明します。
  
フォルダー レベルのアクセス許可によって、ユーザーは、他のユーザーのメールボックスの 1 つ以上のフォルダーにアクセス可能になります。フォルダーのアクセス許可は代理人アクセスに似ていますが、次のような相違点があります。  
  
- フォルダーのアクセス許可では、ユーザーに "代理人として送信" させたり、別のユーザーとして "差出人を指定して送信" したりすることはできません。 ユーザーは、フォルダーにのみアクセスできます。 ユーザーは、フォルダーのアイテムを作成できますが、それらを送信することはできません。
    
- メールボックスの任意のフォルダーで、フォルダーのアクセス許可を設定できますが、代理人を追加できるのは、予定表、連絡先、受信トレイ、履歴、メモ、タスクのフォルダーのみです。
    
- [特定のフォルダーのアクセス許可](#bk_folderperms)の数を設定できます。 代理人を追加する場合、[5 つのアクセス許可レベル](delegate-access-and-ews-in-exchange.md#bk_delegateperms)の内 1 つのみを割り当てることができます。
    
- 匿名ユーザーおよび既定ユーザーのフォルダーのアクセス許可を設定できます。メールが有効なアカウントにだけ代理人アクセスを付与できます。
    
アクセス制御エントリ (ACE) と随意アクセス制御リスト (DACL) に精通していれば、ユーザーが各フォルダーのアクセス許可のセットを 1 つだけ持てることをご存じでしょう。ユーザーにアクセス許可のセットを追加しようとすると、そのユーザーがアクセス許可のセットを既に持っている場合、エラーが返されます。フォルダーのアクセス許可を追加、削除、更新する場合、現在の DACL を取得し、任意の ACE を追加するか削除し、更新した DACL を送信します。同じユーザーに対して複数の ACE を追加することはできません。EWS マネージ API を使用してアクセス許可を更新する場合、ユーザーの現在の ACE を削除し、新しい ACE をコレクションに追加する必要があります。EWS を使用している場合は、以前の ACE のセットを新しいセットに置き換えるだけです。
  
1 つのフォルダーで複数のアクセス許可を変更する場合は、追加、削除、更新をバッチ処理することができます。複数のフォルダーでユーザーの更新をするときには、バッチ処理はできないことに注意してください。1 つのフォルダーのアクセス許可を取得するために、1 回の呼び出しが必要です。そのフォルダーに対するアクセス許可を更新するには、2 番目の呼び出しが必要です。ユーザーのアクセス許可を追加、削除、更新する場合、各タスクで、同じ 2 つのメソッド呼び出しまたは操作を使用します。
  
**表 1. フォルダー アクセス許可を設定する EWS マネージ API メソッドと EWS 操作**

|目的|使用する EWS マネージ API メソッド…|使用する EWS 操作…|
|:-----|:-----|:-----|
|フォルダーのアクセス許可の有効化、削除、更新  <br/> |[Folder.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) の後に [Folder.Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.reply%28v=exchg.80%29.aspx) <br/> |[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) の後に [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|フォルダーの作成、フォルダーのアクセス許可の定義  <br/> |[Folder.Save](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
   
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
    
さらに、次のアクセス許可レベルを使用できます。それは、表 2 に示すように個別アクセス許可と値のサブセットを定義します。
  
- なし    
- Owner (所有者)    
- PublishingEditor (出版編集者)    
- Editor (編集者)    
- PublishingAuthor (出版著者)    
- Author (著者)    
- NoneditingAuthor (非編集著者)    
- Reviewer (校閲者)    
- 共同作成者   
- Custom: この値は、アプリケーションでは設定できません。 個別アクセス許可のカスタム コレクションがアプリケーションに含まれている場合、サーバーはこの値を設定します。    
- FreeBusyTimeOnly: これは予定表フォルダーにのみ設定できます。   
- FreeBusyTimeAndSubjectAndLocation: これは予定表フォルダーにのみ設定できます。
    
次の表は、アクセス許可レベルに基づき、既定で適用される個別アクセス許可を示しています。
  
**表 2.アクセス許可レベルによる個別アクセス許可**

|権限レベル|アイテム作成可能|サブ フォルダー作成可能|フォルダーの所有者になる|フォルダーを表示可能|連絡先フォルダーにする|アイテムの編集|アイテムの削除|アイテムの参照可能|
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
   
フォルダー レベルのアクセス許可の要求でカスタム以外のアクセス許可レベルを指定する場合、個別アクセス許可の設定を指定する必要はありません。 アクセス許可レベルを設定する場合、個別アクセス許可を指定すると、応答で **ErrorInvalidPermissionSettings** エラーが返されます。 
  
## <a name="adding-folder-permissions-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してフォルダーのアクセス許可を追加する
<a name="bk_enableewsma"> </a>

次のコード例は、以下の目的で EWS マネージ API を使用する方法を示しています。 
  
- 新規ユーザーに対して [FolderPermission](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderpermission%28v=exchg.80%29.aspx) オブジェクトを新規作成する。 
    
- [Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) メソッドを使用して、フォルダーに対する現在のアクセス許可を取得する。 
    
- 新しい **FolderPermissions** を [Folder.Permissions](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.permissions%28v=exchg.80%29.aspx) プロパティに追加する。 
    
- [Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) メソッドを呼び出して、サーバーに新規アクセス許可を保存する。 
    
この例では、**service** はメールボックス所有者の有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーは Exchange サーバーに既に認証されていると想定しています。 
  
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

**FolderPermission** オブジェクトをカスタム アクセス許可レベルで作成する場合、書き込み可能な [FolderPermission プロパティ](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderpermission_properties%28v=exchg.80%29.aspx)の一部またはすべてを設定できます。 ただし、アプリケーションが [FolderPermissionLevel](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderpermissionlevel%28v=exchg.80%29.aspx) を明示的に **Custom** に設定することは決してないことにご注意ください。 **FolderPermission** オブジェクトを作成し、個別アクセス許可を設定する場合のみ、**FolderPermissionLevel** は Custom に設定されます。 
  
## <a name="adding-folder-permissions-by-using-ews"></a>EWS を使用してフォルダーのアクセス許可を追加する
<a name="bk_enableews"> </a>

次の EWS のコード例では、現在のアクセス許可を取得し、新しいアクセス許可の一覧を送信することによって、特定のフォルダーにアクセス許可を追加する方法を示しています。
  
最初の手順は、[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) 要求を送信することです。この要求では、[DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) 値でアクセス許可を追加するフォルダー (この例では [送信済みアイテム] フォルダー) を指定し、[FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) 値に folder:PermissionSet を含んでいます。 この要求は、指定したフォルダーのアクセス許可設定を取得します。 
  
これは、[フォルダーのアクセス許可を追加する](#bk_enableewsma)ために **Bind** メソッドを呼び出す際に、EWS マネージ API が送信する XML 要求でもあります。
  
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

サーバーは、**GetFolder** 要求に [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) メッセージで応答します。このメッセージには、フォルダーが正常に取得されたことを示す、値が **NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素が含まれます。 [FolderId](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) 値と [ParentFolderId](http://msdn.microsoft.com/library/258f4b1f-367e-4c7d-9c29-eb775a2398c7%28Office.15%29.aspx) 値は、読みやすくするために短縮してあります。 
  
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

次に、**UpdateFolder** 操作を使用して、更新された [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) を送信します。それには、新規ユーザーのための [Permission](http://msdn.microsoft.com/library/b8d0429a-0e58-4480-9847-4901970c7033%28Office.15%29.aspx) が含まれています。 [UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) 操作で各フォルダーの [SetFolderField](http://msdn.microsoft.com/library/8c69db7b-54b5-4ae2-abca-4d6e0937a790%28Office.15%29.aspx) 要素を含めると、そのフォルダーのすべてのアクセス許可設定が上書きされることに注意してください。 同様に、**UpdateFolder** 操作の [DeleteFolderField](http://msdn.microsoft.com/library/f9c2187b-4c60-4358-b4b4-ede50eadae48%28Office.15%29.aspx) オプションを含めると、フォルダーのすべてのアクセス許可設定が削除されます。 
  
これは、[フォルダーのアクセス許可を追加する](#bk_enableewsma)ために **Update** メソッドを呼び出す際に、EWS マネージ API が送信する XML 要求でもあります。
  
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

サーバーは、**UpdateFolder** 要求に [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) メッセージで応答します。このメッセージには、フォルダーが正常に更新されたことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素の値が含まれます。
  
## <a name="removing-folder-permissions-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してフォルダーのアクセス許可を削除する
<a name="bk_removeewsma"> </a>

次のコード例は、既定および匿名のアクセス許可を除く、特定のフォルダーのすべてのユーザーのアクセス許可を削除するために、EWS マネージ API を使用する方法を示しています。
  
1. **Bind** メソッドを使用して、フォルダーの現在のアクセス許可を取得します。 
    
2. **Permissions** コレクションを反復処理し、個別ユーザーのアクセス許可を削除します。 
    
3. **Update** メソッドを呼び出して、変更を保存します。 
    
この例では、フォルダーのすべてのユーザー アクセス許可を削除します。特定のユーザーのアクセス許可のみを削除するようこの例を変更する場合、次のコードの行を変更して、ユーザーの表示名、または SMTP アドレスのいずれかを識別できるようにします。
  
```cs
if (sentItemsFolder.Permissions[t].UserId.DisplayName != null || sentItemsFolder.Permissions[t].UserId.PrimarySmtpAddress != null)
```

この例では、**service** はメールボックス所有者の有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーは Exchange サーバーに既に認証されていると想定しています。 
  
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
  
最初の手順は、[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) 要求を送信することです。この要求では、[DistinguishedFolderId](http://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) 値でアクセス許可を削除するフォルダー (この例では [送信済みアイテム] フォルダー) を指定し、[FieldURI](http://msdn.microsoft.com/library/24af8e3b-3074-4c8c-8d0a-52446508d044%28Office.15%29.aspx) 値に folder:PermissionSet を含んでいます。 この要求は、指定したフォルダーの [PermissionSet](http://msdn.microsoft.com/library/6ac1bd17-a089-46bb-b9e6-f5b1dfe1076d%28Office.15%29.aspx) を取得します。 
  
これは、[フォルダーのアクセス許可を削除する](#bk_removeewsma)ために **Bind** メソッドを呼び出す際に、EWS マネージ API が送信する XML 要求でもあります。
  
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

サーバーは、**GetFolder** 要求に [GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) メッセージで応答します。このメッセージには、フォルダーが正常に取得されたことを示す、値が **NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素が含まれます。 **FolderId** 要素の値と **ParentFolderId** 要素の値は、読みやすくするために短縮してあります。 
  
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

次に、**UpdateFolder** 操作を使用し、更新された **PermissionSet** を送信します。削除したユーザーの **Permission** は含まれていません。 
  
これは、[フォルダーのアクセス許可を削除する](#bk_removeewsma)ために **Update** メソッドを呼び出す際に、EWS マネージ API が送信する XML 要求でもあります。
  
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

サーバーは、**UpdateFolderResponse** メッセージで **UpdateFolder** 要求に応答します。このメッセージには、更新が正常に完了したことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素の値が含まれます。
  
## <a name="updating-folder-permissions-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してフォルダーのアクセス許可を更新する
<a name="bk_updateewsma"> </a>

EWS マネージ API を使用して、特定のフォルダーのフォルダーのアクセス許可を更新することもできます。アクセス許可を更新するには、次のことを行います。 
  
1. 古いアクセス許可の[フォルダーのアクセス許可を削除します](#bk_removeewsma)が、(まだ) **Update** メソッドを呼び出しません。 
    
2. [新規または変更されたユーザーのフォルダーのアクセス許可を追加します](#bk_enableewsma)。
    
3. **Update** メソッドを呼び出して、変更を保存します。 
    
同じユーザーのアクセス許可の 2 つのセットを追加しようとする場合、「指定したアクセス許可のセットには、重複したユーザー Id が含まれています」という説明がある **ServiceResponseException** エラーを受け取ります。 このケースでは、**Permission** コレクションから現在のアクセス許可を削除してから、新しいアクセス許可を **Permission** コレクションに追加します。 
  
## <a name="updating-folder-permissions-by-using-ews"></a>EWS を使用してフォルダーのアクセス許可を更新する
<a name="bk_updateews"> </a>

EWS を使用して、削除と追加のプロセスを組み合わせ、特定のフォルダーのフォルダーのアクセス許可を更新することもできます。アクセス許可を更新するには、次のことを行います。 
  
1. **GetFolder** 操作を使用して、フォルダーの現在のアクセス許可を取得します。 
    
2. **UpdateFolder** 操作を使用して、更新されたアクセス許可の一覧を送信します。 
    
これらは、EWS を使用して[アクセスの有効化](#bk_enableews)または[アクセスの削除](#bk_removeews)を行うのに使用するのと同じ 2 つの操作です。 唯一の違いは、**GetFolder** 応答を受信したときにユーザーの **Permission** 設定が含まれていることです。 単に既存の **Permission** 要素を新しい **Permission** 要素に取り替え、新しい **Permission** の値 (複数の場合もある) を指定して **UpdateFolder** 操作を送信します。 
  
同じユーザーに、アクセス許可のセットを 2 つ追加しようとすると、値が **ErrorDuplicateUserIdsSpecified** の **ResponseCode** を受け取ります。 このケースでは、要求からユーザーのアクセス許可の古い値を削除してから、要求を再試行します。

## <a name="next-steps"></a>次の手順

ユーザーのアクセス許可を特定のフォルダーに設定した後、そのユーザーは代理人としてフォルダーにアクセスできます。詳細については、以下を参照してください。
  
- [Exchange で EWS を使用して、代理人としてメールにアクセスする](how-to-access-email-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用して予定表に代理人としてアクセスする](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用して、代理人として連絡先にアクセスする](how-to-access-contacts-as-a-delegate-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目

- [Exchange での代理人アクセスと EWS](delegate-access-and-ews-in-exchange.md)   
- [Exchange で EWS を使用して代理人を追加および削除する](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [Exchange の EWS のフォルダーとアイテム](folders-and-items-in-ews-in-exchange.md)
    

