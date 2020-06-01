---
title: StandardTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StandardTime
api_type:
- schema
ms.assetid: 13084726-ab24-4009-be99-c4a4273c9e05
description: StandardTime 要素は、バイアス (UTC) 要素で表される協定世界時 (UTC) を基準とした時刻からのオフセットを表します。 この要素には、夏時間が計測される地域で夏時間から標準時への切り替えに関する情報も含まれます。
ms.openlocfilehash: 793f058840d4fd9216f03e660f5be0f7564906cf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456403"
---
# <a name="standardtime"></a>StandardTime

**Standardtime**要素は、[バイアス (utc](bias-utc.md) ) 要素で表される協定世界時 (utc) を基準とした時刻からのオフセットを表します。 この要素には、夏時間が計測される地域で夏時間から標準時への切り替えに関する情報も含まれます。 
  
- [TimeZone (Availability)](timezone-availability.md)
- [StandardTime](standardtime.md)
  
```xml
<StandardTime>
   <Bias>int</Bias>
   <Time>string</Time>
   <DayOrder>short</DayOrder>
   <Month>short</Month>
   <DayOfWeek>Sunday or Monday or Tuesday or Wednesday or Thursday or Friday or Saturday</DayOfWeek>
   <Year>string</Year>
</StandardTime>
```

 **SerializableTimeZoneTime**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[バイアス](bias.md) <br/> |標準時と夏時間の[時差 (utc)](bias-utc.md)要素によって識別される utc オフセットからのオフセットを表します。 この値は分単位です。  <br/> |
|[Time](time.md) <br/> |標準時と夏時間の切り替え時間を表します。  <br/> |
|[DayOrder](dayorder.md) <br/> |標準時および夏時間への切り替えの日付を表す、 [DayOfWeek (TimeZone)](dayofweek-timezone.md)要素で指定された日の _n_th 発生を表します。  <br/> |
|[Month](month.md) <br/> |標準時と夏時間との間の年間の移行月を表します。  <br/> |
|[DayOfWeek (TimeZone)](dayofweek-timezone.md) <br/> |標準時および夏時間からの切り替えが行われる曜日を表します。  <br/> |
|[Year](year.md) <br/> |年に応じて変更されるタイムゾーンを定義します。 この要素は省略できます。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[TimeZone (Availability)](timezone-availability.md) <br/> | タイムゾーン情報を識別する要素を格納します。 この要素には、標準時から夏時間への切り替えに関する情報も含まれています。 <br/><br/>この要素の XPath 式は次のとおりです。 <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/> <br/> `/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="remarks"></a>注釈

**Standardtime**要素は、 [Bias (UTC)](bias-utc.md)要素で表されるオフセット時間を表します。 子[バイアス](bias.md)要素が0と等しい場合、標準時は[bias (utc)](bias-utc.md)要素で表される、utc からのバイアスオフセットと等しくなります。 
  
## <a name="example"></a>例

次の例は、夏時間が測定される地域を示しています。 夏時間から標準時への切り替えは午前2時に発生します。 10月の5番目の日曜日。
  
```xml
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>5</DayOrder>
    <Month>10</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>4</Month>
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

- [GetUserAvailability 操作](getuseravailability-operation.md)
- [ユーザーの空き時間情報の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

