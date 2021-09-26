---
title: DaylightTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DaylightTime
api_type:
- schema
ms.assetid: 9f551ee4-d945-477c-b981-9554b197d26d
description: DaylightTime 要素は、夏時間が観測される地域の Bias (UTC) 要素で表される協定世界時 (UTC) を基準にした時刻からのオフセットを表します。 この要素には、標準時からの夏時間への移行がいつ行われるかについての情報も含みます。
ms.openlocfilehash: 95d09fe01602f2d55d1a39dc7164a3f60a328f2a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543433"
---
# <a name="daylighttime"></a>DaylightTime

**DaylightTime** 要素は、夏時間が観測される地域の [Bias (UTC)](bias-utc.md)要素で表される協定世界時 (UTC) を基準にした時刻からのオフセットを表します。 この要素には、標準時からの夏時間への移行がいつ行われるかについての情報も含みます。 
  
- [TimeZone (Availability)](timezone-availability.md) 
- [DaylightTime](daylighttime.md)
  
```xml
<DaylightTime>
   <Bias>int</Bias>
   <Time>string</Time>
   <DayOrder>short</DayOrder>
   <Month>short</Month>
   <DayOfWeek>Sunday or Monday or Tuesday or Wednesday or Thursday or Friday or Saturday</DayOfWeek>
   <Year>string</Year>
</DaylightTime>
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
|[Year](year.md) <br/> |年に応じて変化するタイム ゾーンを定義するために使用します。 この要素は省略できます。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[TimeZone (Availability)](timezone-availability.md) <br/> | タイム ゾーン情報を識別する要素が含まれます。<br/><br/>この要素には、標準時と夏時間の切り替えに関する情報も含みます。<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="example"></a>例

次の部分的な GetUserAvailability 要求は、夏時間を認識する場所にあるクライアント アプリケーションを表します。
  
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

