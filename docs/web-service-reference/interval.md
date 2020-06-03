---
title: Interval/間隔
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
description: Interval 要素は、連続する2つのアイテム間の間隔を定義します。
ms.openlocfilehash: 70a41cfc438f057cbe11d792f0004d46d0abcc85
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526565"
---
# <a name="interval"></a>Interval/間隔

**Interval**要素は、連続する2つのアイテム間の間隔を定義します。 
  
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
|[DailyRegeneration](dailyregeneration.md) <br/> |タスクが再生成される頻度 (日単位) を表します。  <br/> |
|[DailyRecurrence](dailyrecurrence.md) <br/> |タスクが繰り返される頻度 (日単位) を表します。  <br/> |
|[月の明示再生](monthlyregeneration.md) <br/> |タスクが再生成される頻度 (月単位) を表します。  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |定期的なタスクの相対月パターンを表します。  <br/> |
|[WeeklyRecurrence](weeklyrecurrence.md) <br/> |頻度 (週単位) と、タスクが繰り返される曜日を表します。  <br/> |
|[WeeklyRegeneration](weeklyregeneration.md) <br/> |タスクが再生成される頻度 (週単位) を表します。  <br/> |
|[YearlyRegeneration](yearlyregeneration.md) <br/> |タスクが再生成される頻度 (年単位) を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

整数を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

