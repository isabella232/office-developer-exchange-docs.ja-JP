---
title: パブリック フォルダー階層の要求をルーティングする
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: ec35df8e-4d75-4aa1-8b9c-ae1db7e05772
description: パブリック フォルダー階層についての知識を必要とするパブリック フォルダー情報に関するすべての要求 (パブリック フォルダーの移動や更新、削除、検索など) は、特定のユーザーの既定のパブリック フォルダー階層のメールボックスにルーティングする必要があります。 そのメールボックスに要求をルーティングするには、X-AnchorMailbox ヘッダーと X-PublicFolderMailbox ヘッダーの値を自動検出サービスから返される特定の値に設定する必要があります。
ms.openlocfilehash: 2773aa3ab29868c69d1fb088deb6c8a96dfb9ecc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455702"
---
# <a name="route-public-folder-hierarchy-requests"></a>パブリック フォルダー階層の要求をルーティングする

パブリック フォルダー階層についての知識を必要とするパブリック フォルダー情報に関するすべての要求 (パブリック フォルダーの移動や更新、削除、検索など) は、特定のユーザーの既定のパブリック フォルダー階層のメールボックスにルーティングする必要があります。 そのメールボックスに要求をルーティングするには、**X-AnchorMailbox** ヘッダーと **X-PublicFolderMailbox** ヘッダーの値を自動検出サービスから返される特定の値に設定する必要があります。 
  
**パブリック フォルダーの概要**

