---
title: AbsoluteYearlyRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AbsoluteYearlyRecurrence
api_type:
- schema
ms.assetid: 96f53e2c-3893-4f6e-a78a-ac179f45c5db
description: AbsoluteYearlyRecurrence 要素は、年間の定期的なパターンを表します。
ms.openlocfilehash: 205da336a6a6ca4fd39120e83ab264e1543354e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760410"
---
# <a name="absoluteyearlyrecurrence"></a>AbsoluteYearlyRecurrence

**AbsoluteYearlyRecurrence**要素は、年間の定期的なパターンを表します。 
  
```xml
<AbsoluteYearlyRecurrence>
   <DayOfMonth/>
   <Month/>
</AbsoluteYearlyRecurrence>
```

 **AbsoluteYearlyRecurrencePatternType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[DayOfMonth](dayofmonth.md) <br/> |定期的なアイテムが発生する月の日について説明します。 このプロパティの値の範囲は、1 から 31 です。 特定の月のこの値が大きい場合、月の日数よりも、月の最後の日がこのプロパティと見なされます。  <br/> |
|[月 (定期的なアイテム)](month-item-recurrence.md) <br/> |年間の定期的なアイテムが発生する月をについて説明します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[定期的な予定 (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |定期タスクの頻度に関する情報が含まれています。  <br/> |
|[定期的なアイテム (RecurrenceType)](recurrence-recurrencetype.md) <br/> |予定表アイテムおよび会議出席依頼に定期的なパターンが含まれています。  <br/> |
   
## <a name="remarks"></a>備考

MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

