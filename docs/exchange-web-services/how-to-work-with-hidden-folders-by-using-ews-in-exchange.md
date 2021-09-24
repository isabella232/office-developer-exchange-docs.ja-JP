---
title: Exchange で EWS を使用して隠しフォルダーを操作する
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: 7ae7c045-cd90-4c9f-baf5-0464d5058f45
description: Exchange で EWS マネージ API または EWS を使用して、フォルダーを非表示にしたり、隠しフォルダーを検索したりする方法について説明します。
ms.openlocfilehash: 722cc09aa62ae4201362c59f7d7d2b4988e25837
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513074"
---
# <a name="work-with-hidden-folders-by-using-ews-in-exchange"></a>Exchange で EWS を使用して隠しフォルダーを操作する

Exchange で EWS マネージ API または EWS を使用して、フォルダーを非表示にしたり、隠しフォルダーを検索したりする方法について説明します。
  
1 つの例外を除き、Exchange メールボックスのルート内 (非 IPM サブツリー) のフォルダーはユーザーから非表示になっています。 逆に、**MsgFolderRoot** (IPM サブツリー) 内のすべてのフォルダーはユーザーに表示されます。 **MsgFolderRoot** の下のフォルダーを非表示にしてみましょう。 それほど複雑ではありません。たった 1 つのプロパティ ([PidTagAttributeHidden](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx) (0x10F4000B) 拡張プロパティ) を操作するだけです。 このプロパティを **true** に設定すると、Outlook またはこのプロパティを使用してフォルダーの表示/非表示を決定する別のクライアントでは、ユーザーにはフォルダーが非表示になります。 これは拡張プロパティであるため、通常のフォルダー プロパティよりも使用するのが複雑です。そのため、この記事では、主なシナリオについて順を追って説明します。
  
**表 1. 隠しフォルダーを処理するための EWS マネージ API メソッドと EWS 操作**