|ヘッダー|必要なもの|取得する方法|
|:-----|:-----|:-----|
|**X-AnchorMailbox** <br/> |自動検出の SOAP 応答 [GetUserSettings](https://msdn.microsoft.com/library/office/dd877096%28v=exchg.150%29.aspx) から得られる [PublicFolderInformation](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) 値。これが **X-AnchorMailbox** ヘッダーの値になります。<br/><br/> ![TODO](media/Ex15_PF_PFH_Anchor.png)| 1. ユーザーのメールボックスの SMTP アドレスで **GetUserSetting** 要求を送信します。<br/><br/>2. 自動検出サービスが返す **PublicFolderInformation** 要素の値をキャッシュします。 これは、コード内に既存の自動検出呼び出しからキャッシュすることも、新しい [EWS マネージ API の GetUserSettings 呼び出し](#bk_getpfinfoewsma)または [GetUserSettings SOAP 要求](#bk_getpfinfoews)からキャッシュすることもできます。  <br/><br/>3. **PublicFolderInformation** 要素を使用して、**X AnchorMailbox** ヘッダーの値を入力します。 **PublicFolderInformation** 要素の値は、SMTP アドレスです。  <br/> |
|**X-PublicFolderMailbox** <br/> |[POX 自動検出の応答](https://msdn.microsoft.com/library/bb204082%28v=exchg.150%29.aspx)から得られる [Server](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) 値。これが **X-PublicFolderMailbox** ヘッダーの値になります。<br/><br/> ![TODO](media/Ex15_PF_PFH_PFMailbox.png)|1. **X-AnchorMailbox** 電子メール アドレスを使用して、[POX 自動検出サービスを呼び出します](#bk_makeautodrequest)。  <br/><br/>2. 自動検出サービスから返された **Server** 要素を使用して、**X-PublicFolderMailbox** ヘッダーの値を設定します。 **X-PublicFolderMailbox** の値は、ユーザー名が GUID になる SMTP アドレスです。  <br/> |

<br/>

ヘッダーの値が決定したら、それらを[パブリック フォルダー階層の要求を行うときに](#bk_setheadervalues)含めます。
  
この記事の手順は、パブリック フォルダー階層の要求に固有のものです。要求がパブリック フォルダー階層とコンテンツのどちらの要求かを特定するには、「[パブリック フォルダー要求のルーティング](public-folder-access-with-ews-in-exchange.md#bk_routing)」を参照してください。
  
## <a name="determine-the-value-of-the-x-anchormailbox-header-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して X-AnchorMailbox ヘッダーの値を決定する
<a name="bk_getpfinfoewsma"> </a>

EWS マネージ API を使用して [PublicFolderInformation (POX)](https://msdn.microsoft.com/library/a221aa9e-b4ac-4ec5-aa42-7e2a69e8eaa6%28Office.15%29.aspx) 値を取得するには、自動検出サービスへの既存の呼び出しで返される **PublicFolderInformation** 要素の値をキャッシュするか、新しい呼び出しを行います。 
  
新しい呼び出しを行う場合は、コードに [EWS マネージ API を使用してユーザー設定を取得](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)[EWS マネージ API を使用してユーザー設定を取得](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)してから、次のコードを使用して **GetUserSettings** サンプル メソッドを呼び出します。こうすれば、**PublicFolderInformation** 要素の値だけを取得します。 入力パラメーターとして、メールボックス ユーザーの SMTP アドレスを含めます。 
  
```cs
GetUserSettingsResponse userResponse = GetUserSettings(adservice, "sonyaf@contoso.com", 3, UserSettingName.PublicFolderInformation);
Console.WriteLine("X-AnchorMailbox value for public folder hierarchy requests: {0}", userResponse.Settings[UserSettingName.PublicFolderInformation]);
```

コードを実行すると、次の情報がコンソールに表示されます。
  
`X-AnchorMailbox for public folder hierarchy requests: SharedPublicFolder@contoso.com`

この時点で **PublicFolderInformation** 値は用意できています。この値は、X-AnchorMailbox ヘッダーの値としてパブリック フォルダー階層に対する要求のすべてに含めます。 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="determine-the-value-of-the-x-anchormailbox-header-using-soap"></a>SOAP を使用して X-AnchorMailbox ヘッダーの値を決定する
<a name="bk_getpfinfoews"> </a>

次のコード例は、SOAP 操作の [GetUserSettings](https://msdn.microsoft.com/library/dd877096%28v=exchg.150%29.aspx) を使用して、**PublicFolderInformation** 値を取得する方法を示しています。 メールボックス ユーザーは [Mailbox](https://msdn.microsoft.com/library/dd877076%28v=exchg.150%29.aspx) 要素で指定されます。また、[RequestedSettings](https://msdn.microsoft.com/library/office/dd877107%28v=exchg.150%29.aspx) 要素によって応答を [PublicFolderInformation](https://msdn.microsoft.com/library/dn751006%28v=exchg.150%29.aspx) 値に制限しています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover"
               xmlns:wsa="http://www.w3.org/2005/08/addressing"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <a:RequestedServerVersion>Exchange2007_SP1</a:RequestedServerVersion>
    <wsa:Action>https://schemas.microsoft.com/exchange/2010/Autodiscover/Autodiscover/GetUserSettings</wsa:Action>
    <wsa:To>https://pod51042.outlook.com/autodiscover/autodiscover.svc</wsa:To>
  </soap:Header>
  <soap:Body>
    <a:GetUserSettingsRequestMessage xmlns:a="https://schemas.microsoft.com/exchange/2010/Autodiscover">
      <a:Request>
        <a:Users>
          <a:User>
            <a:Mailbox>sonyaf@contoso.com</a:Mailbox>
          </a:User>
        </a:Users>
        <a:RequestedSettings>
          <a:Setting>PublicFolderInformation</a:Setting>
        </a:RequestedSettings>
      </a:Request>
    </a:GetUserSettingsRequestMessage>
  </soap:Body>
</soap:Envelope>
```

応答には、**PublicFolderInformation** 値が含まれています。 
  
```XML
<UserSetting i:type="StringSetting">
    <Name>PublicFolderInformation</Name>
    <Value>SharedPublicFolder@contoso.com</Value>
</UserSetting>
```

この時点で **PublicFolderInformation** 値は用意できています。この値は、X-AnchorMailbox ヘッダーの値としてパブリック フォルダー階層に対する要求のすべてに含めます。 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com`

## <a name="make-an-autodiscover-request-to-determine-the-x-publicfolderinformation-value"></a>自動検出要求によって X-PublicFolderInformation 値を決定する
<a name="bk_makeautodrequest"> </a>

**PublicFolderInformation** SMTP アドレスを使用して自動検出要求を行います。これは、**X-AnchorMailbox** 値として使用されています。 「[Exchange 2013: Get user settings with Autodiscover](https://code.msdn.microsoft.com/exchange/Exchange-2013-Get-user-7e22c86e)」のコード サンプルを使用して、自動検出サービスを呼び出します。このコード サンプルを使用すると、自動検出プロセスが合理化されます。 このコード サンプルでは、次の表に示したコマンド ライン引数を使用して **PublicFolderInformation** SMTP アドレスの POX 自動検出サービスを呼び出しています。 
  
|**コマンド ライン引数**|**説明**|
|:-----|:-----|
|emailAddress  <br/> |**PublicFolderInformation** SMTP アドレス。  <br/> |
|-skipSOAP  <br/> | このシナリオに、POX 自動検出要求を使用します。  <br/> |
|-auth authEmailAddress  <br/> |認証に使用されるメールボックス ユーザーの電子メール アドレスです。サンプルを実行すると、メールボックス ユーザーのパスワードの入力を求められます。  <br/> |
   
たとえば、SharedPublicFolder@contoso.com が **PublicFolderInformation** 要素の SMTP アドレスで、sonyaf@contoso.com がメールボックス ユーザーのときに、コマンド ライン引数は次のようになります。 
  
`SharedPublicFolder@contoso.com -skipSOAP -auth sonyaf@contoso.com`

「**Exchange 2013: Get user settings with Autodiscover**」のサンプルを実行すると、最後の自動検出応答は成功し、メールボックス GUID に関連付けられているすべてのユーザー設定が含まれます。 EXCH [Protocol](https://msdn.microsoft.com/library/bb204278%28v=exchg.150%29.aspx)[Type](https://msdn.microsoft.com/library/office/bb204223%28v=exchg.150%29.aspx) 要素に関連付けられた [Server](https://msdn.microsoft.com/library/bb204084%28v=exchg.150%29.aspx) 値が **X-PublicFolderInformation** ヘッダー値になります。 
  
```XML
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/responseschema/2006">
  <Response xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a">
    …
    <Account>
      <AccountType>email</AccountType>
      <Action>settings</Action>
      <Protocol>
        <Type>EXCH</Type>
        <Server>1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com</Server>

```

また、「**Exchange 2013: Get user settings with Autodiscover**」のサンプルを使用しない場合は、[自動検出エンドポイントの一覧を生成](how-to-generate-a-list-of-autodiscover-endpoints.md)することによって **Server** 値を取得してから、正常な応答を受信するまで次の POX 自動検出要求をそれぞれの URL に送信します。 SharedPublicFolder@contoso.com が **X-PublicFolderMailbox** ヘッダーの値になります。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<Autodiscover xmlns="https://schemas.microsoft.com/exchange/autodiscover/outlook/requestschema/2006">
  <Request>
    <EMailAddress>SharedPublicFolder@contoso.com</EMailAddress>
    <AcceptableResponseSchema>https://schemas.microsoft.com/exchange/autodiscover/outlook/responseschema/2006a</AcceptableResponseSchema>
  </Request>
</Autodiscover>
```

自動検出プロセスの詳細については、「[Exchange の自動検出](autodiscover-for-exchange.md)」、「[自動検出エンドポイントの一覧を生成する](how-to-generate-a-list-of-autodiscover-endpoints.md)」、および「[自動検出を使用して Exchange からユーザー設定を取得する](how-to-get-user-settings-from-exchange-by-using-autodiscover.md)」を参照してください。
  
## <a name="set-the-values-of-the-x-anchormailbox-and-x-publicfoldermailbox-headers"></a>X-AnchorMailbox ヘッダーと X-PublicFolderMailbox ヘッダーの値を設定する
<a name="bk_setheadervalues"> </a>

「[EWS マネージ API を使用して X-AnchorMailbox ヘッダーの値を決定する](#bk_getpfinfoewsma)」または「[SOAP を使用して X-AnchorMailbox ヘッダーの値を決定する](#bk_getpfinfoews)」で取得した **PublicFolderInformation** SMTP アドレスの値と、「[自動検出要求によって X-PublicFolderInformation 値を決定する](#bk_makeautodrequest)」で取得した **Server** 値を使用して、パブリック フォルダー コンテンツ要求の **X-AnchorMailbox** ヘッダーと **X-PublicFolderMailbox** ヘッダーの値を設定します。 
  
たとえば、**PublicFolderInformation** SMTP アドレスが SharedPublicFolder@contoso.com で、**Server** 値が 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com だとすると、次に示すメソッドまたは操作の呼び出し時には、次に示すヘッダーを含めます。 
  
`X-AnchorMailbox: SharedPublicFolder@contoso.com` <br/>
`X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com`

**X-AnchorMailbox ヘッダーと X-PublicFolder ヘッダーが必要なパブリック フォルダーの呼び出し**

|**EWS マネージ API メソッド**|**EWS 操作**|
|:-----|:-----|
|[Folder.FindFolders](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.findfolders%28v=exchg.80%29.aspx) <br/> [Folder.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.delete%28v=exchg.80%29.aspx) <br/> [Folder.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.update%28v=exchg.80%29.aspx) <br/> [Folder.Move](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.move%28v=exchg.80%29.aspx) <br/> |[CreateFolder](https://msdn.microsoft.com/library/6f6c334c-b190-4e55-8f0a-38f2a018d1b3%28Office.15%29.aspx) <br/> [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) <br/> [DeleteFolder](https://msdn.microsoft.com/library/b0f92682-4895-4bcf-a4a1-e4c2e8403979%28Office.15%29.aspx) <br/> [UpdateFolder](https://msdn.microsoft.com/library/3494c996-b834-4813-b1ca-d99642d8b4e7%28Office.15%29.aspx) <br/> [MoveFolder](https://msdn.microsoft.com/library/c7233966-6c87-4a14-8156-b1610760176d%28Office.15%29.aspx) <br/> |
   
EWS マネージ API を使用してこれらのヘッダーを追加するには、[HttpHeaders.Add](https://msdn.microsoft.com/library/system.net.http.headers.httpheaders.add%28v=vs.118%29.aspx) メソッドを使用します。 
  
```cs
service.HttpHeaders.Add("X-AnchorMailbox", "SharedPublicFolder@contoso.com");service.HttpHeaders.Add("X-PublicFolderMailbox", "1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com");
```

たとえば、次のコードは、この記事の例で取得した値に **X-AnchorMailbox** ヘッダーと **X-PublicFolderMailbox** ヘッダーが設定されている [FindFolder](https://msdn.microsoft.com/library/7a9855aa-06cc-45ba-ad2a-645c15b7d031%28Office.15%29.aspx) 要求を示しています。 
  
```XML
POST https://outlook.office365.com/EWS/Exchange.asmx HTTP/1.1
Content-Type: text/xml; charset=utf-8
User-Agent: SoapSender1.0
X-AnchorMailbox: SharedPublicFolder@contoso.com
X-PublicFolderMailbox: 1ec2a236-ed93-4f88-b9c6-33e63fa4aa44@contoso.com
Host: outlook.office365.com
Content-Length: 1174
Expect: 100-continue
Connection: Keep-Alive
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindFolder Traversal="Shallow">
      <m:FolderShape>
        <t:BaseShape>AllProperties</t:BaseShape>
      </m:FolderShape>
      <m:IndexedPageFolderView MaxEntriesReturned="1" Offset="0" BasePoint="Beginning" />
      <m:Restriction>
        <t:IsEqualTo>
          <t:FieldURI FieldURI="folder:DisplayName" />
          <t:FieldURIOrConstant>
            <t:Constant Value="My Public Contacts" />
          </t:FieldURIOrConstant>
        </t:IsEqualTo>
      </m:Restriction>
      <m:ParentFolderIds>
        <t:FolderId Id="AQEuAAADy/LIWjRCp0GFb0W6aGPbwwEARg5aCLUc8k6wLfl1c0a/2AAAAwIAAAA=" ChangeKey="AQAAABYAAABGDloItRzyTrAt+XVzRr/YAABdo/XB" />
      </m:ParentFolderIds>
    </m:FindFolder>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a>関連項目

- [Exchange での EWS を使用したパブリック フォルダー アクセス](public-folder-access-with-ews-in-exchange.md)    
- [パブリック フォルダー コンテンツ要求のルーティング](how-to-route-public-folder-content-requests.md)    
- [EWS マネージ API を使用してユーザー設定を取得する](how-to-get-user-settings-from-exchange-by-using-autodiscover.md#bk_Managed)
    

