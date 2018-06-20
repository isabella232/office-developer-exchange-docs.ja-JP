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
description: GetAttachment 操作を使用して、Exchange ストア内の項目に既存の添付ファイルを取得します。
ms.openlocfilehash: c260033208bf49c60463c09041d8ffcc52a8f5c2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760643"
---
# <a name="getattachment-operation"></a>GetAttachment 操作

GetAttachment 操作を使用して、Exchange ストア内の項目に既存の添付ファイルを取得します。
  
## <a name="getattachment-request-example"></a>GetAttachment 要求の例

### <a name="description"></a>説明

GetAttachment 要求の次の使用例は、添付ファイルを取得する方法を示します。
  
### <a name="code"></a>コード

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
xmlns:xsd="http://www.w3.org/2001/XMLSchema"
xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <GetAttachment xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <AttachmentShape/>
      <AttachmentIds>
        <t:AttachmentId Id="AAAtAEFkbWluaX..."/>
      </AttachmentIds>
    </GetAttachment>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a>コメント

[AttachmentShape](attachmentshape.md)要素を使用する添付ファイルの情報が返される必要がありますを指定することができます。 空の[AttachmentShape](attachmentshape.md)要素は有効であり、テキスト本文の種類、し、追加のプロパティを使用しない項目の添付ファイルの MIME コンテンツのない添付ファイルを表示します。 
  
[AttachmentIds](attachmentids.md)コレクションを取得する 1 つまたは複数の添付ファイルの識別子を指定できます。 **GetAttachment**に渡す前に RequestAttachmentIdType、 **CreateAttachment**から受信するすべての AttachmentIds、 **RootItemId**および**RootItemChangeKey**属性が必要であるためにの削除の種類は、これらに注意してください。
  
> [!NOTE]
> 添付ファイルの識別子と変更キーは、読みやすさを保持するために短縮されています。 
  
### <a name="request-elements"></a>要素を要求します。

次の要素は、要求で使用されます。
  
- [GetAttachment](getattachment.md)
    
- [AttachmentShape](attachmentshape.md)
    
- [AttachmentIds](attachmentids.md)
    
- [AttachmentId (GetAttachment と DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
## <a name="getattachment-response-example"></a>GetAttachment 応答の例

### <a name="description"></a>説明

GetAttachment 要求に正常な応答の例を次に示します。 この例では、添付ファイルを返します。
  
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
    <GetAttachmentResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                           xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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

GetAttachment の応答メッセージは常に、すべて添付ファイルを含みます。すべてのプロパティ常に含まれます。 ファイルの添付ファイルのこれらのプロパティは、[名前 (AttachmentType)](name-attachmenttype.md)、[コンテンツ タイプ](contenttype.md)、 [ContentId](contentid.md)、 [ContentLocation](contentlocation.md)、および[コンテンツ](content.md)です。 項目の添付ファイルのこれらのプロパティは[(AttachmentType) の名前](name-attachmenttype.md)、[コンテンツ タイプ](contenttype.md)、 [ContentId](contentid.md)、 [ContentLocation](contentlocation.md)すべてのアイテムのプロパティでは、 **AllProperties**の図形が使われていた場合と同様、GetItem の呼び出しで。 [AttachmentShape](attachmentshape.md)要素では、存在する場合、項目の添付ファイルの拡張プロパティの追加を要求するコンシューマー アプリケーションできます。 
  
### <a name="successful-response-elements"></a>正常な応答の要素

次の要素は、応答で使用されます。
  
- [ServerVersionInfo](serverversioninfo.md)
    
- [GetAttachmentResponse](getattachmentresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [GetAttachmentResponseMessage](getattachmentresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [添付ファイル](attachments-ex15websvcsotherref.md)
    
- [FileAttachment](fileattachment.md)
    
- [AttachmentId (GetAttachment と DeleteAttachment)](attachmentid-getattachment-and-deleteattachment.md)
    
- [名 (AttachmentType)](name-attachmenttype.md)
    
- [コンテンツ](content.md)
    
## <a name="see-also"></a>関連項目



[CreateAttachment 操作](createattachment-operation.md)
  
[DeleteAttachment 操作](deleteattachment-operation.md)

