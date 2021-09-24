---
title: Interval
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Interval
api_type:
- schema
ms.assetid: d0c97a5f-96be-40c6-b7d4-abf4c3870adf
description: Interval 要素は、連続する 2 つの定期的なアイテム間の間隔を定義します。
ms.openlocfilehash: 6df46865d7a89a0bfde9afc5f84ffdb78d956a30
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59541029"
---
# <a name="interval"></a>Interval

**Interval 要素は**、連続する 2 つの定期的なアイテム間の間隔を定義します。 
  
```xml
<Interval/>
```

 **int**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AbsoluteMonthlyRecurrence](absolutemonthlyrecurrence.md) <br/> |1 か月ごと。  <br/> |
|[DailyRegeneration](dailyregeneration.md) <br/> |タスクが再生成される頻度を日数で示します。  <br/> |
|[DailyRecurrence](dailyrecurrence.md) <br/> |タスクが再帰する頻度を日数で示します。  <br/> |
|[MonthlyRegeneration](monthlyregeneration.md) <br/> |タスクが再生成される頻度を月数で示します。  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |定期的なタスクの相対的な月次パターンについて説明します。  <br/> |
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |タスクが再帰する頻度を週数で表します。  <br/> |
|[WeeklyRegeneration](weeklyregeneration.md) <br/> |タスクが再生成される頻度を数週間で示します。  <br/> |
|[YearlyRegeneration](yearlyregeneration.md) <br/> |タスクが再生成される頻度 (年数) について説明します。  <br/> |
   
## <a name="text-value"></a>テキスト値

整数を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

