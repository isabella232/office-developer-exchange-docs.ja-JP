---
title: パブリック フォルダーのコンテンツ要求のルーティング
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 59d2f05e-90fb-471e-ac06-70becc15b295
description: パブリック フォルダーのコンテンツを含むパブリック フォルダーの情報の要求はすべて、ターゲット フォルダーのコンテンツを保持するパブリック フォルダー メールボックスにルーティングされる必要があります。そのメールボックスへの要求をルーティングするには、X-AnchorMailbox ヘッダーと X-PublicFolderMailbox ヘッダーを特定の値に設定する必要があります。
ms.openlocfilehash: 523b9c8efc65253f7970fffeb5800e451784522d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527741"
---
# <a name="route-public-folder-content-requests"></a>パブリック フォルダーのコンテンツ要求のルーティング

パブリック フォルダーのコンテンツを含むパブリック フォルダーの情報の要求はすべて、ターゲット フォルダーのコンテンツを保持するパブリック フォルダー メールボックスにルーティングされる必要があります。そのメールボックスへの要求をルーティングするには、**X-AnchorMailbox** ヘッダーと **X-PublicFolderMailbox** ヘッダーを特定の値に設定する必要があります。 
  
次の表では、このプロセスの概要を説明します。
  
**パブリック フォルダーの概要**

