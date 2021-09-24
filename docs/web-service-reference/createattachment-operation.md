---
title: CreateAttachment 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CreateAttachment
api_type:
- schema
ms.assetid: e066db95-6963-4507-a8d0-8efad287f550
description: CreateAttachment 操作は、アイテムまたはファイルの添付ファイルを作成し、指定したアイテムに添付します。
ms.openlocfilehash: 0c75e8c73bf4352e2703a6ca6ac06e261e8f37c9
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511882"
---
# <a name="createattachment-operation"></a>CreateAttachment 操作

CreateAttachment 操作は、アイテムまたはファイルの添付ファイルを作成し、指定したアイテムに添付します。
  
## <a name="file-createattachment-request-example"></a>File CreateAttachment 要求の例

### <a name="description"></a>説明

CreateAttachment 要求の次の例は、添付ファイルを作成する方法を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
<soap:Body>
  <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
    <ParentItemId Id="AAAtAE..." ChangeKey="CQAAABYA..."/>
    <Attachments>
      <t:FileAttachment>
        <t:Name>SomeFile</t:Name>
        <t:Content>AQIDBAU=</t:Content>
      </t:FileAttachment>
    </Attachments>
  </CreateAttachment>
</soap:Body>
</soap:Envelope>
```

### <a name="comment"></a>コメント

添付ファイルの名前を指定する必要があります。
  
> [!NOTE]
> 親アイテム識別子と変更キーは、読みやすさを維持するために短縮されました。 
  
### <a name="request-elements"></a>要求要素

要求では、次の要素が使用されます。
  
- [CreateAttachment](createattachment.md)
    
- [ParentItemId](parentitemid.md)
    
- [添付ファイル](attachments-ex15websvcsotherref.md)
    
- [FileAttachment](fileattachment.md)
    
- [Name (AttachmentType)](name-attachmenttype.md)
    
- [コンテンツ](content.md)
    
## <a name="successful-file-createattachment-response-example"></a>正常なファイルの CreateAttachment 応答の例

### <a name="description"></a>説明

次の例は、CreateAttachment 要求に対する正常な応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="AAAtAE=" RootItemId="AAAtAEFk=" RootItemChangeKey="CQAAAB"/>
            </t:FileAttachment>
          </m:Attachments>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a>コメント

応答には、添付ファイルの識別子が含まれる。 また、ルート アイテムの識別子と変更キーも含まれる。 アイテム識別子と変更キーは、読みやすさを維持するために短縮されました。
  
### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateAttachmentResponse](createattachmentresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateAttachmentResponseMessage](createattachmentresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [添付ファイル](attachments-ex15websvcsotherref.md)
    
- [FileAttachment](fileattachment.md)
    
- [AttachmentId](attachmentid.md)
    
## <a name="item-createattachment-request-example"></a>Item CreateAttachment 要求の例

### <a name="description"></a>説明

CreateAttachment 要求の次の例は、アイテム添付ファイルを作成する方法を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <CreateAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <ParentItemId Id="AAAtAE=" ChangeKey="CQAAABYA"/>
      <Attachments>
        <t:ItemAttachment>
          <t:Name>An item attachment</t:Name>
          <t:Message>
            <t:Subject>A message to attach</t:Subject>
          </t:Message>
        </t:ItemAttachment>
      </Attachments>
    </CreateAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a>コメント

添付ファイルの名前を指定する必要があります。
  
 **メモ** 親アイテム識別子と変更キーは、読みやすさを維持するために短縮されました。 
  
### <a name="request-elements"></a>要求要素

要求では、次の要素が使用されます。
  
- [CreateAttachment](createattachment.md)
    
- [ParentItemId](parentitemid.md)
    
- [添付ファイル](attachments-ex15websvcsotherref.md)
    
- [ItemAttachment](itemattachment.md)
    
- [Name (AttachmentType)](name-attachmenttype.md)
    
- [Message](message-ex15websvcsotherref.md)
    
- [[件名]](subject.md)
    
## <a name="successful-item-createattachment-response-example"></a>成功したアイテムの CreateAttachment 応答の例

### <a name="description"></a>説明

次の例は、CreateAttachment 要求に対する正常な応答を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:ItemAttachment>
              <t:AttachmentId Id="AAAtAEFk=" RootItemId="AAAtAEFkb=" RootItemChangeKey="CQAAABYA"/>
            </t:ItemAttachment>
          </m:Attachments>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comment"></a>コメント

応答には、新しい添付ファイルの識別子が含まれる。 また、ルート アイテムの識別子と変更キーも含まれる。 ルート アイテムは、添付ファイルを含むアイテムです。 アイテム識別子と変更キーは、読みやすさを維持するために短縮されました。
  
### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateAttachmentResponse](createattachmentresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateAttachmentResponseMessage](createattachmentresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [添付ファイル](attachments-ex15websvcsotherref.md)
    
- [ItemAttachment](itemattachment.md)
    
- [AttachmentId](attachmentid.md)
    
## <a name="createattachment-error-response-example"></a>CreateAttachment エラー応答の例

### <a name="description"></a>説明

次の例は、CreateAttachment 要求に対するエラー応答を示しています。 このエラーは、添付ファイルの名前が指定されていないという事実が原因です。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="8" MinorVersion="0" MajorBuildNumber="653" MinorBuildNumber="0" 
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"/>
  </soap:Header>
  <soap:Body>
    <CreateAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:CreateAttachmentResponseMessage ResponseClass="Error">
          <m:MessageText>Required property is missing.</m:MessageText>
          <m:ResponseCode>ErrorRequiredPropertyMissing</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:MessageXml>
            <t:ExceptionFieldURI FieldURI="attachment:Name"/>
          </m:MessageXml>
          <m:Attachments/>
        </m:CreateAttachmentResponseMessage>
      </m:ResponseMessages>
    </CreateAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="error-response-elements"></a>エラー応答要素

エラー応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [CreateAttachmentResponse](createattachmentresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [CreateAttachmentResponseMessage](createattachmentresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
- [MessageXml](messagexml.md)
    
- [ExceptionFieldURI](exceptionfielduri.md)
    
- [添付ファイル](attachments-ex15websvcsotherref.md)
    
## <a name="remarks"></a>注釈

1 回のラウンド トリップで複数の添付ファイルがアイテムに添付されている場合、最後の応答メッセージの RootItemChangeKey は、添付ファイルを持つアイテムの新しい変更キーを表すファイルです。
  
## <a name="see-also"></a>関連項目



[DeleteAttachment 操作](deleteattachment-operation.md)
  
[GetAttachment 操作](getattachment-operation.md)

