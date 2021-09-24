---
title: IsPartiallyIndexed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 542e7b90-eafe-4711-a9d7-71bbc30d9646
description: IsPartiallyIndexed 要素は、アイテムが部分的にインデックス付けされているかどうかを示します。
ms.openlocfilehash: 3917f14bbdae13f4485edcbbcd595989c3cd907f
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540987"
---
# <a name="ispartiallyindexed"></a>IsPartiallyIndexed

**IsPartiallyIndexed** 要素は、アイテムが部分的にインデックス付けされているかどうかを示します。 
  
```XML
<IsPartiallyIndexed>true | false</IsPartiallyIndexed>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[NonIndexableItemDetail](nonindexableitemdetail.md)
  
## <a name="text-value"></a>テキスト値

**IsPartiallyIndexed** 要素のテキスト値 **が true** の場合は、メールボックス アイテムが部分的にインデックス付けされた状態を示します。 false の **値は** 、メールボックス アイテムが部分的にインデックス付けされていないかどうかを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

