---
title: IsPartiallyIndexed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 542e7b90-eafe-4711-a9d7-71bbc30d9646
description: IsPartiallyIndexed 要素は、項目が部分的にインデックスを作成するかどうかを示します。
ms.openlocfilehash: e780fac23aeec1d80e547a47b322073fecdc2a0b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832082"
---
# <a name="ispartiallyindexed"></a>IsPartiallyIndexed

**IsPartiallyIndexed**要素は、項目が部分的にインデックスを作成するかどうかを示します。 
  
```XML
<IsPartiallyIndexed>true | false</IsPartiallyIndexed>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[NonIndexableItemDetail](nonindexableitemdetail.md)
  
## <a name="text-value"></a>テキスト値

の**場合は true** 、 **IsPartiallyIndexed**要素のテキスト値は、メールボックスのアイテムのインデックスは部分的にことを示します。 **False**の値は、メールボックスのアイテムが部分的に索引付けられないことを示します。 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

