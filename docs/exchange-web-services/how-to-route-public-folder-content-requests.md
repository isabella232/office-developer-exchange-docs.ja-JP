---
title: パブリック フォルダー コンテンツの要求をルーティングします。
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 59d2f05e-90fb-471e-ac06-70becc15b295
description: ターゲット フォルダーのコンテンツを保持するパブリック フォルダーのパブリック フォルダーのメールボックスにルーティングする必要性の内容に関連するパブリック フォルダーの情報のすべての要求。 要求をそのメールボックスに転送するには、特定の値に X AnchorMailbox X PublicFolderMailbox のヘッダーを設定する必要があります。
ms.openlocfilehash: ad36c1526a24d815ec690879d633774d429ed36c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759065"
---
# <a name="route-public-folder-content-requests"></a>パブリック フォルダー コンテンツの要求をルーティングします。

ターゲット フォルダーのコンテンツを保持するパブリック フォルダーのパブリック フォルダーのメールボックスにルーティングする必要性の内容に関連するパブリック フォルダーの情報のすべての要求。 要求をそのメールボックスに転送するには、特定の値に**X AnchorMailbox** **X PublicFolderMailbox**のヘッダーを設定する必要があります。 
  
次の表では、このプロセスの概要を説明します。
  
**パブリック フォルダーの概要**

