---
title: ApplyConversationAction 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationAction
api_type:
- schema
ms.assetid: 73d7943d-d361-4f8b-9948-d85f886efa1a
description: ApplyConversationAction 操作では、設定を 1 回だけか、会話内のすべてのアイテムで次の操作をします。 ApplyConversationAction 操作を使用すると、分類、移動、コピー、削除、および会話のすべてのアイテムの読み取り状態を設定できます。 会話で新着メッセージをアクションを設定することもできます。
ms.openlocfilehash: 2a485b84ee87aec2ed807e3f4f0901b83432fa0a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759366"
---
# <a name="applyconversationaction-operation"></a>ApplyConversationAction 操作

**ApplyConversationAction**操作では、設定を 1 回だけか、会話内のすべてのアイテムで次の操作をします。 **ApplyConversationAction**操作を使用すると、分類、移動、コピー、削除、および会話のすべてのアイテムの読み取り状態を設定できます。 会話で新着メッセージをアクションを設定することもできます。 
  
## <a name="applyconversationaction-request-example"></a>ApplyConversationAction 要求の例

### <a name="description"></a>説明

**ApplyConversationAction**要求の次の例では、指定したスレッドの別のフォルダーにアイテムを移動する方法を示します。 会話に追加される項目は、指定したフォルダーにも移動されます。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ApplyConversationAction>
      <m:ConversationActions>
        <t:ConversationAction>
          <t:Action>AlwaysMove</t:Action>
          <t:ConversationId Id="AAQkADVkNjM1EH39AWcDUGrnrnJ32hHpdc="/>
          <t:DestinationFolderId>
            <t:FolderId Id="AAMkADVkNjM1ODI3LTEwYTAtNDUBTTT6tWal35iSoKAAAABZZWAAA="/>
          </t:DestinationFolderId>
        </t:ConversationAction>
      </m:ConversationActions>
    </m:ApplyConversationAction>
  </soap:Body>
</soap:Envelope>
```

### <a name="remarks"></a>備考

会話とフォルダーの識別子は、読みやすさを保持するために短縮されています。
  
## <a name="applyconversationaction-response-example"></a>ApplyConversationAction の応答の例

### <a name="description"></a>説明

**ApplyConversationAction**要求に正常な応答の例を次に示します。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="1" 
                         MajorBuildNumber="91" 
                         MinorBuildNumber="0" 
                         Version="Exchange2010_SP1" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ApplyConversationActionResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                       xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ApplyConversationActionResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:ApplyConversationActionResponseMessage>
      </m:ResponseMessages>
    </m:ApplyConversationActionResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>関連項目

- [ApplyConversationAction 操作](applyconversationaction-operation.md)
- [Exchange での EWS の操作](ews-operations-in-exchange.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)
- [EWS での会話](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

