---
title: DayOrder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DayOrder
api_type:
- schema
ms.assetid: 3022f839-12a2-42a9-820e-3ea585ce8657
description: DayOrder 要素は、期間から標準時および夏時間に移行する日付を表す、DayOfWeek (TimeZone) 要素で指定された日の n 番目の出現を表します。
ms.openlocfilehash: 53a8cb979bdb7aefead5623b4680f4c1a4ef5509
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526964"
---
# <a name="dayorder"></a>DayOrder

**Dayorder**要素は、期間から標準時および夏時間に移行する日付を表す[DayOfWeek (TimeZone)](dayofweek-timezone.md)要素で指定された日の _n_th を表します。 
  
```xml
<DayOrder>...</DayOrder>
```

**短い**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | 時間のオフセット (協定世界時 (UTC) を基準として、 [Bias (utc)](bias-utc.md)要素で表される) を表します。<br/><br/>この要素には、夏時間が計測される地域で夏時間から標準時への切り替えに関する情報も含まれます。<br/><br/>[Standardtime](standardtime.md)要素に対する XPath 式を次に示します。<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | 夏時間が計測される地域で、 [Bias (utc)](bias-utc.md)要素によって表される utc を基準とした時刻からのオフセットを表します。<br/><br/>この要素には、標準時から夏時間への切り替えが行われるタイミングに関する情報も含まれています。<br/><br/>[Daylighttime](daylighttime.md)要素の XPath 式を次に示します。<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 **Dayorder**要素の値は、1 ~ 5 にすることができます。 この要素の最大値は、月と年に応じて4または5のいずれかになります。 
  
## <a name="remarks"></a>注釈

値5、値10を持つ[Month](month.md)要素、および値が日曜日である[DayOfWeek (TimeZone)](dayofweek-timezone.md)要素を含む**Dayorder**要素を含む[standardtime](standardtime.md)要素は、標準時から夏時間への切り替えが10月の5番目の日曜日に行われることを意味します。 
  
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

