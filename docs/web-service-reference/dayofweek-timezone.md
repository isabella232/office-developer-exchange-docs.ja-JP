---
title: DayOfWeek (タイムゾーン)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 416e8892-ebb1-4fac-82cf-e27549a6c175
description: DayOfWeek の要素では、タイム ゾーンの切り替えが発生する曜日を表します。
ms.openlocfilehash: 7816b90000be36cf3a3354d26d978684bfdcfe40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759935"
---
# <a name="dayofweek-timezone"></a>DayOfWeek (タイムゾーン)

**DayOfWeek**の要素では、タイム ゾーンの切り替えが発生する曜日を表します。 
  
```xml
<DayOfWeek>...</DayOfWeek>
```

**DayOfWeekType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | 基準にして世界協定時刻 (UTC)[バイアス (UTC)](bias-utc.md)の要素で表される時間からのオフセットを表します。<br/><br/>この要素は、夏時間が発生した地域で夏時間から切り替えに関する情報を標準時も含みます。<br/><br/>この要素への XPath 式は、次のように。<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | 夏時間が発生した地域の[バイアス (UTC)](bias-utc.md)の要素で表される UTC 時間からのオフセットを表します。<br/><br/>この要素には、標準時間から夏時間への切り替えが発生した場合についての情報も含まれています。<br/><br/>この要素への XPath 式は、次のように。<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
|[RecurringDayTransition](recurringdaytransition.md) <br/> |毎年同じ日に発生するタイム ゾーンの移行を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、次の値を持つ列挙型で表されます。
  
- 日曜日    
- 月曜日    
- 火曜日    
- 水曜日    
- 木曜日    
- 金曜日    
- 土曜日    
- 日    
- 週日   
- WeekendDay
    
## <a name="remarks"></a>備考

5 の値を持つ[DayOrder](dayorder.md)要素、10 の値を持つ[月](month.md)の要素、および**日曜日の値を持つ値**が含まれている[StandardTime](standardtime.md)要素は、標準時間から夏時間への移行を提供します。時間の節約は、10 月の 5 番目の日曜日に発生します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserAvailability 操作](getuseravailability-operation.md)
- [ユーザーの状態を取得します。](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

