---
title: 時刻
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Time
api_type:
- schema
ms.assetid: c4b98be7-141c-4ba8-97ef-9ad1ed19f61f
description: 時刻要素は、標準時間と夏時間との間に 1 日の切り替え時間を表します。
ms.openlocfilehash: 716487fb7ed64dbaa6fa97caf1ea608e4673d2ef
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839676"
---
# <a name="time"></a>時刻型 (Time)

**時刻**要素は、標準時間と夏時間との間に 1 日の切り替え時間を表します。 
  
```xml
<Time>...</Time>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | 基準にして世界協定時刻 (UTC)[バイアス (UTC)](bias-utc.md)の要素で表される時間からのオフセットを表します。 この要素は、夏時間が発生した地域で夏時間から切り替えに関する情報を標準時も含みます。  <br/><br/>  [StandardTime](standardtime.md)要素への XPath 式は、次のように。 <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/> <br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | 夏時間が発生した地域の[バイアス (UTC)](bias-utc.md)の要素で表される UTC 時間からのオフセットを表します。 この要素には、標準時間から夏時間への切り替えが発生した場合についての情報も含まれています。  <br/><br/>  [DaylightTime](daylighttime.md)要素への XPath 式は、次のように。  <br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、時間、分、および次の形式で秒を表します: hh:mm:ss です。
  
## <a name="remarks"></a>備考

[DaylightTime](daylighttime.md)要素では、**時間**の要素が発生する場合は、夏時間から標準時への移行が発生する時刻を表します。 [時刻](time.md)要素は、 [StandardTime](standardtime.md)要素で発生した場合、標準時間から夏時間への切り替えが発生する時刻を表します。 
  
この要素には、最小出現回数が 0 と 1 つの最大出現します。
  
## <a name="example"></a>例

要求の次の部分は、午前 2 時の遷移時間を表します 夏時間への標準時間です。
  
```xml
<StandardTime>
   <Bias>0</Bias>
   <Time>02:00:00</Time>
   <DayOrder>5</DayOrder>
   <Month>10</Month>
   <DayOfWeek>Sunday</DayOfWeek>
</StandardTime
```

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

