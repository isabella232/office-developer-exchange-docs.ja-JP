---
title: TimeZone (Availability)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZone
api_type:
- schema
ms.assetid: d662ffae-1f93-4c08-85a4-c69de2f7c681
description: TimeZone 要素には、タイムゾーン情報を識別する要素が含まれています。 この要素には、標準時から夏時間への切り替えに関する情報も含まれています。
ms.openlocfilehash: ba4b0a4805dba54450e01e89c5e9ef746404b716
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460275"
---
# <a name="timezone-availability"></a>TimeZone (Availability)

**TimeZone**要素には、タイムゾーン情報を識別する要素が含まれています。 この要素には、標準時から夏時間への切り替えに関する情報も含まれています。 
  
```xml
<TimeZone>
   <Bias/>
   <StandardTime/>
   <DaylightTime/>
</TimeZone>
```

 **SerializableTimeZone**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Bias (UTC)](bias-utc.md) <br/> |協定世界時 (UTC) からの一般的なオフセットを表します。 この値は分単位です。  <br/> |
|[StandardTime](standardtime.md) <br/> |[Bias (utc)](bias-utc.md)要素で表される utc を基準とした時間からのオフセットを表します。 この要素には、夏時間が計測される地域で夏時間から標準時への切り替えに関する情報も含まれます。  <br/> |
|[DaylightTime](daylighttime.md) <br/> |夏時間が計測される地域で、 [Bias (utc)](bias-utc.md)要素によって表される utc を基準とした時刻からのオフセットを表します。 この要素には、標準時から夏時間への切り替えが行われるタイミングに関する情報も含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |ユーザーの空き時間情報を取得するために使用する引数が含まれています。 これはルート要素です。  <br/> GetUserAvailabilityRequest message の**TimeZone**要素は、要求の DateTime 値が指定されているタイムゾーンを表します。 Availability service によって返される DateTime 値もこのタイムゾーンに含まれています。  <br/> この要素の XPath を次に示します。  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |要求されたメールボックスユーザーのタイムゾーン設定および稼働時間を表します。  <br/> GetUserAvailabilityResponse message の**TimeZone**要素は、要求されたメールボックスユーザーのタイムゾーン設定を表します。  <br/> この要素の XPath を次に示します。  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a>注釈

この要素は[GetUserAvailabilityRequest](getuseravailabilityrequest.md)要素で必要です。 この要素は、親要素が[WorkingHours](workinghours-ex15websvcsotherref.md)要素の数回または少なくとも0回発生します。 
  
## <a name="example"></a>例

次の例は、クライアントアプリケーションで8時間の UTC からのオフセットを識別する XML 要求の一部を示しています。
  
```XML
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>11</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>2</DayOrder>
    <Month>3</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </DaylightTime>
</TimeZone>
```

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)
  
[バイアス](bias.md)


[ユーザーの空き時間情報の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

