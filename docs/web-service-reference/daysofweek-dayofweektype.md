---
title: DaysOfWeek (DayOfWeekType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DaysOfWeek
api_type:
- schema
ms.assetid: ba8f990d-d37d-403d-b31f-55e5208c8ad5
description: DaysOfWeek 要素は、アイテムの定期的なパターンで使用される曜日を表します。
ms.openlocfilehash: 44552350679df1fec3d237d9b09f1a5feb9cc4b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458825"
---
# <a name="daysofweek-dayofweektype"></a>DaysOfWeek (DayOfWeekType)

**DaysOfWeek**要素は、アイテムの定期的なパターンで使用される曜日を表します。 
  
```xml
<DaysOfWeek/>
```

**DayOfWeekType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RelativeYearlyRecurrence](relativeyearlyrecurrence.md) <br/> |相対的な年単位の定期的なパターンを記述します。  <br/> |
|[RelativeMonthlyRecurrence](relativemonthlyrecurrence.md) <br/> |相対的な月単位の定期的なパターンを記述します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 指定可能な値は次のいずれかです。
  
- 日曜日    
- 月曜日    
- 火曜日   
- 水曜日    
- 木曜日    
- 金曜日    
- 土曜日    
- Day (TimeChangePatternTypes では使用されません)    
- Weekday (TimeChangePatternTypes では使用されません)    
- WeekendDay (TimeChangePatternTypes では使用されません)
    
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

