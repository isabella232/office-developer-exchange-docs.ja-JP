---
title: ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: a7034730-210d-4916-b992-dda342f890f8
description: ExtendedProperties 要素は、追加のプロパティの配列を指定します。
ms.openlocfilehash: 69099842ad25a0d4f65250b3477563537c569907
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520564"
---
# <a name="extendedproperties-nonemptyarrayofextendedpropertytype"></a>ExtendedProperties (NonEmptyArrayOfExtendedPropertyType)

**ExtendedProperties 要素** は、追加のプロパティの配列を指定します。 
  
```XML
<ExtendedProperties>
    <ExtendedProperty/>
</ExtendedProperties>
```

 **NonEmptyArrayOfExtendedPropertyType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーとアイテムの拡張 MAPI プロパティを識別します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ImGroup](imgroup.md) <br/> |インスタント メッセージング グループを表します。  <br/> |
|[SearchPreviewItem](searchpreviewitem.md) <br/> |アイテムを開かなくても、プレビュー用のメールボックス アイテムの最初の 256 文字を指定します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

