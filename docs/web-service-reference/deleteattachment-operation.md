---
title: DeleteAttachment 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteAttachment
api_type:
- schema
ms.assetid: 4d48e595-b98c-48e7-bbeb-cacf91d12a78
description: DeleteAttachment 操作を使用して、Exchange ストア内の既存の項目からファイルおよびアイテムの添付ファイルを削除します。
ms.openlocfilehash: 4b94bfd8d6333c1f52be8ad7d0d111ab2a0552b3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759964"
---
# <a name="deleteattachment-operation"></a>DeleteAttachment 操作

DeleteAttachment 操作を使用して、Exchange ストア内の既存の項目からファイルおよびアイテムの添付ファイルを削除します。
  
## <a name="remarks"></a>備考

この操作では、ID で 1 つまたは複数の添付ファイルを削除できます。
  
## <a name="deleteattachment-request-example"></a>DeleteAttachment 要求の例

### <a name="description"></a>説明

DeleteAttachment 要求の次の例では、アイテムの添付ファイルを削除する方法を示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <DeleteAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX"/>
      </AttachmentIds>
    </DeleteAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

添付ファイル識別子が読みやすさを保持するために小さすぎます。
  
### <a name="request-elements"></a>要素を要求します。

次の要素は、要求で使用されます。
  
- [DeleteAttachment](deleteattachment.md)
    
- [AttachmentIds](attachmentids.md)
    
- [AttachmentId](attachmentid.md)
    
## <a name="deleteattachment-response-example"></a>DeleteAttachment 応答の例

### <a name="description"></a>説明

DeleteAttachment 要求に正常な応答の例を次に示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="662" MinorBuildNumber="0" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <DeleteAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

CreateAttachment 操作では、 **RootItemId**と**RootItemChangeKey**を含む AttachmentIdType 型の要素を返します。 DeleteAttachment 要求内の識別子には、これらの属性は許可されていません。 DeleteAttachment は、これらの属性が含まれていない RequestAttachmentIdType の種類の要素を使用します。
  
DeleteAttachment の応答には、親項目の ID が含まれています。 アイテムから添付ファイルが削除されると、アイテムの変更キーが変更されます。 DeleteAttachment の応答から、新しいアイテムの変更キーを取得できます。
  
> [!NOTE]
> [RootItemId](rootitemid.md)の識別子と変更キーは、読みやすさを保持するために短縮されています。 
  
### <a name="successful-response-elements"></a>正常な応答の要素

次の要素は、応答で使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [DeleteAttachmentResponse](deleteattachmentresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [DeleteAttachmentResponseMessage](deleteattachmentresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [RootItemId](rootitemid.md)
    
## <a name="see-also"></a>関連項目

- [CreateAttachment 操作](createattachment-operation.md) 
- [GetAttachment 操作](getattachment-operation.md)

