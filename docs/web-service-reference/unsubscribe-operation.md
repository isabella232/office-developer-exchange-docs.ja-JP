---
title: 操作の購読を解除します。
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
description: 購読の取り消し操作を使用して、プル サブスクリプションの通知を終了します。 サブスクリプションのタイムアウトを通知するのではなく、この操作を使用します。 この操作の通知をプルのみです。
ms.openlocfilehash: 64514a718d473f0fd7d0320bd1ccecddb1940ac8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839821"
---
# <a name="unsubscribe-operation"></a>操作の購読を解除します。

購読の取り消し操作を使用して、プル サブスクリプションの通知を終了します。 サブスクリプションのタイムアウトを通知するのではなく、この操作を使用します。 この操作の通知をプルのみです。
  
## <a name="unsubscribe-request-example"></a>購読の取り消しの要求の例

### <a name="description"></a>説明

購読を解除するクライアントの通知サービスに送信される SOAP XML メッセージの例を次に示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
  xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <Unsubscribe xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <SubscriptionId>e6fbf5c1-7e26-4bc6-a5f2-882063d5e34e</SubscriptionId>  
    </Unsubscribe>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-request-elements"></a>要求要素の購読を解除します。

次の要素は、要求で使用されます。
  
- [購読の取り消し](unsubscribe.md)
    
- [サブスクリプション Id (GetEvents)](subscriptionid-getevents.md)
    
## <a name="successful-unsubscribe-response-example"></a>成功した購読取り消しの応答の例

### <a name="description"></a>説明

購読の取り消しの要求に正常な応答の例を次に示します。
  
### <a name="code"></a>コード

```xml
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:UnsubscribeResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:UnsubscribeResponseMessage>
      </m:ResponseMessages>
    </UnsubscribeResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="unsubscribe-response-elements"></a>応答要素の購読を解除します。

次の要素は、応答で使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [購読の取り消し](unsubscribe.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UnsubscribeResponseMessage](unsubscriberesponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
## <a name="unsubscribe-error-response-example"></a>エラー応答の例の購読を解除します。

### <a name="description"></a>説明

見つからない場合、サブスクリプションの識別子を使用して、購読を解除しようとするへの応答としての登録解除エラー応答は、次の例が発生した Exchange ストアにします。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="628" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <UnsubscribeResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="unsubscribe-error-response-elements"></a>エラー応答の要素の購読を解除します。

エラー応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [UnsubscribeResponse](unsubscriberesponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [UnsubscribeResponseMessage](unsubscriberesponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>関連項目

- [サブスクライブ操作](subscribe-operation.md)
- [GetEvents 操作](getevents-operation.md)
- [プル サブスクリプションを使用します。](http://msdn.microsoft.com/library/f956bc0e-2b25-4613-966b-54c65456897c%28Office.15%29.aspx)

