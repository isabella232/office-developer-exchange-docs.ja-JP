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
description: AttachmentShape 要素は、GetAttachment 要求への応答で返される追加のプロパティを識別します。
ms.openlocfilehash: dc6769faa5fd28ce31b796f86c507aec54abff7a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759455"
---
# <a name="attachmentshape"></a>AttachmentShape

**AttachmentShape**要素は、 [GetAttachment](getattachment.md)要求への応答で返される追加のプロパティを識別します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[IncludeMimeContent](includemimecontent.md) <br/> |応答で、多目的インターネット メール拡張 (MIME) のコンテンツ アイテムまたは添付ファイルが返されるかどうかを指定します。 この要素はオプションです。  <br/> |
|[BodyType](bodytype.md) <br/> |応答の本文のテキストを書式設定する方法を識別します。 この要素はオプションです。  <br/> |
|[FilterHtmlContent](filterhtmlcontent.md) <br/> |添付ファイルから安全でない HTML コンテンツがフィルター処理されたかどうかを指定します。 この要素はオプションです。  <br/> |
|[AdditionalProperties](additionalproperties.md) <br/> |応答で返される追加プロパティを識別します。 この要素はオプションです。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetAttachment](getattachment.md) <br/> |Exchange ストア内のメールボックスから添付ファイルを取得する要求を定義する要素。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/GetAttachment` <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetAttachment 操作](getattachment-operation.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

