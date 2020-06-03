---
title: SendItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItem
api_type:
- schema
ms.assetid: 337b89ef-e1b7-45ed-92f3-8abe4200e4c7
description: SendItem 操作は、Exchange ストアにある電子メールメッセージを送信するために使用されます。
ms.openlocfilehash: 9136379e50723211fe5a483c7f113da4fa125fc1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530339"
---
# <a name="senditem-operation"></a>SendItem 操作

SendItem 操作は、Exchange ストアにある電子メールメッセージを送信するために使用されます。
  
## <a name="senditem-e-mail-message-request-example"></a>SendItem (電子メールメッセージ) の要求の例

### <a name="description"></a>Description

次の例は、電子メールメッセージを送信する方法を示しています。
  
### <a name="code"></a>コード

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="AAAtAEF=" ChangeKey="CQAAABY+T" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

アイテム識別子は読みやすくするために短縮されています。
  
### <a name="request-elements"></a>Request 要素

要求では、次の要素が使用されます。
  
- [SendItem](senditem.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="successful-senditem-e-mail-message-response"></a>Successful SendItem (電子メールメッセージ) 応答

### <a name="description"></a>Description

次の例は、成功した SendItem 応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SendItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </SendItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SendItemResponse](senditemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SendItemResponseMessage](senditemresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
### <a name="comments"></a>コメント

[送信済みアイテム] 識別フォルダーにコピーを保存するために SendAndSaveCopy オプションが設定されているプリンシパルの [下書き] フォルダーにある電子メールメッセージを送信しようとする代理人は、送信済みアイテムのコピーを送信済みアイテムの識別フォルダーに移動することを黙って失敗します。 アイテムはプリンシパルの [下書き] フォルダーに残ります。 この問題の回避策は、プリンシパルのメールボックスを[DistinguishedFolderId](distinguishedfolderid.md)要素で指定することです。 
  
代理人が電子メールメッセージを作成して、代理人のメールボックスの [下書き] フォルダーに保存する場合に考慮すべきもう1つのシナリオがあります。 代理人がアイテムを送信し、プリンシパルの送信済みアイテムの識別フォルダーにコピーを保存しようとすると、メッセージは正常に送信され、下書きメッセージは代理人の下書きフォルダーに残り、送信されたメッセージは代理人またはプリンシパルの [送信済みアイテム] フォルダーに表示されず、応答は成功します。
  
## <a name="invalid-senditem-e-mail-message-request-example"></a>無効な SendItem (電子メールメッセージ) 要求の例

### <a name="description"></a>Description

次のコードサンプルは、無効な識別子を持つ要求の例を示しています。
  
### <a name="code"></a>コード

```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <SendItem xmlns="https://schemas.microsoft.com/exchange/services/2006/messages" 
              SaveItemToFolder="true">
      <ItemIds>
        <t:ItemId Id="%BadItemId%" ChangeKey="CQAAABYAAA" />
      </ItemIds>
    </SendItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="senditem-e-mail-message-error-response"></a>SendItem (電子メールメッセージ) エラー応答

### <a name="description"></a>Description

次の例は、無効な識別子を含む SendItem 要求へのエラー応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="602" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <SendItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Error">
          <m:MessageText>Id is malformed.</m:MessageText>
          <m:ResponseCode>ErrorInvalidIdMalformed</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </SendItemResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>エラー応答要素

エラー応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [SendItemResponse](senditemresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [SendItemResponseMessage](senditemresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>関連項目



[SendItem 操作](senditem-operation.md)
  
 **SendItemType**


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