|ヘッダー|必要なもの|取得する方法|
|:-----|:-----|:-----|
|**X AnchorMailbox** <br/> |1。 [X PublicFolderInformation の値、X AnchorMailbox](how-to-route-public-folder-hierarchy-requests.md)のパブリック フォルダー階層メールボックスです。<br/><br/>2. は自動検出サービスに送信されたメールボックスのコンテンツを格納するパブリック フォルダーのメールボックスの GUID です。<br/><br/>  Autodisover の応答で**AutoDiscoverSMTPAddress**では、 **X AnchorMailbox**のヘッダーの値になります。  <br/> ![TODO](media/Ex15_PF_PFContent.png)| 1.、 [EWS のマネージ API を実装して](#bk_determineguidewsma)、この資料のコード例を使用します。 または[EWS を使用](#bk_determineguidews)し、GUID を取得するのには、結果を変換します。<br/><br/>2。 GUID とドメイン名を使用しての[自動検出要求を作成](#bk_makeautodrequest)します。<br/><br/>3.[ヘッダーの値を設定](#bk_setheadervalues)するのには自動検出の応答で返される**AutoDiscoverSMTPAddress**の要素の値を使用します。  <br/> |
|**X PublicFolderMailbox** <br/> |作業は完了しています。X-PublicFolderMailbox の値は X-AnchorMailbox の値と同じです。  <br/> |既に取得済みです。  <br/> |
   
ヘッダーの値を確認した後は、[パブリック フォルダー コンテンツの要求を作成するとき](#bk_setheadervalues)に含めます。
  
この資料の手順は、パブリック フォルダーのコンテンツ要求に固有です。 要求は、パブリック フォルダー階層またはコンテンツの要求かどうかを確認するのには、[パブリック フォルダー要求のルーティング](public-folder-access-with-ews-in-exchange.md#bk_routing)を参照してください。
  
## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-the-ews-managed-api"></a>EWS マネージ API を使用してパブリック フォルダー メールボックスの GUID を特定する
<a name="bk_determineguidewsma"> </a>

パブリック フォルダー コンテンツ メールボックスの GUID を特定するには、次の動作を実行する以下のコード例を使用します。  
  
- [パブリック フォルダー階層構造のルーティングの要求](how-to-route-public-folder-hierarchy-requests.md)によって取得した**X AnchorMailbox**と**X PublicFolderInformation**のヘッダーを使用します。
    
- EWS のマネージ API の[FindFolders](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx)メソッドを呼び出すし、 **PR_REPLICA_LIST** (0x66980102) のプロパティが要求されています 
    
**PR_REPLICA_LIST**値は、メールボックス フォルダーの内容を持つパブリック フォルダーのメールボックスの GUID を指定します。 **PR_REPLICA_LIST**プロパティは、バイト配列が、このシナリオでは、GUID としてキャストします。 GUID とドメイン名は、自動検出を呼び出す対象となるアドレスをフォームに連結されます。 
  
この例では、 `service` 、 [ExchangeService](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)のオブジェクト、メールボックス ユーザーは、`PFHAnchorHeader`と`PFHMailboxHeader` **X AnchorMailbox**と**X PublicFolderMailbox**のヘッダーの値は、ドメインで使用するドメイン名とは、テナント。 
  
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

"要求が失敗しましたエラーが発生する場合。 基になる接続が閉じられました: SSL と TLS のセキュリティで保護されたチャネルに対する信頼関係を確立できませんでした」、[検証のコールバック メソッドへの呼び出しを追加](how-to-validate-a-server-certificate-for-the-ews-managed-api.md)する必要があります。 コードの例では、プレース ホルダーとそのメソッドのコメントが含まれます。
  
メールボックス GUID が同じパブリック フォルダーのルートの下のすべてのパブリック フォルダーの場合は、例は、[自動検出を呼び出すこと](#bk_makeautodrequest)をコンソールに出力するときと、戻り値として使用するアドレスを示します。 メールボックス GUID は、同じパブリック フォルダーのルートの下のすべてのパブリック フォルダーではありません、場合[自動検出要求を作成](#bk_makeautodrequest)するのにはコンテンツ要求内のフォルダーに関連付けられているアドレスにします。 
  
## <a name="determine-the-guid-of-the-public-folder-mailbox-by-using-ews"></a>EWS を使用してパブリック フォルダー メールボックスの GUID を特定する
<a name="bk_determineguidews"> </a>

次のコード例は、EWS [FindFolder](http://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx)操作を使用して**PR_REPLICA_LIST** (0x66980102) プロパティの値を取得する方法です。 [ExtendedFieldURI](http://msdn.microsoft.com/library/b3c6ea3a-9ead-44b9-9d99-64ecf12bde23%28Office.15%29.aspx)要素の**PropertyTag**属性は、 **PR_REPLICA_LIST**プロパティの 10 進値 (26264) に設定されてし、**バイナリ**を**登録するとき**の属性を設定します。
  
EWS のマネージ API は、 [EWS のマネージ API を使用してパブリック フォルダーのメールボックスの GUID を確認](#bk_determineguidewsma)するのには**FindFolders**メソッドを使用する場合を送信する XML 要求にもです。
  
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
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

サーバーは、 **PR_REPLICA_LIST**の拡張プロパティの値を含む[FindFolderResponse](http://msdn.microsoft.com/library/f5dd813c-9698-4a39-8fca-3a825df365ed%28Office.15%29.aspx)メッセージの**FindFolder**要求に応答します。 ベース 64 の文字列形式として EWS の応答のプロパティの値が表示されるノートには、バイト配列がエンコードされています。 読みやすさのいくつかの応答ヘッダーの値に短縮されます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="1019" MinorBuildNumber="15" Version="V2_17" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body>
    <m:FindFolderResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

XML、MWVjMmEyMzYtZWQ5My00Zjg4LWI5YzYtMzNlNjNmYTRhYTQ0AA で返される**PR_REPLICA_LIST**の値を使用するのには = =、メールボックス GUID を特定するには、値の値を変換する方法と同様の形式で GUID に変換する必要があります、[EWS のマネージ API のコード例](#bk_determineguidewsma)です。 GUID は、[自動検出要求](#bk_makeautodrequest)に含まれている SMTP アドレスを作成するドメイン名とし、連結されます。
  
## <a name="make-an-autodiscover-request"></a>自動検出要求を作成する
<a name="bk_makeautodrequest"> </a>

によって返されるアドレスを使用して、`GetMailboxGuidAddress`自動検出を呼び出すメソッドです。 使用することをお勧め、 [Exchange 2013: 自動検出でユーザー設定を取得する](http://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e)の自動検出プロセスを合理化するために自動検出サービスを呼び出すためのコード サンプルです。 このコード サンプルでは、次の表に記載されているコマンドライン引数を使用して、メールボックス GUID に関連付けられている[AutoDiscoverSMTPAddress](http://msdn.microsoft.com/en-us/library/office/dn750991%28v=exchg.150%29.aspx)の値を取得するのには POX の自動検出サービスを呼び出します。 
  
|**引数**|**説明**|
|:-----|:-----|
|emailAddress  <br/> |によって返されるアドレス、`GetMailboxGuidAddress`メソッドで[パブリック フォルダーのメールボックスの GUID を指定](http://msdn.microsoft.com/library/bk_determineguidewsma.aspx)します。  <br/> |
|-skipSOAP  <br/> |POX 自動検出要求が必要であることを示します。  <br/> |
|-auth authEmailAddress  <br/> |認証に使用されるメールボックス ユーザーの電子メール アドレスです。サンプルを実行すると、メールボックス ユーザーのパスワードの入力を求められます。  <br/> |
   
たとえば、コマンドラインの引数の場合は、次のようになります。
  
`1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com -skipSOAP -auth sonyaf@contoso.com`

`1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com` 、 **GetMailboxGuidAddress**メソッドによって返されるアドレスと`sonyaf@contoso.com`は、メールボックス ユーザーです。 
  
実行すると、 **Exchange 2013: 自動検出とユーザー設定を取得する**サンプルでは、最後の自動検出応答する必要がありますが成功してメールボックス GUID に関連付けられているすべてのユーザー設定が含まれます。 **AutoDiscoverSMTPAddress**ユーザーは、ローカルで設定を保存するとを使用する次の手順でします。 
  
またはを使用したくない場合**Exchange 2013: 自動検出とユーザー設定を取得する**サンプルでは、 **AutoDiscoverSMTPAddress**のユーザーによって[自動検出エンドポイントの一覧を生成する](how-to-generate-a-list-of-autodiscover-endpoints.md)に設定して、次に送信を取得できますPOX 正常な応答を受信するまでは、各 URL に要求を自動検出します。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="http://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</EMailAddress>
    <AcceptableResponseSchema>http://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

自動検出プロセスの詳細については、 [Exchange の自動検出](autodiscover-for-exchange.md)、[自動検出エンドポイントの一覧を生成する](how-to-generate-a-list-of-autodiscover-endpoints.md)、および[ユーザー設定の自動検出を使用して Exchange からの取得](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)を参照してください。
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a>X-AnchorMailbox ヘッダーと X-PublicFolderMailbox ヘッダーの値を設定する
<a name="bk_setheadervalues"> </a>

取得には[、自動検出要求を行う](#bk_makeautodrequest)には、 **AutoDiscoverSMTPAddress**の値を使用して、パブリック フォルダーのコンテンツ要求に**X AnchorMailbox** **X PublicFolderMailbox**のヘッダーの値を設定します。 
  
たとえば、NewPublicFolder@contoso.com の AutoDiscoverSMTPAddress が指定されている場合は、以下のメソッドの呼び出しまたは操作を行うときに、次のヘッダーを含めます。
  
`X-AnchorMailbox: NewPublicFolder@contoso.com`<br/>
`X-PublicFolderMailbox: NewPublicFolder@contoso.com`

**X AncorMailbox と X-パブリック フォルダーのヘッダーを必要とするパブリック フォルダーの呼び出し**

|**EWS マネージ API メソッド**|**EWS の操作**|
|:-----|:-----|
|[Item.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.bind%28v=exchg.80%29.aspx) <br/> [Item.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) <br/> [Item.Copy](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.copy%28v=exchg.80%29.aspx) <br/> [Item.Move](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.move%28v=exchg.80%29.aspx) <br/> [Item.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) <br/> [Folder.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) <br/> [Folder.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folder.finditems%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/78a52120-f1d0-4ed7-8748-436e554f75b6%28Office.15%29.aspx) <br/> [GetItem](http://msdn.microsoft.com/library/e3590b8b-c2a7-4dad-a014-6360197b68e4%28Office.15%29.aspx) <br/> [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> [CopyItem](http://msdn.microsoft.com/library/bcc68f9e-d511-4c29-bba6-ed535524624a%28Office.15%29.aspx) <br/> [MoveItem](http://msdn.microsoft.com/library/dcf40fa7-7796-4a5c-bf5b-7a509a18d208%28Office.15%29.aspx) <br/> [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> [GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx) <br/> [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) <br/> |
   
EWS のマネージ API を使用して、これらのヘッダーを追加するには、 [HttpHeaders.Add](http://msdn.microsoft.com/en-us/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx)メソッドを使用します。 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "NewPublicFolder@contoso.com");
service.HttpHeaders.Add("X-PublicFolderMailbox", "NewPublicFolder@contoso.com");
```

次のコードは、この資料の例で取得した値に設定し、 **X AnchorMailbox** **X PublicFolderMailbox**のヘッダーで[GetFolder](http://msdn.microsoft.com/library/355bcf93-dc71-4493-b177-622afac5fdb9%28Office.15%29.aspx)要求を示しています。 
  
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
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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
- [自動検出エンドポイントの一覧を生成します。](how-to-generate-a-list-of-autodiscover-endpoints.md)   
- [Exchange から自動検出を使用してユーザー設定を取得します。](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)
    

