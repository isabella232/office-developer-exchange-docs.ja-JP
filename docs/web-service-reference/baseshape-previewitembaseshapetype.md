---
title: BaseShape (PreviewItemBaseShapeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b9e2fdd-5678-4178-9297-7f12a3ca9d64
description: BaseShape 要素は、返されたすべてのプロパティを持つ既定のプレビューを指定します。または、コンパクトプレビューで返されるプロパティの数が少なくなります。
ms.openlocfilehash: 29f008840d649f97dfb299fee8e7bf5aaa573404
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527419"
---
# <a name="baseshape-previewitembaseshapetype"></a>BaseShape (PreviewItemBaseShapeType)

**Baseshape**要素は、返されたすべてのプロパティを持つ既定のプレビューを指定します。または、コンパクトプレビューで返されるプロパティの数が少なくなります。 
  
```XML
<BaseShape> Default | Compact</BaseShape>
```

 **PreviewItemBaseShapeType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[プレビュー Itemresponseshape](previewitemresponseshape.md) <br/> |応答の図形を含みます。  <br/> |
   
## <a name="text-value"></a>テキスト値

**BaseShape 要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|既定値  <br/> |すべてのプロパティが表示されることを示します。  <br/> |
|コンパクト  <br/> |選択されているプロパティのみが表示されることを示します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

