---
title: 絞り込み条件
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8395b45f-3b94-4473-82ac-2a12c4309170
description: 絞り込み条件要素では、検索の絞り込み条件を指定します。
ms.openlocfilehash: aad1874760e02b2226cbe1a5bb700013d3816cc0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833038"
---
# <a name="refiner"></a>絞り込み条件

**絞り込み条件**要素では、検索の絞り込み条件を指定します。 
  
```XML
<Refiner>
   <Name/>
   <Value/>
   <Count/>
   <Token/>
</Refiner>
```

 **SearchRefinerItemType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[名 (文字列)](name-string.md) | [値](value.md) | [数](count.md) | [トークン (文字列)](token-string.md)
  
### <a name="parent-elements"></a>親要素

[絞り込み条件](refiners.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> ||
   

