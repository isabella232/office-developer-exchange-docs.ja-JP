---
title: Unsubscribe 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Unsubscribe
api_type:
- schema
ms.assetid: 994a9d2b-1501-4804-90f0-12bd914496ec
description: 登録解除操作を使用して、プル通知サブスクリプションを終了します。 サブスクリプションのタイムアウトを使用するのではなく、この操作を使用します。 この操作は、プル通知に対してのみ有効です。
ms.openlocfilehash: 054f89af1ba5c780c7de5016a6dfe34086c97f02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468027"
---
# <a name="unsubscribe-operation"></a>Unsubscribe 操作

登録解除操作を使用して、プル通知サブスクリプションを終了します。 サブスクリプションのタイムアウトを使用するのではなく、この操作を使用します。 この操作は、プル通知に対してのみ有効です。
  
## <a name="unsubscribe-request-example"></a>登録解除要求の例

### <a name="description"></a>説明

次の例は、通知サービスからクライアントの登録を解除するために送信される SOAP XML メッセージを示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Unsubscribe xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>e6fbf5c1-7e26-4bc6-a5f2-882063d5e34e</SubscriptionId>  
    </Unsubscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-request-elements"></a>登録解除の要求要素

要求では、次の要素が使用されます。
  
- [登録を解除する](unsubscribe.md)
    
- [SubscriptionId (GetEvents)](subscriptionid-getevents.md)
    
## <a name="successful-unsubscribe-response-example"></a>正常な登録解除の応答の例

### <a name="description"></a>説明

次の例は、購読中止要求に対する正常な応答を示しています。
  
### <a name="code"></a>コード

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-response-elements"></a>応答の取り消し要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [登録を解除する](unsubscribe.md)
    
- [ResponseMessages](responsemessages.md)
    
- [非表示の表示/非表示のメッセージ](unsubscriberesponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="unsubscribe-error-response-example"></a>登録解除エラーの応答の例

### <a name="description"></a>説明

次のサブスクライブ解除エラー応答の例は、Exchange ストアに配置できないサブスクリプション識別子を使用してサブスクライブを中止しようとした場合に発生します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Error">
          <m:MessageText>The specified subscription was not found.</m:MessageText>
          <m:ResponseCode>ErrorSubscriptionNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-error-response-elements"></a>登録解除エラー応答要素

エラー応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UnsubscribeResponse](unsubscriberesponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [非表示の表示/非表示のメッセージ](unsubscriberesponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>関連項目

- [サブスクライブ操作](subscribe-operation.md)
- [GetEvents 操作](getevents-operation.md)
- [プルサブスクリプションの使用](https://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

