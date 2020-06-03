---
title: GetAttachment 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 24d10a15-b942-415e-9024-a6375708f326
description: GetAttachment 操作は、Exchange ストア内のアイテムの既存の添付ファイルを取得するために使用されます。
ms.openlocfilehash: ac7eafd61c62b077a8d20e5fd8d004924bf06cf1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461290"
---
# <a name="getattachment-operation"></a>GetAttachment 操作

GetAttachment 操作は、Exchange ストア内のアイテムの既存の添付ファイルを取得するために使用されます。
  
## <a name="getattachment-request-example"></a>GetAttachment 要求の例

### <a name="description"></a>Description

次の GetAttachment 要求の例は、添付ファイルを取得する方法を示しています。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

[Attachmentshape](attachmentshape.md)要素を使用すると、どの添付ファイル情報を返すかを指定できます。 空の[Attachmentshape](attachmentshape.md)要素は有効であり、アイテムの添付ファイルの MIME コンテンツのない添付ファイル、テキストの本文の種類、および追加のプロパティを持たない添付ファイルをレンダリングします。 
  
[AttachmentIds](attachmentids.md)コレクションを使用すると、返される1つ以上の添付ファイル識別子を指定できます。 これらの型は RequestAttachmentIdType であることに注意してください。 **createattachment**から受け取る AttachmentIds は、 **RootItemId**属性と**RootItemChangeKey**属性を削除してから、 **getattachment**に渡す必要があります。
  
> [!NOTE]
> 読みやすくするために、添付ファイル識別子と変更キーが短縮されています。 
  
### <a name="request-elements"></a>Request 要素

要求では、次の要素が使用されます。
  
- [GetAttachment](getattachment.md)
    
- [AttachmentShape](attachmentshape.md)
    
- [AttachmentIds](attachmentids.md)
    
- [AttachmentId (GetAttachment と DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a>GetAttachment 応答の例

### <a name="description"></a>Description

次の例は、GetAttachment 要求に対する正常な応答を示しています。 次の使用例は、添付ファイルを取得します。
  
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
    <GetAttachmentResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetAttachmentResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Attachments>
            <t:FileAttachment>
              <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
              <t:Name>SomeFile</t:Name>
              <t:Content>AQIDBAU=</t:Content>
            </t:FileAttachment>
          </m:Attachments>
        </m:GetAttachmentResponseMessage>
      </m:ResponseMessages>
    </GetAttachmentResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

GetAttachment の応答メッセージには常に、完全な添付ファイルが含まれます。つまり、すべてのプロパティが常に含まれます。 添付ファイルの場合、これらのプロパティは[Name (AttachmentType)](name-attachmenttype.md)、 [ContentType](contenttype.md)、 [ContentId](contentid.md)、 [contentlocation](contentlocation.md)、および[Content](content.md)です。 アイテムの添付ファイルの場合、これらのプロパティは、GetItem 呼び出しで**allproperties**図形が使用されている場合と同様に、 [Name (attachmenttype)](name-attachmenttype.md)、 [ContentType](contenttype.md)、 [ContentId](contentid.md)、 [contentlocation](contentlocation.md) 、およびすべてのアイテムのプロパティに該当します。 [Attachmentshape](attachmentshape.md)要素が存在する場合、コンシューマーアプリケーションは、アイテムの添付ファイルに追加の拡張プロパティを要求できます。 
  
### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetAttachmentResponse](getattachmentresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetAttachmentResponseMessage](getattachmentresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [Attachments](attachments-ex15websvcsotherref.md)
    
- [FileAttachment](fileattachment.md)
    
- [AttachmentId (GetAttachment と DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
- [Name (AttachmentType)](name-attachmenttype.md)
    
- [Content](content.md)
    
## <a name="see-also"></a>関連項目



[CreateAttachment 操作](createattachment-operation.md)
  
[DeleteAttachment 操作](deleteattachment-operation.md)

