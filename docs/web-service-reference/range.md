---
title: Range
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ee2891e4-3aa6-4258-9727-1f2ee9622508
description: 範囲の要素は、繰り返しの予定表アイテムの予定表アイテムの出現回数の範囲を指定します。
ms.openlocfilehash: 0264c541604808b46a50e292b8ff75f205796295
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832946"
---
# <a name="range"></a>Range

**範囲**の要素は、繰り返しの予定表アイテムの予定表アイテムの出現回数の範囲を指定します。 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 **OccurrencesRangeType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Start** <br/> |**開始**属性のテキスト値は、定期的なアイテムの範囲の開始日です。 これは、 **dateTime**値です。  <br/> |
|**End** <br/> |**最終**属性のテキスト値は、定期的なアイテムの範囲の終了日です。 これは、 **dateTime**値です。  <br/> |
|**Count** <br/> |**数**の属性のテキスト値は、定期的なアイテムの数です。 これは、**整数**値です。  <br/> |
|**CompareOriginalStartTime** <br/> |**True**の**CompareOriginalStartTime**属性のテキスト値は、クライアントが新しい開始時刻を元の開始時刻を比較する必要があることを示します。 **False**の値は、クライアントが新しい開始時刻を元の開始時刻を比較する必要がないことを示します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[Ranges](ranges.md)
  
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
   

