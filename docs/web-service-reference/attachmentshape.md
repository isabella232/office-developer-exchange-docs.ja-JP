---
title: AttachmentShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttachmentShape
api_type:
- schema
ms.assetid: 734914b5-3a16-4744-90a5-741fd30c4676
description: AttachmentShape 要素は、GetAttachment 要求に対する応答で返される追加のプロパティを識別します。
ms.openlocfilehash: e70fbaad0f649c5afdc151b777efef0f8927ba1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529666"
---
# <a name="attachmentshape"></a>AttachmentShape

**Attachmentshape**要素は、 [getattachment](getattachment.md)要求に対する応答で返される追加のプロパティを識別します。 
  
- [GetAttachment](getattachment.md)
  
- [AttachmentShape](attachmentshape.md)
  
```xml
<AttachmentShape>
   <IncludeMimeContent/>
   <BodyType/>
   <FilterHtmlContent/>
   <AdditionalProperties/>
</AttachmentShape>
```

 **AttachmentResponseShapeType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[IncludeMimeContent](includemimecontent.md) <br/> |アイテムまたは添付ファイルのマルチパーパスインターネットメール内線 (MIME) コンテンツを応答で返すかどうかを指定します。 この要素は省略できます。  <br/> |
|[BodyType](bodytype.md) <br/> |応答で本文テキストを書式設定する方法を指定します。 この要素は省略できます。  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |安全でない可能性のある HTML コンテンツを添付ファイルからフィルター処理するかどうかを指定します。 この要素は省略できます。  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |応答で返される追加のプロパティを識別します。 この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetAttachment](getattachment.md) <br/> |Exchange ストア内のメールボックスから添付ファイルを取得するための要求を定義する要素。  <br/> この要素の XPath 式を次に示します。  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetAttachment 操作](getattachment-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

