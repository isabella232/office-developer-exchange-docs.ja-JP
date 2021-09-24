---
title: FilterHtmlContent
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FilterHtmlContent
api_type:
- schema
ms.assetid: 2f9358a0-de1d-4544-9aa0-d9f6519f3b5f
description: FilterHtmlContent 要素は、安全でない可能性のある HTML コンテンツをアイテムまたは添付ファイルからフィルター処理するかどうかを指定します。
ms.openlocfilehash: 9400c86465db994251a00164517590268e7e4ad1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510086"
---
# <a name="filterhtmlcontent"></a>FilterHtmlContent

**FilterHtmlContent** 要素は、安全でない可能性のある HTML コンテンツをアイテムまたは添付ファイルからフィルター処理するかどうかを指定します。 
  
```xml
<FilterHtmlContent>true or false</FilterHtmlContent>
```

 **boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AttachmentShape](attachmentshape.md) <br/> | [GetAttachment](getattachment.md)要求への応答で返す追加のプロパティを識別します。  <br/><br/>  次に、この要素の XPath 式を示します。 <br/> <br/>  `/GetAttachment/AttachmentShape` <br/> |
|[ItemShape](itemshape.md) <br/> | GetItem、FindItem、または SyncFolderItems 応答に含めるアイテムのプロパティとコンテンツを識別します。  <br/> <br/> この要素の XPath 式を次に示します。 <br/> <br/>  `/GetItem/ItemShape`<br/> <br/>  `/FindItem/ItemShape`<br/> <br/>  `/SyncFolderItems/ItemShape` <br/> |
   
## <a name="text-value"></a>テキスト値

この要素には **、true** または false を **指定できます**。 既定値は **false** です。 これはブール型のデータ型です。
  
## <a name="remarks"></a>注釈

この要素は省略できます。
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Exchange Server EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

