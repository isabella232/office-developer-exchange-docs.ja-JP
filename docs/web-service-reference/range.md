---
title: 範囲
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ee2891e4-3aa6-4258-9727-1f2ee9622508
description: Range 要素は、定期的な予定表アイテムの予定表アイテムの出現範囲を指定します。
ms.openlocfilehash: b5fb41709905290326b47e2662383031c34fd9c9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465311"
---
# <a name="range"></a>範囲

**Range**要素は、定期的な予定表アイテムの予定表アイテムの出現範囲を指定します。 
  
```XML
<Range Start="" End="" Count="" CompareOriginalStartTime=""/>
```

 **OccurrencesRangeType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Start** <br/> |**Start**属性のテキスト値は、定期的なアイテムの範囲の開始日です。 これは**dateTime**値です。  <br/> |
|**End** <br/> |**End**属性のテキスト値は、定期的なアイテムの範囲の終了日です。 これは**dateTime**値です。  <br/> |
|**Count** <br/> |**Count**属性のテキスト値は、定期的なアイテムの出現回数です。 これは**整数**値です。  <br/> |
|**CompareOriginalStartTime** <br/> |**Compareoriginalstarttime**属性のテキスト値が**true**になっている場合は、クライアントが元の開始時刻を新しい開始時刻と比較する必要があることを示します。 値が**false**の場合は、クライアントが元の開始時刻と新しい開始時刻を比較する必要がないことを示します。  <br/> |
   
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
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   

