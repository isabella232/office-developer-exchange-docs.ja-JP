---
title: AttachmentShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AttachmentShape
api_type:
- schema
ms.assetid: 734914b5-3a16-4744-90a5-741fd30c4676
description: AttachmentShape 要素は、GetAttachment 要求への応答で返す追加のプロパティを識別します。
ms.openlocfilehash: 2c7ceb25f481ec07577117e46e26537e657e18c7
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520039"
---
# <a name="attachmentshape"></a>AttachmentShape

**AttachmentShape 要素は**[、GetAttachment](getattachment.md)要求への応答で返す追加のプロパティを識別します。 
  
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
|[IncludeMimeContent](includemimecontent.md) <br/> |アイテムまたは添付ファイルの多目的インターネット メール拡張機能 (MIME) コンテンツを応答で返すかどうかを指定します。 この要素は省略できます。  <br/> |
|[BodyType](bodytype.md) <br/> |本文テキストが応答で書式設定される方法を識別します。 この要素は省略できます。  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |安全でない可能性のある HTML コンテンツを添付ファイルからフィルター処理するかどうかを指定します。 この要素は省略できます。  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |応答で返す追加のプロパティを識別します。 この要素は省略できます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetAttachment](getattachment.md) <br/> |メールボックス ストア内のメールボックスから添付ファイルを取得する要求を定義するExchange。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetAttachment 操作](getattachment-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