|ヘッダー|必要なもの|取得する方法|
|:-----|:-----|:-----|
|**X-AnchorMailbox** <br/> |1. パブリック フォルダー階層メールボックス用の [X-AnchorMailbox と X-PublicFolderInformation の値](how-to-route-public-folder-hierarchy-requests.md)。<br/><br/>2. メールボックスのコンテンツを含むパブリック フォルダー メールボックスの GUID。これは自動検出サービスに送信されます。<br/><br/>  自動検出の応答の **AutoDiscoverSMTPAddress** が **X-AnchorMailbox** ヘッダーの値になります。  <br/> ![TODO](media/Ex15_PF_PFContent.png)| 1. この記事にある、[EWS マネージ API を実装する](#bk_determineguidewsma)コード例を使用します。 または、[EWS を使用](#bk_determineguidews)し、結果を変換して GUID を取得します。<br/><br/>2. GUID とドメイン名を使用して、[自動検出を要求](#bk_makeautodrequest)します。<br/><br/>3. 自動検出の応答で返された **AutoDiscoverSMTPAddress** 要素の値を使用して、[ヘッダーの値を設定](#bk_setheadervalues)します。  <br/> |
|**X-PublicFolderMailbox** <br/> |作業は完了しています。X-PublicFolderMailbox の値は X-AnchorMailbox の値と同じです。  <br/> |既に取得済みです。  <br/> |
   
ヘッダーの値が決定したら、それらを[パブリック フォルダーのコンテンツ要求を行うときに](#bk_setheadervalues)含めます。
  
この記事の手順は、パブリック フォルダー コンテンツの要求に固有のものです。要求がパブリック フォルダー階層かコンテンツ要求かを特定するには、「[パブリック フォルダー要求のルーティング](public-folder-access-with-ews-in-exchange.md#bk_routing)」を参照してください。

<a name="bk_determineguidewsma"> </a>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してパブリック フォルダー メールボックスの GUID を特定する


パブリック フォルダーのコンテンツ メールボックスの GUID を特定するには、次の動作を実行する以下のコード例を使用します。 
  
- [パブリック フォルダー階層の要求をルーティング](how-to-route-public-folder-hierarchy-requests.md)して取得した **X-AnchorMailbox** ヘッダーと **X-PublicFolderInformation** ヘッダーを使用します。
    
- EWS マネージ API の [FindFolders](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) メソッドを呼び出して、**PR_REPLICA_LIST** (0x66980102) プロパティの要求を含めます。 
    
**PR_REPLICA_LIST** の値は、フォルダーのコンテンツを含むパブリック フォルダー メールボックスのメールボックス GUID を識別します。**PR_REPLICA_LIST** プロパティはバイト配列ですが、このシナリオでは GUID としてキャストされます。GUID とドメイン名が連結されて、自動検出を呼び出すためのアドレスが形成されます。 
  
この例では、`service` をメールボックス ユーザーの [ExchangeService](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクト、`PFHAnchorHeader` と `PFHMailboxHeader` を **X-AnchorMailbox** ヘッダーと **X-PublicFolderMailbox** ヘッダーの値、ドメインをテナントによって使用されるドメイン名とします。 
  
```cs
public static string GetMailboxGuidAddress(ExchangeService service, String PFHAnchorHeader, String PFHMailboxHeader, String domain)
{
    // Create a new folder view, and pass in the maximum number of folders to return.
    FolderView view = new FolderView(10);
    // Create an extended property definition for the PR_REPLICA_LIST property.
    ExtendedPropertyDefinition PR_REPLICA_LIST = new ExtendedPropertyDefinition(0x6698, MapiPropertyType.Binary);
    // As a best practice, limit the properties returned to only those required.
    // In this case, return the folder ID, the folder display name, and 
    // the value of the PR_REPLICA_LIST extended property definition.
    view.PropertySet = new PropertySet(BasePropertySet.IdOnly, FolderSchema.DisplayName, PR_REPLICA_LIST);
    service.HttpHeaders.Add("X-AnchorMailbox", PFHAnchorHeader);
    service.HttpHeaders.Add("X-PublicFolderMailbox", PFHMailboxHeader);
    // Add a call to the CertificateValidationCallback method here if needed.
    // ServicePointManager.ServerCertificateValidationCallback = CertificateValidationCallBack;
    // Call FindFolders to retrieve the folder hierarchy, starting with the PublicFolderRoot folder.
    // This method call results in a FindFolder call to EWS.
    FindFoldersResults findResults = service.FindFolders(WellKnownFolderName.PublicFoldersRoot, view);
    string GuidAsString = null;
    List<string> Guids = new List<string>();
    // For each folder under the root, display the name, and copy the value of the 
    // PR_REPLICA_LIST byte array to a string value. 
    foreach (Folder folder in findResults.Folders)
    {
        Console.WriteLine("Public folder display name: {0}", folder.DisplayName);
        byte[] ByteArr = (byte[])folder.ExtendedProperties[0].Value;
        GuidAsString = System.Text.Encoding.ASCII.GetString(ByteArr, 0, 36);
        Guids.Add(GuidAsString);
        Console.WriteLine("Address for Autodiscover: {0}.{1}\r\n", GuidAsString, domain);
    }
    // Concatenate the GUID value of the PR_REPLICA_LIST with the domain name to generate the 
    // SMTP address to use for the AutoDiscover request for the public folder content mailbox.
    string AutoDSMTPAddress = GuidAsString + "@" + domain;
    // Check that all folders have the same GUID value. If they do not, use the GUID value of the
    // folder that you're requesting content for.
    string commonGuid = CompareGuidsForEquality(Guids);
    if (commonGuid == "Not Equal")
    {
        Console.WriteLine("The GUIDs for all the folders in the hierarchy are not the same. Run the Autodiscover sample using the address returned above that is associated with the folder in your hierarchy request.", AutoDSMTPAddress);
        return null;
    }
    else
    {
        Console.WriteLine("The GUIDs for all public folders in the hierarchy are the same. Run the Autodiscover sample using the {0} address.", AutoDSMTPAddress);
        return AutoDSMTPAddress;
    }
}
// Method to compare the GUID for each folder under the public folder root.
// If each GUID is the same, return the GUID.
// If the GUIDs are not the same, return "Not equal".
public static string CompareGuidsForEquality(List<string> list)
{
    string NotEqual = "Not equal";
    string first = list.First();
    return list.All(x => x == first) ? first : NotEqual;
}
```

"要求が失敗しました。基になる接続が閉じられました。SSL/TLS のセキュリティで保護されているチャネルに対する信頼関係を確立できませんでした" というエラーが発生したら、[検証コールバック メソッドの呼び出しを追加](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)する必要があります。そのメソッドのプレースホルダーとコメントはコード例に含まれています。
  
メールボックスの GUID がパブリック フォルダー ルートにあるすべてのパブリック フォルダーで統一されている場合、この例は、コンソール出力で[自動検出を呼び出す](#bk_makeautodrequest)ときに使用するアドレスを戻り値として示します。 メールボックスの GUID がパブリック フォルダー ルートにあるすべてのパブリック フォルダーで統一されていない場合、コンテンツ要求のフォルダーに関連付けられているアドレスで[自動検出を要求する](#bk_makeautodrequest)必要があります。 

<a name="bk_determineguidews"> </a>

## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-ews"></a>EWS を使用してパブリック フォルダー メールボックスの GUID を特定する

次のコード例では、EWS [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) 操作を使用して **PR_REPLICA_LIST** (0x66980102) プロパティの値を取得する方法を示します。[ExtendedFieldURI](https://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx) 要素の、**PropertyTag** 属性は **PR_REPLICA_LIST** プロパティの 10 進数 (26264) に、**PropertyType** 属性は **Binary** に設定します。
  
これは、[EWS マネージ API を使用してパブリック フォルダー メールボックスの GUID を特定](#bk_determineguidewsma)するために **FindFolders** メソッドを使用するときに、EWS マネージ API が送信する XML 要求です。
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
Accept: text/xml
User-Agent: ExchangeServicesClient/15.00.0913.015
Accept-Encoding: gzip,deflate
Authorization: Basic c29ueWFmQGNvbnRvc28xMDAwLm9ubWljcm9zb2Z0LmNvbTpFWENIIzIwMTQ=
Host: outlook.office365.com
Cookie: ClientId=KZPBLKA9ZMPXAQDW
Content-Length: 1005
Expect: 100-continue
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:ExtendedFieldURI PropertyTag="26264" PropertyType="Binary" />
        </t:AdditionalProperties>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="10" Offset="0" BasePoint="Beginning" />
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="publicfoldersroot" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

サーバーは、**FindFolder** 要求に対して **PR_REPLICA_LIST** の拡張プロパティの値を含む [FindFolderResponse](https://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx) メッセージで応答します。プロパティの値は、Base-64 のエンコードされたバイト配列の文字列形式として EWS 応答に表れることに注意してください。応答内のいくつかのヘッダー値は読みやすいように短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="1019" MinorBuildNumber="15" Version="V2_17" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body>
    <m:FindFolderResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindFolderResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="2" TotalItemsInView="2" IncludesLastItemInRange="true">
            <t:Folders>
              <t:ContactsFolder>
                <t:FolderId Id="AAEuAAAAAADL8shaNEKnQYVvRbpoY9vDAQBGDloItRzyTrAt+XVzRr/YAABdofPkAAA=" ChangeKey="AwAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/2h"/>
                <t:DisplayName>My Public Contacts</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x6698" PropertyType="Binary"/>
                  <t:Value>MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==</t:Value>
                </t:ExtendedProperty>
              </t:ContactsFolder>
              <t:Folder>
                <t:FolderId Id="AQEuAAADy/LIWjRCp0GFb0W6aGPbwwEARg5aCLUc8k6wLfl1c0a/2AAAAxEAAAA=" ChangeKey="AQAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/W/"/>
                <t:DisplayName>SampleFolder</t:DisplayName>
                <t:ExtendedProperty>
                  <t:ExtendedFieldURI PropertyTag="0x6698" PropertyType="Binary"/>
                  <t:Value>MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==</t:Value>
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

XML で返された **PR_REPLICA_LIST** の値 (MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA==) を使用してメールボックス GUID を特定するには、[EWS マネージ API のコード例](#bk_determineguidewsma)で値が変換されたのと同様の形式で値を GUID に変換する必要があります。その後、GUID はドメイン名と連結されて SMTP アドレスが作成されます。このアドレスは[自動検出要求](#bk_makeautodrequest)に含まれます。
  
## <a name="make-an-autodiscover-request"></a>自動検出を要求する
<a name="bk_makeautodrequest"> </a>

`GetMailboxGuidAddress` メソッドによって返されたアドレスを使用して自動検出を呼び出します。 「[Exchange 2013: 自動検出によるユーザー設定の取得](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e)」のコード例を使用して、自動検出サービスを呼び出すことをお勧めします。これは、このコード例が自動検出プロセスを効率化するためです。 このコード例では、次の表に記載されているコマンドライン引数を使用して POX 自動検出サービスを呼び出し、メールボックスの GUID に関連付けられている [AutoDiscoverSMTPAddress](https://msdn.microsoft.com/library/office/dn750991%28v=exchg.150%29.aspx) の値を取得します。 

  
|**引数**|**説明**|
|:-----|:-----|
|emailAddress  <br/> |[パブリック フォルダー メールボックスの GUID を特定する](#bk_determineguidewsma)で、`GetMailboxGuidAddress` メソッドによって返されたアドレスです。  <br/> |
|-skipSOAP  <br/> |POX 自動検出要求が必要であることを示します。  <br/> |
|-auth authEmailAddress  <br/> |認証に使用されるメールボックス ユーザーの電子メール アドレスです。サンプルを実行すると、メールボックス ユーザーのパスワードの入力を求められます。  <br/> |
   
たとえば、コマンドライン引数は次のようになります。
  
`1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com -skipSOAP -auth sonyaf@contoso.com`

ここで、`1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com` は **GetMailboxGuidAddress** メソッドによって返されたアドレスで、`sonyaf@contoso.com` はメールボックス ユーザーです。 
  
**Exchange 2013: Get user settings with Autodiscover** のサンプルを実行すると、最後の自動検出応答は成功し、メールボックス GUID に関連付けられているすべてのユーザー設定が含まれます。次の手順で使用するので、ローカルに **AutoDiscoverSMTPAddress** ユーザー設定を保存します。 
  
または、**Exchange 2013: Get user settings with Autodiscover** のサンプルを使用しない場合は、[自動検出エンドポイントの一覧を生成](how-to-generate-a-list-of-autodiscover-endpoints.md)することによって **AutoDiscoverSMTPAddress** ユーザー設定を取得してから、正常な応答を受信するまで次の POX 自動検出要求をそれぞれの URL に送信します。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</EMailAddress>
    <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

自動検出プロセスの詳細については、「[Exchange の自動検出](autodiscover-for-exchange.md)」、「[自動検出エンドポイントの一覧を生成する](how-to-generate-a-list-of-autodiscover-endpoints.md)」、および「[自動検出を使用して Exchange からユーザー設定を取得する](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)」を参照してください。
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a>X-AnchorMailbox ヘッダーと X-PublicFolderMailbox ヘッダーの値を設定する
<a name="bk_setheadervalues"> </a>

[自動検出要求を作成する](#bk_makeautodrequest)で取得した **AutoDiscoverSMTPAddress** の値を使用して、パブリック フォルダー コンテンツ要求に **X-AnchorMailbox** ヘッダーと **X-PublicFolderMailbox** ヘッダーの値を設定します。 
  
たとえば、NewPublicFolder@contoso.com の AutoDiscoverSMTPAddress が指定されている場合は、以下のメソッドまたは操作の呼び出し時に、次のヘッダーを含めます。
  
`X-AnchorMailbox: NewPublicFolder@contoso.com`<br/>
`X-PublicFolderMailbox: NewPublicFolder@contoso.com`

**X-AncorMailbox ヘッダーと X-PublicFolder ヘッダーが必要なパブリック フォルダー呼び出し**

|**EWS マネージ API メソッド**|**EWS 操作**|
|:-----|:-----|
|[Item.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Item.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [Item.Copy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [Item.Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [Item.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [Folder.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [Folder.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[CreateItem](https://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [GetItem](https://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [CopyItem](https://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [MoveItem](https://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |
   
EWS マネージ API を使用してこれらのヘッダーを追加するには、[HttpHeaders.Add](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) メソッドを使用します。 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "NewPublicFolder@contoso.com");
service.HttpHeaders.Add("X-PublicFolderMailbox", "NewPublicFolder@contoso.com");
```

次のコードは、**X-AnchorMailbox** ヘッダーと **X-PublicFolderMailbox** ヘッダーがこの記事の例で取得した値に設定されている [GetFolder](https://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) 要求を示します。 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
User-Agent: SoapSender1.0
X-AnchorMailbox: NewPublicFolder@contoso.com
X-PublicFolderMailbox: NewPublicFolder@contoso.com
Authorization: Basic c29ueWFmQGNvbnRvc28xMDAwLm9ubWljcm9zb2Z0LmNvbTpFWENIIzIwMTQ=
Host: outlook.office365.com
Content-Length: 688
Expect: 100-continue
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:GetFolder>
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:FolderIds>
        <t:DistinguishedFolderId Id="publicfoldersroot" />
      </m:FolderIds>
    </m:GetFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目

- [Exchange での EWS を使用したパブリック フォルダー アクセス](public-folder-access-with-ews-in-exchange.md)    
- [Exchange の自動検出](autodiscover-for-exchange.md)    
- [自動検出エンドポイントの一覧を生成する](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [自動検出を使用して Exchange からユーザー設定を取得する](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
  