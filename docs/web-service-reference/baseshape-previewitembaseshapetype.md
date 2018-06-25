---
title: BaseShape (PreviewItemBaseShapeType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b9e2fdd-5678-4178-9297-7f12a3ca9d64
description: BaseShape の要素は、返される少数のプロパティで返されるすべてのプロパティの既定のプレビューまたはコンパクトなプレビューのいずれかを指定します。
ms.openlocfilehash: 1f060ae9adf52cc2916a634e3d954e3fc0903941
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759491"
---
# <a name="baseshape-previewitembaseshapetype"></a>BaseShape (PreviewItemBaseShapeType)

**BaseShape**の要素は、返される少数のプロパティで返されるすべてのプロパティの既定のプレビューまたはコンパクトなプレビューのいずれかを指定します。 
  
```XML
<BaseShape> Default | Compact</BaseShape>
```

 **PreviewItemBaseShapeType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[PreviewItemResponseShape](previewitemresponseshape.md) <br/> |応答の図形が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

**BaseShape の要素のテキスト値**

|**値**|**説明**|
|:-----|:-----|
|Default  <br/> |すべてのプロパティが表示されていることを示します。  <br/> |
|コンパクト  <br/> |選択したプロパティのみが表示されていることを示します。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型のスキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にすることができます。  <br/> ||
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