|**タスク**|**EWS マネージ API メソッド**|**EWS 操作**|
|:-----|:-----|:-----|
|フォルダーを非表示にする  <br/> |[Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) の後に [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> |[GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) の後に [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> |
|隠しフォルダーを検索する  <br/> |[FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) <br/> |[FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> |
   
ルート内のフォルダーのうち、ユーザーに表示されている例外のフォルダーは、 Finder フォルダー (**SearchFolders**[WellKnownFolder](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) 列挙値または **searchfolders**[DistinguishedFolderId](https://msdn.microsoft.com/library/50018162-2941-4227-8a5b-d6b4686bb32f%28Office.15%29.aspx) 要素値とも呼ばれる) です。これにはユーザーの検索フォルダーが含まれます。 Finder フォルダーに作成される検索フォルダーは、Outlook ユーザーに表示されます。 ユーザーに表示されない検索フォルダーを作成する必要がある場合は、ルート フォルダーに移動して非表示にします。 他のフォルダーとは異なり、**PidTagAttributeHidden** プロパティを **true** に設定しても、Finder フォルダー内の検索フォルダーは非表示にされません。 
  
## <a name="hide-a-folder-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してフォルダーを非表示にする
<a name="bk_hideewsma"> </a>

[PidTagAttributeHidden](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx) 拡張プロパティを **true** に変更して、[既存のフォルダーを隠しフォルダーにする](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma)ことができます。 最初に、[プロパティ用に拡張プロパティの定義](properties-and-extended-properties-in-ews-in-exchange.md)を作成します。 次に、[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) メソッドを使用してフォルダーを見つけ、**PidTagAttributeHidden** プロパティの値を true に更新し、[Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) メソッドを使用して変更を保存します。 
  
この例では、**service** がメールボックスの所有者に対して有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーは Exchange サーバーから認証されており、**folderId** が非表示にされるフォルダーを識別する有効な [Folder.Id](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.id%28v=exchg.80%29.aspx) であることを想定しています。 
  
```cs
private static void MakeHidden(FolderId folderId, ExchangeService service)
{
    // Create an extended property definition for the PidTagAttributeHidden property.
    ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
    PropertySet propSet = new PropertySet(isHiddenProp);
    // Bind to a folder and retrieve the PidTagAttributeHidden property.
    Folder folder = Folder.Bind(service, folderId, propSet);
    // Set the PidTagAttributeHidden property to true.
    folder.SetExtendedProperty(isHiddenProp, true);
    // Save the changes.
    folder.Update();
}
```

## <a name="hide-a-folder-by-using-ews"></a>EWS を使用してフォルダーを非表示にする
<a name="bk_hideews"> </a>

[PidTagAttributeHidden](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx) 拡張プロパティを **true** に変更し、EWS を使用して、[既存のフォルダーを隠しフォルダーにする](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_createfolderewsma)ことができます。 最初に、[GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) 操作を使用してフォルダーを見つけ、[ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) 要素を含め、**PropertyTag** 値を 4340、**PropertyType** 値を Boolean に設定することによって **PidTagAttributeHidden** プロパティを取得します。 
  
これは、[隠しフォルダーにする](#bk_hideewsma)前にフォルダーを取得するため **Bind** メソッドを使用する際に、EWS マネージ API が送信する XML 要求でもあります。
  
[FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) 値は読みやすさのために短くしてあります。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:FolderIds>
        <t:FolderId Id="IQywAAAA==" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

サーバーは、**GetFolder** 要求に [GetFolderResponse](https://msdn.microsoft.com/library/47abeec8-78dd-4297-8525-099174ec880d%28Office.15%29.aspx) メッセージで応答します。このメッセージには、フォルダーが正常に取得されたことを示す、**NoError** の [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素の値が含まれます。この応答には、[ExtendedProperty](https://msdn.microsoft.com/library/196278d4-5e77-4e0a-8af6-8ac065610510%28Office.15%29.aspx) の [Value](https://msdn.microsoft.com/library/f9701409-b620-4afe-b9ee-4c1e95507af7%28Office.15%29.aspx) も含まれます。この例では、**Value** は **false** に設定されています。これは、フォルダーが現時点で非表示になっていないことを意味します。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="898"
                         MinorBuildNumber="23"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Folders>
            <t:Folder>
              <t:FolderId Id="IQywAAAA=="
                          ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAABED" />
              <t:ExtendedProperty>
                <t:ExtendedFieldURI PropertyTag="0x10f4"
                                    PropertyType="Boolean" />
                <t:Value>false</t:Value>
              </t:ExtendedProperty>
            </t:Folder>
          </m:Folders>
        </m:GetFolderResponseMessage>
      </m:ResponseMessages>
    </m:GetFolderResponse>
  </s:Body>
</s:Envelope>
```

**ExtendedProperty** の値を true に変更するには、[UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) 操作を使用します。**ExtendedProperty**、**ExtendedFieldURI**、**Value** 要素を **PidTagAttributeHidden** 拡張プロパティに含め、**Value** 要素を **true** に設定してフォルダーを非表示にします。  
  
これは、フォルダーを更新して [隠しフォルダーにする](#bk_hideewsma)ため **Update** メソッドを使用する際に、EWS マネージ API が送信する XML 要求でもあります。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:UpdateFolder>
      <m:FolderChanges>
        <t:FolderChange>
          <t:FolderId Id="IQywAAAA=="
                      ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAABED" />
          <t:Updates>
            <t:SetFolderField>
              <t:ExtendedFieldURI PropertyTag="4340"
                                  PropertyType="Boolean" />
              <t:Folder>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="4340"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:SetFolderField>
          </t:Updates>
        </t:FolderChange>
      </m:FolderChanges>
    </m:UpdateFolder>
  </soap:Body>
</soap:Envelope>
```

サーバーは、**UpdateFolder** 要求に [UpdateFolderResponse](https://msdn.microsoft.com/library/31f47739-dc9c-46ba-9e3f-cce25dc85e6e%28Office.15%29.aspx) メッセージで応答します。このメッセージには、フォルダーが正常に更新されて非表示にされたことを示す、**NoError** の [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素の値が含まれます。
  
## <a name="find-all-hidden-folders-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してすべての隠しフォルダーを検索する
<a name="bk_findhiddenewsma"> </a>

親フォルダーにあるすべての隠しフォルダーは、**PidTagAttributeHidden** 拡張プロパティの [拡張プロパティの定義](properties-and-extended-properties-in-ews-in-exchange.md)を作成し、[FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findfolders%28v=exchg.80%29.aspx) メソッドを使用して **PidTagAttributeHidden** 値が **true** に設定されているフォルダーを検索することによって見つけることができます。 この例では、MsgFolderRoot (インフォメーション ストアの先頭または IPM サブツリーとも呼ばれる) が、検索する親フォルダーとして使用されます。
  
この例では、**service** はメールボックス所有者の有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーは Exchange サーバーから既に認証されていると想定しています。 
  
```cs
private static void FindHiddenFolders(ExchangeService service)
{
    // Create an extended property definition for the PidTagAttributeHidden property.
    ExtendedPropertyDefinition isHiddenProp = new ExtendedPropertyDefinition(0x10f4, MapiPropertyType.Boolean);
    // Create a folder view to retrieve up to 100 folders and 
    // retrieve only the PidTagAttributeHidden and the display name.
    FolderView folderView = new FolderView(100);
    folderView.PropertySet = new PropertySet(isHiddenProp, FolderSchema.DisplayName);
    // Indicate a Traversal value of Deep, so that all subfolders are retrieved.
    folderView.Traversal = FolderTraversal.Deep;
    // Find all hidden folders under the MsgFolderRoot.
    // This call results in a FindFolder call to EWS.
    FindFoldersResults findFolder = service.FindFolders(WellKnownFolderName.MsgFolderRoot,
            new SearchFilter.IsEqualTo(isHiddenProp, true), folderView);
    // Display the folder ID and display name of each hidden folder.
    foreach (Folder folder in findFolder)
    {
        Console.WriteLine("FolderId: {0}", folder.Id);
        Console.WriteLine("DisplayName: {0}", folder.DisplayName);
        Console.WriteLine("\r\n");
    }
}
```

## <a name="find-all-hidden-folders-by-using-ews"></a>EWS を使用してすべての隠しフォルダーを検索する
<a name="bk_findhiddenews"> </a>

[FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) 操作を呼び出し、[PidTagAttributeHidden](https://msdn.microsoft.com/library/cc433490%28v=exchg.80%29.aspx) 拡張プロパティが **true** に設定されているフォルダーを検索することによって、EWS を使用して既存のフォルダーの下のすべての隠しフォルダーを検索できます。 この検索を行うには、次の要求に示すように、[ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) 要素を検索する [IsEqualTo](https://msdn.microsoft.com/library/48e7e067-049c-4184-8026-071e6f558e8a%28Office.15%29.aspx)[Restriction](https://msdn.microsoft.com/library/77f19014-d112-4999-8e83-ecc32a117a73%28Office.15%29.aspx) を **PidTagAttributeHidden** プロパティ (**PropertyTag** 値を 4243、**PropertyType** 値を Boolean に設定) に含めます。 この例では、MsgFolderRoot (インフォメーション ストアの先頭または IPM サブツリーとも呼ばれる) が、検索する親フォルダーとして使用されます。 
  
これは、[すべての隠しフォルダーを検索](#bk_findhiddenewsma)するのに **FindFolders** メソッドを使用する際に、EWS マネージ API が送信する XML 要求でもあります。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
    <t:TimeZoneContext>
      <t:TimeZoneDefinition Id="Central Standard Time" />
    </t:TimeZoneContext>
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Deep">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
          <t:FieldURI FieldURI="folder:DisplayName" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="100"
                               Offset="0"
                               BasePoint="Beginning" />
      <m:Restriction>
        <t:IsEqualTo>
          <t:ExtendedFieldURI PropertyTag="4340"
                              PropertyType="Boolean" />
          <t:FieldURIOrConstant>
            <t:Constant Value="true" />
          </t:FieldURIOrConstant>
        </t:IsEqualTo>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="msgfolderroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

サーバーは、**FindFolder** 要求に [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) メッセージで応答します。このメッセージには、メッセージのルート フォルダーの下のすべての隠しフォルダーを含むフォルダー検索が正常に行われたことを示す、**NoError** の [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素の値が含まれます。
  
[FolderId](https://msdn.microsoft.com/library/00d14e3e-4365-4f21-8f88-eaeea73b9bf7%28Office.15%29.aspx) 値は読みやすさのために短くしてあります。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="898"
                         MinorBuildNumber="23"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="6"
                        TotalItemsInView="6"
                        IncludesLastItemInRange="true">
            <t:Folders>
              <t:ContactsFolder>
                <t:FolderId Id="IBHgAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACz" />
                <t:DisplayName>{06967759-274D-40B2-A3EB-D7F9E73727D7}</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBHwAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAAC7" />
                <t:DisplayName>{A9E2BC46-B3A0-4243-B315-60D991004455}</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBIQAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAADO" />
                <t:DisplayName>GAL Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:ContactsFolder>
                <t:FolderId Id="IBHQAAAA=="
                            ChangeKey="AwAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACa" />
                <t:DisplayName>Recipient Cache</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="HAAAAA=="
                            ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAAAACS" />
                <t:DisplayName>Conversation Action Settings</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
              <t:Folder>
                <t:FolderId Id="IQywAAAA=="
                            ChangeKey="AQAAABYAAAD32nSTjepyT63rYH17n9THAAAeZIBf" />
                <t:DisplayName>TestFolder</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x10f4"
                                      PropertyType="Boolean" />
                  <t:Value>true</t:Value>
                </t:ExtendedProperty>
              </t:Folder>
            </t:Folders>
          </m:RootFolder>
        </m:FindFolderResponseMessage>
      </m:ResponseMessages>
    </m:FindFolderResponse>
  </s:Body>
</s:Envelope>
```

## 
<a name="bk_findhiddenews"> </a>

フォルダーを非表示または再表示したら、フォルダー階層を取得するか、[フォルダー階層を同期させる](how-to-synchronize-folders-by-using-ews-in-exchange.md)ことをお勧めします。[EWS マネージ API を使用してフォルダー階層を取得する](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyewsma)方法または [EWS を使用してフォルダー階層を取得する](how-to-work-with-folders-by-using-ews-in-exchange.md#bk_getfolderhierarchyews)方法を示す例は、階層内のどのフォルダーが非表示にされているかも示します。 
  
## <a name="see-also"></a>関連項目


- [Exchange の EWS のフォルダーとアイテム](folders-and-items-in-ews-in-exchange.md)
    
- [Exchange で EWS を使用してフォルダーを操作する](how-to-work-with-folders-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用して検索フォルダーを操作する](how-to-work-with-search-folders-by-using-ews-in-exchange.md)
    

