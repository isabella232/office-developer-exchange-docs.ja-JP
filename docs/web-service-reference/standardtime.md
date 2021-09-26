---
title: StandardTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- StandardTime
api_type:
- schema
ms.assetid: 13084726-ab24-4009-be99-c4a4273c9e05
description: StandardTime 要素は、バイアス (UTC) 要素で表される協定世界時 (UTC) を基準にした時刻からのオフセットを表します。 この要素には、夏時間が観測される地域の夏時間からの標準時への移行に関する情報も含みます。
ms.openlocfilehash: ceddc511bf1883078c88dee240fc308d02024220
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59544662"
---
# <a name="standardtime"></a>StandardTime

**StandardTime 要素** は、バイアス (UTC) 要素で表される協定世界時 [(UTC)](bias-utc.md)を基準にした時刻からのオフセットを表します。 この要素には、夏時間が観測される地域の夏時間からの標準時への移行に関する情報も含みます。 
  
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
|[バイアス](bias.md) <br/> |標準時と夏時間の Bias [(UTC)](bias-utc.md) 要素で識別される UTC オフセットからのオフセットを表します。 この値は分単位です。  <br/> |
|[Time](time.md) <br/> |標準時と夏時間の切り替え時刻を表します。  <br/> |
|[DayOrder](dayorder.md) <br/> |標準時_n_th夏時間への移行日を表す [DayOfWeek (TimeZone)](dayofweek-timezone.md) 要素で指定された日の日付を表します。  <br/> |
|[Month](month.md) <br/> |標準時と夏時間の間の移行月を表します。  <br/> |
|[DayOfWeek (TimeZone)](dayofweek-timezone.md) <br/> |標準時と夏時間の間の移行が発生する週の日を表します。  <br/> |
|[Year](year.md) <br/> |年に応じて変更されるタイム ゾーンを定義します。 この要素は省略できます。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[TimeZone (Availability)](timezone-availability.md) <br/> | タイム ゾーン情報を識別する要素が含まれます。 この要素には、標準時と夏時間の切り替えに関する情報も含みます。 <br/><br/>この要素の XPath 式を次に示します。 <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/> <br/> `/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="remarks"></a>注釈

**StandardTime 要素** は、Bias (UTC) 要素で表されるオフセット [時間を表](bias-utc.md)します。 子 Bias 要素 [が](bias.md) 0 の場合、標準時間は [Bias (UTC)](bias-utc.md) 要素で表される UTC からのバイアス オフセットと等しくなります。 
  
## <a name="example"></a>例

次の例は、夏時間が観測される領域を示しています。 夏時間から標準時への移行は、2 時に観測されます。 第 10 月の第 5 日曜日。
  
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
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserAvailability 操作](getuseravailability-operation.md)
- [ユーザーの可用性の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

