---
title: Exchange EWS を使用してサービスの構成情報を取得します。
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 9379740a-96e1-490d-a229-0f9937c548d2
description: Exchange の EWS から UM、ポリシー微調整、メールのヒント、保護ルールのサービス構成情報を取得する方法を紹介します。
ms.openlocfilehash: e84a563bb094a2fe03e08f8e1a81b2b054d45850
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758951"
---
# <a name="get-service-configuration-information-by-using-ews-in-exchange"></a>Exchange EWS を使用してサービスの構成情報を取得します。

Exchange の EWS から UM、ポリシー微調整、メールのヒント、保護ルールのサービス構成情報を取得する方法を紹介します。
  
EWS アプリケーションは、ユニファイド メッセージング (UM)、ポリシー微調整を行うとき、メールのヒント、または保護のルールで動作しますか。 場合は、アプリケーションが必要なサービスの構成情報を取得するのには[GetServiceConfiguration の操作](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx)を呼び出す必要があります。 **GetServiceConfiguration**操作では、EWS のこれらの機能のそれぞれに固有の構成情報を返します。 
  
> [!NOTE]
> EWS マネージ API はこの機能を実装していません。 
  
**表 1 です。GetServiceConfiguration 操作によって返される構成情報**

|EWS の機能|GetServiceConfiguration 操作によって返されるもの|
|:-----|:-----|
|UM  <br/> | <ul><li>UM が有効かどうかを示す値。</li><li>電話での再生が有効かどうかを示す値。</li><li>電話での再生のダイヤル文字列。</li></ul> |
|ポリシー微調整  <br/> | <ul><li>クライアントでの表示用のポリシー微調整。</li></ul> |
|メールのヒント  <br/> | <ul><li>メールのヒントが有効かどうかを示す値。</li><li>要求あたりの最大受信者数。</li><li>最大メッセージ サイズ。</li><li>多数の対象ユーザーのしきい値。</li><li>外部の受信者数を表示するかどうかを示す値。</li><li>内部ドメインの一覧。</li><li>ポリシーのヒントが有効かどうかを示す値。</li><li>メールの受信者数が多数であると見なされるかどうかの、対象ユーザー数の最大しきい値。  </li></ul>|
|保護ルール  <br/> | <ul><li>クライアントにセットアップされた保護ルール。</li><li>組織内部のドメインの一覧。  </li></ul> |
   
## <a name="code-example-get-service-configuration-information-for-mail-tips-by-using-ews"></a>コード例:EWS を使用して、メールのヒントのサービス構成情報を取得する

次のコード例では、メールのヒントについてはサービスの構成情報を要求する[GetServiceConfiguration の操作](http://msdn.microsoft.com/library/070cbfe5-325a-4955-8e4a-8230ea0459a7%28Office.15%29.aspx)を使用します。 [ConfigurationName](http://msdn.microsoft.com/library/3b524a2f-9c6b-4550-9f3d-f78d176b0f7b%28Office.15%29.aspx)要素に異なる値を追加することによって、その他のサービスの構成情報を要求できます。 
  
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

サービスの構成情報を要求すると後、は、それを解析できるように、XML 応答をロードするのには、 [XmlDocument クラス](http://msdn.microsoft.com/en-us/library/system.xml.xmldocument.aspx)を使用します。 そして、シナリオによっては、次のいずれかの操作を行います。 
  
- [GetMailTips 操作](http://msdn.microsoft.com/library/025483ec-a9f3-4735-8a95-d26e30ea7974%28Office.15%29.aspx)を使用すると、クライアント アプリケーションがユーザーに表示するのにためのメール ヒントを取得できます。 
    
- UM が有効な場合、携帯電話経由で[メールボックスのアイテムを再生する方法について説明](http://blogs.msdn.com/b/exchangedev/archive/2009/11/05/play-exchange-2010-mailbox-items-on-your-phone-by-using-the-ews-managed-api.aspx)をします。 
    
## <a name="see-also"></a>関連項目

- [Exchange 内の構成オプション](configuration-options-for-ews-in-exchange.md)    
- [EWS アプリケーションを設定します。](setting-up-your-ews-application.md)    
- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    

