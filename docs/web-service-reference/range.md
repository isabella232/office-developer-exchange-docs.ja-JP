---
title: 範囲
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ee2891e4-3aa6-4258-9727-1f2ee9622508
description: Range 要素は、繰り返し予定表アイテムの予定表アイテムの出現範囲を指定します。
ms.openlocfilehash: 0d16dad24dda48f084b3011d7b96eb719431d9da
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519101"
---
# <a name="range"></a>範囲

**Range 要素** は、繰り返し予定表アイテムの予定表アイテムの出現範囲を指定します。 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 **OccurrencesRangeType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Start** <br/> |Start 属性のテキスト **値** は、定期的なアイテム範囲の開始日です。 これは **dateTime 値** です。  <br/> |
|**End** <br/> |End 属性のテキスト **値** は、定期的なアイテム範囲の終了日です。 これは **dateTime 値** です。  <br/> |
|**Count** <br/> |Count 属性のテキスト **値** は、定期的なアイテムの出現回数です。 これは整数 **値** です。  <br/> |
|**CompareOriginalStartTime** <br/> |**CompareOriginalStartTime** 属性のテキスト値 **が true** の場合、クライアントは元の開始時刻と新しい開始時刻を比較する必要があります。 false の **値は** 、クライアントが元の開始時刻と新しい開始時刻を比較する必要が生じない場合を示します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[Ranges](ranges.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> ||
   

