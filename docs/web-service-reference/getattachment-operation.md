---
title: GetAttachment 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetAttachment
api_type:
- schema
ms.assetid: 24d10a15-b942-415e-9024-a6375708f326
description: GetAttachment 操作は、ストア内のアイテムの既存の添付ファイルを取得Exchangeされます。
ms.openlocfilehash: 44a9e1988deb513039f7700e11c645c366641519
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59509938"
---
# <a name="getattachment-operation"></a>GetAttachment 操作

GetAttachment 操作は、ストア内のアイテムの既存の添付ファイルを取得Exchangeされます。
  
## <a name="getattachment-request-example"></a>GetAttachment 要求の例

### <a name="description"></a>説明

GetAttachment 要求の次の例は、添付ファイルを取得する方法を示しています。
  
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

[AttachmentShape 要素](attachmentshape.md)を使用すると、返す添付ファイル情報を指定できます。 空の [AttachmentShape](attachmentshape.md) 要素は有効であり、アイテムの添付ファイル、テキスト本文の種類、追加のプロパティがない場合は、MIME コンテンツなしで添付ファイルをレンダリングします。 
  
[AttachmentIds コレクションを使用](attachmentids.md)すると、返す 1 つ以上の添付ファイル識別子を指定できます。 これらは RequestAttachmentIdType 型なので **、CreateAttachment** から受け取る AttachmentId は **、GetAttachment** に渡す前に **RootItemId** 属性と **RootItemChangeKey** 属性を削除する必要があります。
  
> [!NOTE]
> 読みやすさを維持するために、添付ファイル識別子と変更キーが短縮されました。 
  
### <a name="request-elements"></a>要求要素

要求では、次の要素が使用されます。
  
- [GetAttachment](getattachment.md)
    
- [AttachmentShape](attachmentshape.md)
    
- [AttachmentIds](attachmentids.md)
    
- [AttachmentId (GetAttachment and DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a>GetAttachment 応答の例

### <a name="description"></a>説明

次の例は、GetAttachment 要求に対する正常な応答を示しています。 次の使用例は、添付ファイルを返します。
  
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

GetAttachment の応答メッセージには、常に完全な添付ファイルが含まれます。つまり、すべてのプロパティが常に含まれます。 添付ファイルの場合、これらのプロパティは[Name (AttachmentType)](name-attachmenttype.md) [、ContentType、ContentId、ContentLocation、](contenttype.md)[および](contentlocation.md) [Content です](content.md)。 [](contentid.md) アイテムの添付ファイルの場合、これらのプロパティは、GetItem 呼び出しで **AllProperties** 図形が使用されている場合と同様に、Name [(AttachmentType)](name-attachmenttype.md) [、ContentType](contenttype.md) [、ContentId、ContentLocation、](contentlocation.md)およびすべてのアイテムのプロパティです。 [](contentid.md) [AttachmentShape](attachmentshape.md)要素が存在する場合、コンシューマー アプリケーションはアイテム添付ファイルの追加の拡張プロパティを要求できます。 
  
### <a name="successful-response-elements"></a>成功した応答要素

応答では、次の要素が使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetAttachmentResponse](getattachmentresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetAttachmentResponseMessage](getattachmentresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [添付ファイル](attachments-ex15websvcsotherref.md)
    
- [FileAttachment](fileattachment.md)
    
- [AttachmentId (GetAttachment and DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
- [Name (AttachmentType)](name-attachmenttype.md)
    
- [コンテンツ](content.md)
    
## <a name="see-also"></a>関連項目



[CreateAttachment 操作](createattachment-operation.md)
  
[DeleteAttachment 操作](deleteattachment-operation.md)

