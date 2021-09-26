---
title: DeleteAttachment 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DeleteAttachment
api_type:
- schema
ms.assetid: 4d48e595-b98c-48e7-bbeb-cacf91d12a78
description: DeleteAttachment 操作は、既存のアイテムからファイルとアイテムの添付ファイルを削除するためにExchangeされます。
ms.openlocfilehash: bd08776e1f4e75204819ef5463e297e3770a34a4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546687"
---
# <a name="deleteattachment-operation"></a>DeleteAttachment 操作

DeleteAttachment 操作は、既存のアイテムからファイルとアイテムの添付ファイルを削除するためにExchangeされます。
  
## <a name="remarks"></a>注釈

この操作では、ID によって 1 つ以上の添付ファイルを削除できます。
  
## <a name="deleteattachment-request-example"></a>DeleteAttachment 要求の例

### <a name="description"></a>説明

DeleteAttachment 要求の次の例は、アイテムの添付ファイルを削除する方法を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX"/>
      </AttachmentIds>
    </DeleteAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

読みやすさを維持するために添付ファイル識別子が短縮されました。
  
### <a name="request-elements"></a>要求要素

要求では、次の要素が使用されます。
  
- [DeleteAttachment](deleteattachment.md)
    
- [AttachmentIds](attachmentids.md)
    
- [AttachmentId](attachmentid.md)
    
## <a name="deleteattachment-response-example"></a>DeleteAttachment 応答の例

### <a name="description"></a>説明

次の例は、DeleteAttachment 要求に対する正常な応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <DeleteAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:DeleteAttachmentResponseMessage xsi:type="m:DeleteAttachmentResponseMessageType" ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootItemId RootItemId="AAAtAEFkbWluaXN..." RootItemChangeKey="CQAAABYAA..."/>
        </m:DeleteAttachmentResponseMessage>
      </m:ResponseMessages>
    </DeleteAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

CreateAttachment 操作は **、RootItemId** と **RootItemChangeKey** を含む AttachmentIdType 型の要素を返します。 これらの属性は、DeleteAttachment 要求内の識別子には使用できません。 DeleteAttachment は RequestAttachmentIdType 型の要素を使用します。これらの属性は含めではありません。
  
DeleteAttachment 応答には、親アイテムの ID が含まれます。 アイテムから添付ファイルを削除すると、アイテムの変更キーが変更されます。 新しいアイテム変更キーは、DeleteAttachment 応答から取得できます。
  
> [!NOTE]
> [RootItemId 識別子と](rootitemid.md)ChangeKey は、読みやすさを維持するために短縮されました。 
  
### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [DeleteAttachmentResponse](deleteattachmentresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [RootItemId](rootitemid.md)
    
## <a name="see-also"></a>関連項目

- [CreateAttachment 操作](createattachment-operation.md) 
- [GetAttachment 操作](getattachment-operation.md)

