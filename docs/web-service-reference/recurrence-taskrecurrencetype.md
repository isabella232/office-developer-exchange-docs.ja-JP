---
title: 定期的な予定 (TaskRecurrenceType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Recurrence
api_type:
- schema
ms.assetid: 99f8414a-9110-4721-a6e5-ebf225d7ed0a
description: 定期的なアイテムの要素には、定期タスクの頻度に関する情報が含まれています。
ms.openlocfilehash: ae2bb35e89a0a50c7ca67cb0e580427150afb99e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833006"
---
# <a name="recurrence-taskrecurrencetype"></a>定期的な予定 (TaskRecurrenceType)

**定期的なアイテム**の要素には、定期タスクの頻度に関する情報が含まれています。 
  
```xml
<Recurrence>
      <RelativeYearlyRecurrence/>
      <NoEndRecurrence/>
</Recurrence>
```

 **TaskRecurrenceType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |定期的なタスクの相対的な年 1 回定期的なパターンをについて説明します。  <br/> |
|[AbsoluteYearlyRecurrence](absoluteyearlyrecurrence.md) <br/> |定期的な仕事の年間の定期的なパターンを表します。  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |定期的なタスクの相対的な毎月定期的なパターンをについて説明します。  <br/> |
|[AbsoluteMonthlyRecurrence](absolutemonthlyrecurrence.md) <br/> |定期的な仕事の毎月の定期的なパターンを表します。  <br/> |
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |週、および日のタスクが繰り返し発生する頻度について説明します。  <br/> |
|[DailyRecurrence](dailyrecurrence.md) <br/> |頻度を日数でタスクが繰り返し発生するについて説明します。  <br/> |
|[DailyRegeneration](dailyregeneration.md) <br/> |次の項目の現在のタスクの完了の期限後、何日間について説明します。  <br/> |
|[WeeklyRegeneration](weeklyregeneration.md) <br/> |次の項目の現在のタスクの完了の期限後の数週間をについて説明します。  <br/> |
|[MonthlyRegeneration](monthlyregeneration.md) <br/> |次に一致する現在のタスクの完了が原因である後数か月間について説明します。  <br/> |
|[YearlyRegeneration](yearlyregeneration.md) <br/> |数年の後、次に一致する現在のタスクの完了が原因であるについて説明します。  <br/> |
|[NoEndRecurrence](noendrecurrence.md) <br/> |定義された終了日がない定期的なパターンをについて説明します。  <br/> この要素の使用は、 [EndDateRecurrence](enddaterecurrence.md)と[NumberedRecurrence](numberedrecurrence.md)の要素の使用を除外します。  <br/> |
|[EndDateRecurrence](enddaterecurrence.md) <br/> |開始日と終了日の項目の定期的なパターンについて説明します。  <br/> この要素の使用は、 [NoEndRecurrence](noendrecurrence.md)と[NumberedRecurrence](numberedrecurrence.md)の要素の使用を除外します。  <br/> 再生のパターンとは、 [EndDateRecurrence](enddaterecurrence.md)を使用できません。  <br/> |
|[NumberedRecurrence](numberedrecurrence.md) <br/> |開始日と定期的なアイテムの出現回数を説明します。  <br/> この要素の使用は、 [NoEndRecurrence](noendrecurrence.md)と[EndDateRecurrence](enddaterecurrence.md)の要素の使用を除外します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
   
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

