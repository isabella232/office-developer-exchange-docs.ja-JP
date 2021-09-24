---
title: DayOfWeek (TimeZone)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 416e8892-ebb1-4fac-82cf-e27549a6c175
description: DayOfWeek 要素は、タイム ゾーンの切り替えが発生する週の日を表します。
ms.openlocfilehash: 5b51a3692a1836d2d2448df88b0ec07ccf1d79a5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59519899"
---
# <a name="dayofweek-timezone"></a>DayOfWeek (TimeZone)

**DayOfWeek** 要素は、タイム ゾーンの切り替えが発生する週の日を表します。 
  
```xml
<DayOfWeek>...</DayOfWeek>
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
|[StandardTime](standardtime.md) <br/> | Bias (UTC) 要素で表される協定世界時 [(UTC)](bias-utc.md) を基準にした時刻からのオフセットを表します。<br/><br/>この要素には、夏時間が観測される地域の夏時間からの標準時への移行に関する情報も含みます。<br/><br/>この要素の XPath 式を次に示します。<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | 夏時間が観測される地域の [Bias (UTC)](bias-utc.md) 要素で表される UTC からの相対時間からのオフセットを表します。<br/><br/>この要素には、標準時からの夏時間への移行がいつ行われるかについての情報も含みます。<br/><br/>この要素の XPath 式を次に示します。<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |毎年同じ日に発生するタイム ゾーン遷移を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、次の可能な値を持つ列挙で表されます。
  
- 日曜日    
- 月曜日    
- 火曜日    
- 水曜日    
- 木曜日    
- 金曜日    
- 土曜日    
- Day    
- 平日   
- WeekendDay
    
## <a name="remarks"></a>注釈

値が 5 の [DayOrder](dayorder.md)要素、値が 10 の [Month](month.md)要素、および日曜日の値を持つ **DayOfWeek** 要素を含む [StandardTime](standardtime.md)要素は、標準時から夏時間への移行が第 10 月の第 5 日曜日に発生します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserAvailability 操作](getuseravailability-operation.md)
- [ユーザーの可用性の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

