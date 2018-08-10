---
title: Exchange で EWS を使用して、サービス構成情報を取得する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9379740a-96e1-490d-a229-0f9937c548d2
description: Exchange の EWS から UM、ポリシー微調整、メールのヒント、保護ルールのサービス構成情報を取得する方法を紹介します。
ms.openlocfilehash: e84a563bb094a2fe03e08f8e1a81b2b054d45850
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758951"
---
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a>Exchange で EWS を使用して、サービス構成情報を取得する

Exchange の EWS から UM、ポリシー微調整、メールのヒント、保護ルールのサービス構成情報を取得する方法を紹介します。
  
EWS アプリケーションが、ユニファイド メッセージング (UM)、ポリシー微調整、メールのヒント、保護ルールと連携している場合、 アプリケーションは [GetServiceConfiguration 操作](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx)を呼び出して、必要なサービス構成情報を取得する必要があります。 **GetServiceConfiguration** 操作では、EWS のこれらの機能のそれぞれに固有の構成情報が返されます。 
  
> [!NOTE]
> EWS マネージ API はこの機能を実装していません。 
  
**表 1. GetServiceConfiguration 操作によって返される構成情報**

|EWS の機能|GetServiceConfiguration 操作によって返されるもの|
|:-----|:-----|
|UM  <br/> | <ul><li>UM が有効かどうかを示す値。</li><li>電話での再生が有効かどうかを示す値。</li><li>電話での再生のダイヤル文字列。</li></ul> |
|ポリシー微調整  <br/> | <ul><li>クライアントでの表示用のポリシー微調整。</li></ul> |
|メールのヒント  <br/> | <ul><li>メールのヒントが有効かどうかを示す値。</li><li>要求あたりの最大受信者数。</li><li>最大メッセージ サイズ。</li><li>多数の対象ユーザーのしきい値。</li><li>外部の受信者数を表示するかどうかを示す値。</li><li>内部ドメインの一覧。</li><li>ポリシーのヒントが有効かどうかを示す値。</li><li>メールの受信者数が多数であると見なされるかどうかの、対象ユーザー数の最大しきい値。  </li></ul>|
|保護ルール  <br/> | <ul><li>クライアントにセットアップされた保護ルール。</li><li>組織内部のドメインの一覧。  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a>コード例: EWS を使用して、メールのヒントのサービス構成情報を取得する

次のコード例では、[GetServiceConfiguration 操作](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx)を使用して、メールのヒントのサービス構成情報を要求します。 別の値の [ConfigurationName](http://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx) 要素をさらに追加して、追加のサービス構成情報を要求することができます。 
  
```cs
private static void GetServiceConfiguration(ExchangeService service, NetworkCredential creds)
{ 
  // XML for the GetServiceConfiguration request SOAP envelope for mail tips configuration information.
  const string getServiceConfigurationRequest = 
    "<?xml version=\"1.0\" encoding=\"utf-8\"?>\n" +
    "<soap:Envelope xmlns:xsi=\"http://www.w3.org/2001/XMLSchema-instance\"\n" +
    "               xmlns:m=\"http://schemas.microsoft.com/exchange/services/2006/messages\"\n" +
    "               xmlns:t=\"http://schemas.microsoft.com/exchange/services/2006/types\" \n" +
    "               xmlns:soap=\"http://schemas.xmlsoap.org/soap/envelope/\"\n" +
    "               xmlns:xs=\"http://www.w3.org/2001/XMLSchema\">\n" +
    "  <soap:Header>\n" +
    "    <t:RequestServerVersion Version=\"Exchange2013\" />\n" +
    "  </soap:Header>\n" +
    "  <soap:Body>\n" +
    "    <m:GetServiceConfiguration>\n" +
    "      <m:ActingAs>\n" +
    "        <t:EmailAddress>user1@contoso.com</t:EmailAddress>\n" +
    "        <t:RoutingType>SMTP</t:RoutingType>\n" +
    "      </m:ActingAs>\n" +
    "      <m:RequestedConfiguration>\n" +
    "        <m:ConfigurationName>MailTips</m:ConfigurationName>\n" +
    "      </m:RequestedConfiguration>\n" +
    "    </m:GetServiceConfiguration>\n" +
    "  </soap:Body>\n" +
    "</soap:Envelope>";
  // Encoded GetServiceConfiguration operation request.
  byte[] payload = System.Text.Encoding.UTF8.GetBytes(getServiceConfigurationRequest);
  try
  {
    HttpWebRequest request = (HttpWebRequest)WebRequest.Create(service.Url);
    request.AllowAutoRedirect = false;
    request.Credentials = creds;
    request.Method = "POST";
    request.ContentType = "text/xml";
    Stream requestStream = request.GetRequestStream();
    requestStream.Write(payload, 0, payload.Length);
    requestStream.Close();
    HttpWebResponse response = (HttpWebResponse)request.GetResponse();
    if (response.StatusCode == HttpStatusCode.OK)
    {
      Stream responseStream = response.GetResponseStream();
      StreamReader reader = new StreamReader(responseStream);
      string responseFromServer = reader.ReadToEnd();
      Console.WriteLine("You will need to parse this response to get the configuration information:\n\n" + responseFromServer);
      reader.Close();
      responseStream.Close();
    }
    else
      throw new WebException(response.StatusDescription);
          
  }
  catch (WebException e)
  {
    Console.WriteLine(e.Message);
  }
}

```

## <a name="next-steps"></a>次の手順

サービス構成情報の要求後、[XmlDocument クラス](http://msdn.microsoft.com/ja-JP/library/system.xml.xmldocument.aspx)を使用して応答 XML を読み込み、それを解析できるようにします。 またシナリオに応じて、次のいずれかの操作を行います。 
  
- [GetMailTips 操作](http://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx)を使用して、クライアント アプリケーションがユーザーに表示するためのメールのヒントを取得する。 
    
- 電話を介して[メールボックス アイテムを再生する方法を理解する](http://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx) (UM が有効な場合)。 
    
## <a name="see-also"></a>関連項目

- [Exchange 内の EWS の構成オプション](configuration-options-for-ews-in-exchange.md)    
- [EWS アプリケーションの設定](setting-up-your-ews-application.md)    
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    

