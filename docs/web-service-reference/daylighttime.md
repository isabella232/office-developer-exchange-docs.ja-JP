---
title: DaylightTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DaylightTime
api_type:
- schema
ms.assetid: 9f551ee4-d945-477c-b981-9554b197d26d
description: DaylightTime 要素を基準にして世界協定時刻 (UTC) 夏時間が発生した地域のバイアス (UTC) の要素で表される時間からのオフセットを表します。 この要素には、標準時間から夏時間への切り替えが発生した場合についての情報も含まれています。
ms.openlocfilehash: 07ec4b1a5f84669aca33d46cdf1fa2e578f3b43b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759934"
---
# <a name="daylighttime"></a>DaylightTime

**DaylightTime**要素を基準にして世界協定時刻 (UTC) 夏時間が発生した地域の[バイアス (UTC)](bias-utc.md)の要素で表される時間からのオフセットを表します。 この要素には、標準時間から夏時間への切り替えが発生した場合についての情報も含まれています。 
  
- [タイムゾーン (可用性)](timezone-availability.md) 
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

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Bias](bias.md) <br/> |標準時間と夏時間の[時差 (UTC)](bias-utc.md)の要素で識別されている UTC オフセットからのオフセットを表します。 この値は分単位です。  <br/> |
|[時間](time.md) <br/> |標準時間と夏時間との間に 1 日の切り替え時間を表します。  <br/> |
|[DayOrder](dayorder.md) <br/> |標準時間と夏時間との切り替えの日付を表す[曜日 (タイムゾーン)](dayofweek-timezone.md)の要素で指定されている日の _n_th の発生を表します。  <br/> |
|[Month](month.md) <br/> |標準時間と夏時間との間の切り替えの月を表します。  <br/> |
|[DayOfWeek (タイムゾーン)](dayofweek-timezone.md) <br/> |標準時間と夏時間からの切り替えが発生する曜日を表します。  <br/> |
|[年](year.md) <br/> |年によって変更されるタイム ゾーンの定義に使用されます。 この要素はオプションです。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[タイムゾーン (可用性)](timezone-availability.md) <br/> | タイム ゾーン情報を識別する要素が含まれています。<br/><br/>この要素には、標準時と夏時間の切り替えに関する情報も含まれています。<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone` <br/><br/>`/GetUserAvailabilityRequest/TimeZone` <br/> |
   
## <a name="example"></a>例

次のような GetUserAvailability の部分の要求では、夏時間を認識する場所にクライアント アプリケーションを表します。
  
```xml
<TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

