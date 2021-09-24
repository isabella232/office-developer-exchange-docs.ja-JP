---
title: ApplyConversationAction 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- ApplyConversationAction
api_type:
- schema
ms.assetid: 73d7943d-d361-4f8b-9948-d85f886efa1a
description: ApplyConversationAction 操作は、会話内のすべてのアイテムに対して 1 回またはフォローアップアクションを設定します。 ApplyConversationAction 操作を使用すると、会話内のすべてのアイテムの読み取り状態を分類、移動、コピー、削除、および設定できます。 会話内の新しいメッセージに対してアクションを設定することもできます。
ms.openlocfilehash: ed3ed02dc045a095bcc86124b8d3e1c5a65dae84
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520102"
---
# <a name="applyconversationaction-operation"></a>ApplyConversationAction 操作

**ApplyConversationAction** 操作は、会話内のすべてのアイテムに対して 1 回またはフォローアップアクションを設定します。 **ApplyConversationAction** 操作を使用すると、会話内のすべてのアイテムの読み取り状態を分類、移動、コピー、削除、および設定できます。 会話内の新しいメッセージに対してアクションを設定することもできます。 
  
## <a name="applyconversationaction-request-example"></a>ApplyConversationAction 要求の例

### <a name="description"></a>説明

**ApplyConversationAction 要求** の次の例は、指定された会話内のアイテムを別のフォルダーに移動する方法を示しています。 スレッドに追加されたアイテムも、指定したフォルダーに移動されます。 
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="remarks"></a>注釈

会話とフォルダーの識別子は、読みやすさを維持するために短縮されました。
  
## <a name="applyconversationaction-response-example"></a>ApplyConversationAction 応答の例

### <a name="description"></a>説明

次の例は **、ApplyConversationAction** 要求に対する正常な応答を示しています。 
  
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
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:ApplyConversationActionResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                       xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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
- [EWS 操作 (Exchange](ews-operations-in-exchange.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)
- [EWS での会話](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

