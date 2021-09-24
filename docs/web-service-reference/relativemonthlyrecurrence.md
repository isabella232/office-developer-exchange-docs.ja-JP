---
title: RelativeMonthlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RelativeMonthlyRecurrence
api_type:
- schema
ms.assetid: a76595db-7460-44ac-ac2a-53241caa33a7
description: RelativeMonthlyRecurrence 要素は、相対的な毎月の定期的なパターンを表します。
ms.openlocfilehash: 326e6581e55e64ffd2bcc9bdfa5108cf63089633
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513445"
---
# <a name="relativemonthlyrecurrence"></a>RelativeMonthlyRecurrence

**RelativeMonthlyRecurrence 要素は**、相対的な毎月の定期的なパターンを表します。 
  
```xml
<RelativeMonthlyRecurrence>
   <Interval/>
   <DaysOfWeek/>
   <DayOfWeekIndex/>
</RelativeMonthlyRecurrence>
```

 **RelativeMonthlyRecurrencePatternType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[間隔](interval.md) <br/> |2 つの連続する月次定期的なパターン アイテム間の間隔を定義します。 この値の範囲は 1 ~ 99 です。  <br/> |
|[DaysOfWeek (DayOfWeekType)](daysofweek-dayofweektype.md) <br/> |相対的な月次繰り返しパターンに含める週の日数について説明します。  <br/> |
|[DayOfWeekIndex](dayofweekindex.md) <br/> |相対的な月次繰り返しパターンで使用される週について説明します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Recurrence (RecurrenceType)](recurrence-recurrencetype.md) <br/> |予定表アイテムと会議出席依頼の定期的なパターンが含まれます。  <br/> |
|[Recurrence (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |定期的なタスクの定期的な情報が含まれています。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

