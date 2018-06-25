---
title: Exchange EWS を使用してフォルダーを操作します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4b3eb746-74c4-42a0-aa2c-742c147f1871
description: Exchange で EWS マネージ API または EWS を使用して、フォルダーを作成、取得、更新、削除する方法について説明します。
ms.openlocfilehash: a9a9e5974b2751268f37a1c9faacce43a333bcdb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759091"
---
# <a name="work-with-folders-by-using-ews-in-exchange"></a>Exchange EWS を使用してフォルダーを操作します。

Exchange で EWS マネージ API または EWS を使用して、フォルダーを作成、取得、更新、削除する方法について説明します。
  
Exchange 内では、構成して、メールボックスを整理するフォルダーを使用します。 ことができます新規作成、取得、更新、および EWS マネージ API または EWS を使用してフォルダーを削除します。 [フォルダー](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx)オブジェクト、[フォルダー](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx)の種類、または[フォルダーの派生クラスや型のいずれか](folders-and-items-in-ews-in-exchange.md#bk_folders)の個々 のメソッドまたは次の表に記載されている操作が実行されます。
  
**表 1 です。メソッドおよび操作の作成、取得、更新、およびフォルダーを削除します。**

|**目的…**|**EWS マネージ API メソッド**|**EWS 操作**|
|:-----|:-----|:-----|
|フォルダーを作成する  <br/> |[Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx) <br/> |[CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> |
|フォルダー階層の作成  <br/> |利用不可  <br/> |[CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx) <br/> |
|フォルダーを取得する  <br/> |[Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> |[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> |
|フォルダー階層の取得  <br/> |[Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> |[FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
|フォルダーを更新する  <br/> |[Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|フォルダーを削除する  <br/> |[Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> |[DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> |

<a name="bk_createfolderewsma"> </a>

## <a name="create-a-folder-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してフォルダーを作成する

クラスを使用して、[フォルダー](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder%28v=exchg.80%29.aspx)のカスタム フォルダーの[表示名](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx)と IPF の[FolderClass](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.folderclass%28v=exchg.80%29.aspx)プロパティの値を新しいジェネリック フォルダーを作成する次のコード例を次に示します。注意してください。 [Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx)メソッドは、受信トレイ フォルダーの子フォルダーとして、フォルダーを保存します。 
  
これらの例は、その**サービス**を想定しています、有効な[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトは、ユーザーが Exchange サーバーに認証されています。 
  
```cs
// Create a custom folder.
Folder folder = new Folder(service);
folder.DisplayName = "Custom Folder";
folder.FolderClass = "IPF.Note";
// Save the folder as a child folder of the Inbox.
folder.Save(WellKnownFolderName.Inbox);
```

フォルダー、 [CalendarFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.calendarfolder%28v=exchg.80%29.aspx)、[メッセージ](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.contactsfolder%28v=exchg.80%29.aspx)、 [SearchFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.searchfolder%28v=exchg.80%29.aspx)、 [TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx)などのさまざまなタイプを作成する (**フォルダー**のジェネリック クラス) ではなく特定のクラスの新しいインスタンスを作成し、設定しないで、**FolderClass**プロパティです。 たとえば、次のコード例は、新しい[TasksFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.tasksfolder%28v=exchg.80%29.aspx)を作成する方法を示します。
  
```cs
// Create a custom Tasks folder.
TasksFolder folder = new TasksFolder(service);
folder.DisplayName = "Custom Tasks";
// Save the folder as a child folder in the Inbox folder.
// This method call results in a CreateFolder call to EWS.
folder.Save(WellKnownFolderName.Inbox);
```

特定のクラスのインスタンスを作成し、 **FolderClass**プロパティを設定しようとすると、 [ErrorNoFolderClassOverride](http://msdn.microsoft.com/en-us/library/exchangewebservices.responsecodetype%28v=exchg.80%29.aspx)エラーがスローされます。 
  
EWS マネージ API を使用して、1 つのメソッドで複数のフォルダーの作成をバッチ操作することはできません。
  
## <a name="create-a-folder-by-using-ews"></a>EWS を使用してフォルダーを作成する
<a name="bk_createfolderews"> </a>

EWS を使用すると、1 つまたは複数のフォルダーを作成できます。
  
1 つのフォルダーを作成するには、 [CreateFolder](http://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx)操作の要求メッセージを送信します。 **CreateFolder**操作の要求は、親フォルダーは、受信トレイでは、[表示名](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx)は、[カスタム フォルダー]、および[FolderClass](http://msdn.microsoft.com/library/0041d135-2869-4612-89a5-d1aa86aa1093%28Office.15%29.aspx)要素の値は、IPF ことを示します。注意してください。 
  
EWS のマネージ API が新しいフォルダーを作成し、 [Folder.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.save%28v=exchg.80%29.aspx)メソッドを呼び出すときに送信する XML 要求にもです。 
  
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
    <m:CreateFolder>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderId>
      <m:Folders>
        <t:Folder>
          <t:FolderClass>IPF.Note</t:FolderClass>
          <t:DisplayName>Custom Folder</t:DisplayName>
        </t:Folder>
      </m:Folders>
    </m:CreateFolder>
  </soap:Body>
</soap:Envelope>
```

サーバー要求に応答し、 **CreateFolder** **NoError**フォルダーが正常に作成されたことを示すとの[フォルダー Id](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx)の[ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx)の値が含まれています[CreateFolderResponse](http://msdn.microsoft.com/library/158adecc-491a-47d9-af73-acc2cd3f8566%28Office.15%29.aspx)メッセージ新しく作成されたメッセージです。 
  
**CreateFolder**操作の要求メッセージに複数のフォルダーを作成するには、[フォルダー](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx)の複数の要素が含まれます。 すべての新しいフォルダーは、同じ親フォルダーにある必要があります。 
  
## <a name="create-a-folder-hierarchy-by-using-ews"></a>EWS を使用してフォルダー階層を作成する
<a name="bk_createfolderhierarchy"> </a>

EWS [CreateFolderPath](http://msdn.microsoft.com/library/5a10aa5e-3f25-4ec3-a0b9-284c30918a1f%28Office.15%29.aspx)操作を使用して 1 回の呼び出しで、フォルダー階層を作成できます。 同じ機能は、EWS のマネージ API で使用可能ではありません。 代わりに、EWS のマネージ API を使用する場合[EWS を使用してフォルダーを作成する](#bk_createfolderews)に示すように、1 つのフォルダーを作成できます。
  
> [!NOTE]
> EWS マネージ API はこの機能を実装していません。 
  
## <a name="get-a-folder-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してフォルダーを取得する
<a name="bk_getfolderewsma"> </a>

次のコード例では、 [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx)メソッドを使用して、受信トレイ フォルダーを取得する方法を示します。 ベスト プラクティスとして、アプリケーションに必要なものだけに返されるプロパティを制限します。 この例では、[プロパティ設定](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx)オブジェクトを作成し、 [BasePropertySet](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset.basepropertyset%28v=exchg.80%29.aspx)プロパティに[IdOnly](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.basepropertyset%28v=exchg.80%29.aspx)の値を適用することによってのみ、 [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx)プロパティに戻り値のプロパティを制限します。 
  
この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。 
  
```cs
// As a best practice, limit the properties returned to only those that are required.
// In this scenario, you only need the FolderId.
PropertySet propSet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get only the properties specified in the PropertySet.
// This method call results in a GetFolder call to EWS.
Folder rootfolder = Folder.Bind(service, WellKnownFolderName.Inbox, propSet);
```

**プロパティ設定**では、 [FolderSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderschema%28v=exchg.80%29.aspx)クラスからプロパティを追加または、オーバー ロードされたいずれかを使用して、追加のプロパティを取得する場合は、最初のクラスのすべてのプロパティを返すメソッドの[バインド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx)します。 
  
EWS のマネージ API を使用して複数のフォルダーを一度に 1 つを取得できない場合に注意してください。 メソッドを呼び出して、**バインド**フォルダーごとに個別にする必要があります。 
  
## <a name="get-a-folder-by-using-ews"></a>EWS を使用してフォルダーを取得する
<a name="bk_getfolderews"> </a>

EWS を使用すると、1 つまたは複数のフォルダーを取得できます。
  
1 つのフォルダーを取得するには、 [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)操作の要求メッセージをサーバーに送信します。 [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx)の設定次の例では、 **IdOnly**にのみ、[フォルダー Id](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx)の指定されたフォルダーが返されます。 [FolderIds](http://msdn.microsoft.com/library/3ff9d15a-7220-4785-ae6b-583a7eb82005%28Office.15%29.aspx)要素を取得するフォルダーが受信トレイ フォルダーであることを示します。 
  
EWS のマネージ API が、 [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx)メソッドを使用してフォルダーにバインドするときに送信する XML 要求にもです。 
  
**GetFolder**操作の要求メッセージに複数のフォルダーを取得するには、複数の[FolderIds](http://msdn.microsoft.com/library/812948d8-c7db-45ce-bb3a-77233a53a974%28Office.15%29.aspx)要素が含まれます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="inbox" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

**GetFolder**操作要求への応答としてクライアントにサーバーから送信される[GetFolderResponse](http://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx)メッセージを次の XML 例に示します。 のみ、受信トレイ フォルダーの[フォルダー Id](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx)の値が含まれています。 読みやすくするため、一部の属性と要素の値が短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="800"
                         MinorBuildNumber="16"
                         Version="V2_6"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
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
              <t:FolderId Id="AAAENAAA=" ChangeKey="AQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAEkbCr"/>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="get-a-folder-hierarchy-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してフォルダー階層を取得する
<a name="bk_getfolderhierarchyewsma"> </a>

次のコード例は、指定したルート フォルダーのサブフォルダーを取得する方法を示します。 この例では、(メールボックスのフォルダーとアイテムが格納)、IPM サブツリーのルートでは、 **MsgFolderRoot**フォルダー内のサブフォルダーを取得します。 
  
この例では、 [Folder.FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)メソッドの応答の結果を制限する[FolderView](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview%28v=exchg.80%29.aspx)クラスのオブジェクトが作成されます。 このシナリオは、次に戻るにはプロパティを制限: [Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx)、[表示名](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx)、およびフォルダーが隠しフォルダーであるかどうかを示す拡張プロパティです。 サーバーが、サブフォルダーを取得するために再帰的な検索を実行する高度に[FolderView.Traversal](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderview.traversal%28v=EXCHG.80%29.aspx)値を設定し、 **MsgFolderRoot**にルート フォルダーを設定して、サーバーがすべてのユーザーのフォルダーを返します (およびサーバーを返さないようにシステム内のフォルダー、非 IPM サブツリー) です。
  
この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。 
  
```XML
// Create a new folder view, and pass in the maximum number of folders to return.
FolderView view = new FolderView(folderViewSize);
// Create an extended property definition for the PR_ATTR_HIDDEN property,
// so that your results will indicate whether the folder is a hidden folder.
ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
// As a best practice, limit the properties returned to only those required.
// In this case, return the folder ID, DisplayName, and the value of the isHiddenProp
// extended property.
view.PropertySet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.DisplayName, isHiddenProp);
// Indicate a Traversal value of Deep, so that all subfolders are retrieved.
view.Traversal = FolderTraversal.Deep;
// Call FindFolders to retrieve the folder hierarchy, starting with the MsgFolderRoot folder.
// This method call results in a FindFolder call to EWS.
FindFoldersResults findFolderResults = service.FindFolders(WellKnownFolderName.MsgFolderRoot, view);
```

## <a name="get-a-folder-hierarchy-by-using-ews"></a>EWS を使用してフォルダー階層を取得する
<a name="bk_getfolderhierarchyews"> </a>

次の XML の例では、EWS を使用してフォルダー階層を取得するために、 [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)操作を使用する方法を示します。 この例では、IPM サブツリーとそのすべてのサブフォルダーのルートは、[ **msgfolderroot** ] フォルダーを取得します。 サーバーは、フォルダー階層の再帰的な検索を実行し、のみフォルダーおよびサブフォルダーを指定したルートの下の応答が返されますようにに**深い****トラバーサル**属性が設定されています。 [BaseShape](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx)の要素は、この例では、サーバーは[フォルダー Id](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx)の要素だけを返しますように**IdOnly**に設定されています。 出力を簡単に理解するためには、 **DisplayName**要素の結果に含めると、 **ExtendedFieldURI**の値**PR_ATTR_HIDDEN**要求内の[AdditionalProperties](http://msdn.microsoft.com/library/7a269aed-dcfd-4c3e-9e14-094e53828101%28Office.15%29.aspx)要素を含んでプロパティ、フォルダーは隠しフォルダーであるかどうかを把握するようにします。 
  
EWS のマネージ API が、 [FindFolders](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx)メソッドを呼び出すときに送信する XML 要求にもです。 
  
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
    <m:FindFolder Traversal="Deep">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="100"
                               Offset="0"
                               BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="msgfolderroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

**FindFolder**操作の要求への応答としてクライアントにサーバーから送信される[FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx)メッセージを次の XML 例に示します。 のみ、[フォルダー Id](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx)、[表示名](http://msdn.microsoft.com/library/e7efbbe1-6629-4d11-bed1-ed899e3f9d77%28Office.15%29.aspx)が含まれており、 **PR_ATTR_HIDDEN**の値は、 **msgrootfolder**フォルダーの下のすべてのサブフォルダーのプロパティを拡張します。 [値](http://msdn.microsoft.com/library/9a30cadd-909e-41b1-b4e9-291643dd89c6%28Office.15%29.aspx)要素設定されている場合 true の場合、フォルダーを非表示に、クライアント ビューにします。 
  
[FindFolder](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)メソッドを使用して複数のフォルダーを取得する場合、EWS のマネージ API を送信する XML 応答にもです。 読みやすいように、いくつかの属性と要素の値に短縮されていて、いくつかのフォルダーは簡潔にするために含まれていません。 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="815"
                         MinorBuildNumber="6"
                         Version="V2_7"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="16"
                        TotalItemsInView="16"
                        IncludesLastItemInRange="true">
            <t:Folders>
              <t:CalendarFolder>
                <t:FolderId Id="AAAEOAAA="
                            ChangeKey="AgAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAA3"/>
                <t:DisplayName>Calendar</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>false</t:Value>
                </t:ExtendedProperty>
              </t:CalendarFolder>
              <t:ContactsFolder>
                <t:FolderId Id="AAAEPAAA="
                            ChangeKey="AwAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAA4"/>
                <t:DisplayName>Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>false</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="AAAUKAAA="
                            ChangeKey="AwAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAAS5"/>
                <t:DisplayName>Recipient Cache</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="AAAUJAAA="
                            ChangeKey="AQAAABYAAAAPxolXAHv3TaHUnjW8wWqXAAAAAASx"/>
                <t:DisplayName>Conversation Action Settings</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean"/>
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
…
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

## <a name="update-a-folder-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してフォルダーを更新する
<a name="bk_updatefolderewsma"> </a>

次のコード例は、EWS マネージ API を使用してフォルダーの表示名を更新する方法を示しています。
  
最初に、 [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx)の応答でサーバーを取得するプロパティの数を制限する[プロパティ設定](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.propertyset%28v=exchg.80%29.aspx)を作成します。 **IdOnly** **BasePropertySet**を使用して、Exchange データベースへの呼び出しを削減することをお勧めします。 次に、フォルダーへのバインドを更新するのには、 **Bind**メソッドを使用します。 [DisplayName](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.displayname%28v=exchg.80%29.aspx)プロパティを更新し、変更を保存する[Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx)メソッドを使用します。 
  
この例と仮定するとその**サービス**は、有効な[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトと、ユーザーが Exchange サーバーに認証されています。 ローカル変数*フォルダー Id*は、更新するフォルダーの[Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx)です。 
  
```cs
// As a best practice, only include the ID value in the PropertySet.
PropertySet propertySet = new PropertySet(BasePropertySet.IdOnly);
// Bind to an existing folder and get the FolderId.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId, propertySet);
// Update the display name of the folder.
folder.DisplayName = "Updated folder name";
// Save the updates.
// This method call results in an UpdateFolder call to EWS.
folder.Update();

```

## <a name="update-a-folder-by-using-ews"></a>EWS を使用してフォルダーを更新する
<a name="bk_updatefolderews"> </a>

次のコード例は、EWS を使用してフォルダーの表示名を更新する方法を示しています。
  
最初に、 [EWS を使用してフォルダーの階層を取得するの](#bk_getfolderhierarchyews)に示すように更新するにはフォルダーを取得するには、 [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)操作要求メッセージを送信します。
  
[UpdateFolder](http://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx)操作の要求メッセージを次に、フォルダーを更新するにはサーバーに送信するには。 **UpdateFolder**操作の要求は、[カスタム フォルダーの更新] に[表示名](http://msdn.microsoft.com/library/42c04f3b-abaa-4197-a3d6-d21677ffb1c0%28Office.15%29.aspx)を更新します。 
  
EWS のマネージ API が、 [Folder.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx)メソッドを使用してフォルダーを更新するときに送信する XML 要求にもです。 読みやすくするため、一部の属性と要素の値が短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="OrV9ZAAA=" ChangeKey="AQAAABYAAABVzRdyy/cHS4XTC9itCRdUAAAOrXWb" />
          <t:Updates>
            <t:SetFolderField>
              <t:FieldURI FieldURI="folder:DisplayName" />
              <t:Folder>
                <t:DisplayName>Updated Custom Folder</t:DisplayName>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

サーバー要求に応答し、 **UpdateFolder** [UpdateFolderResponse](http://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx)メッセージが含まれている**NoError**をし、更新された**で更新されているフォルダーの[フォルダー Id](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx)の[ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx)値変更キー**属性の値です。 
  
## <a name="delete-a-folder-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してフォルダーを削除する
<a name="bk_deletefolderewsma"> </a>

この資料では、EWS のマネージ API を使用してフォルダーを削除する方法を示す基本的な例を提供します。 フォルダーを削除する方法の詳細については、 [Exchange で EWS を使用してアイテムを削除する](deleting-items-by-using-ews-in-exchange.md)を参照してください。
  
EWS のマネージ API を使用してフォルダーを削除するのには最初に、削除するフォルダーにサービス オブジェクトにバインドするのには、 [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx)メソッドを使用します。 次に、 [HardDelete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.deletemode%28v=exchg.80%29.aspx)の削除モードを使用してフォルダーを削除するのには、 [Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx)メソッドを使用します。 
  
この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。 ローカル変数*フォルダー Id*は、削除するフォルダーの[Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx)です。 
  
```cs
// Bind to an existing folder and get all its properties.
// This method call results in a GetFolder call to EWS.
Folder folder = Folder.Bind(service, folderId);
// HardDelete the folder.
// This method call results in a DeleteFolder call to EWS.
folder.Delete(DeleteMode.HardDelete);
```

## <a name="delete-a-folder-by-using-ews"></a>EWS を使用してフォルダーを削除する
<a name="bk_deletefolderews"> </a>

この資料では、EWS を使用してフォルダーを削除する方法を示す基本的な XML の例を提供します。 フォルダーを削除する方法の詳細については、 [Exchange で EWS を使用してアイテムを削除する](deleting-items-by-using-ews-in-exchange.md)を参照してください。
  
EWS を使用してフォルダーを削除するのにはまず、 [EWS を使用してフォルダーを取得する](#bk_getfolderews)ようにを更新するフォルダーを取得するのには、 [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)操作の要求メッセージを送信します。 
  
次に、フォルダーを削除するサーバーに[DeleteFolder](http://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx)操作の要求メッセージを送信します。 **DeleteFolder**操作の要求を示します**削除の種類**は、 **HardDelete**を削除するフォルダーの[フォルダー Id](http://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx)が含まれています。 
  
[Folder.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx)メソッドを使用してフォルダーを削除すると、EWS のマネージ API を送信する XML 要求にもです。 読みやすくするため、一部の属性と要素の値が短縮されています。 
  
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
    <m:DeleteFolder DeleteType="HardDelete">
      <m:FolderIds>
        <t:FolderId Id="OrV9ZAAA=" ChangeKey="AQAAABYAAABVzRdyy/cHS4XTC9itCRdUAAAOrXWf" />
      </m:FolderIds>
    </m:DeleteFolder>
  </soap:Body>
</soap:Envelope>
```

サーバー要求に応答し、 **DeleteFolder**を含む[DeleteFolderResponse](http://msdn.microsoft.com/library/27578bda-ef0a-4a33-bccc-2c1bc1735424%28Office.15%29.aspx)メッセージで、 [ResponseCode](http://msdn.microsoft.com/en-us/library/aa580757%28v=exchg.150%29.aspx) **NoError**フォルダーの削除が成功したことを示す値です。
  
## <a name="next-steps"></a>次の手順
<a name="bk_nextsteps"> </a>

サーバー上のフォルダーを取得または、フォルダーを変更した後[、フォルダー階層の同期](how-to-synchronize-folders-by-using-ews-in-exchange.md)またはサーバー上の[フォルダーの変更についての通知を購読する](notification-subscriptions-mailbox-events-and-ews-in-exchange.md)にする可能性があります。 
  
## <a name="see-also"></a>関連項目

- [Exchange の EWS のフォルダーとアイテム](folders-and-items-in-ews-in-exchange.md)   
- [EWS を使用して Exchange で Exchange メールボックスのアイテムを扱う](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)    
- [Exchange の EWS を使用するアイテムの削除](deleting-items-by-using-ews-in-exchange.md)   
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    

