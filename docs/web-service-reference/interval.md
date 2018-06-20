---
title: Interval
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Interval
api_type:
- schema
ms.assetid: d0c97a5f-96be-40c6-b7d4-abf4c3870adf
description: 間隔の要素は、連続する 2 つの定期的なアイテムの間隔を定義します。
ms.openlocfilehash: 55d26b5b1b51aca3effa93a2e6852c1ae57ef4b0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831962"
---
# <a name="interval"></a>Interval

**間隔**の要素は、連続する 2 つの定期的なアイテムの間隔を定義します。 
  
```xml
<Interval/>
```

 **int**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AbsoluteMonthlyRecurrence](absolutemonthlyrecurrence.md) <br/> |1 か月ごと。  <br/> |
|[DailyRegeneration](dailyregeneration.md) <br/> |日後にタスクが再生成される頻度を説明します。  <br/> |
|[DailyRecurrence](dailyrecurrence.md) <br/> |頻度を日数でタスクが繰り返し発生するについて説明します。  <br/> |
|[MonthlyRegeneration](monthlyregeneration.md) <br/> |月のタスクが再生成される頻度を説明します。  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |定期的なタスクの相対的な月単位のパターンについて説明します。  <br/> |
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |週単位、およびタスクが繰り返し発生する日は、頻度について説明します。  <br/> |
|[WeeklyRegeneration](weeklyregeneration.md) <br/> |週間後、タスクが再生成される頻度を説明します。  <br/> |
|[YearlyRegeneration](yearlyregeneration.md) <br/> |年間で、タスクが再生成される頻度を説明します。  <br/> |
   
## <a name="text-value"></a>テキスト値

整数値を表す文字列値は、必要があります。
  
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

