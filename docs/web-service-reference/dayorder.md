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
description: DayOrder 要素は、標準時間と夏時間との切り替えの日付を表す曜日 (タイムゾーン) の要素で指定された日の n 番目の発生を表します。
ms.openlocfilehash: 03ee678611a6cf58a7256ded67ab4d0a8a06a7ee
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759940"
---
# <a name="dayorder"></a>DayOrder

**DayOrder**要素は、標準時間と夏時間との切り替えの日付を表す[曜日 (タイムゾーン)](dayofweek-timezone.md)の要素で指定された日の _n_th の発生を表します。 
  
```xml
<DayOrder>...</DayOrder>
```

**短い**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | 基準にして世界協定時刻 (UTC)[バイアス (UTC)](bias-utc.md)の要素で表される時間からのオフセットを表します。<br/><br/>この要素は、夏時間が発生した地域で夏時間から切り替えに関する情報を標準時も含みます。<br/><br/>[StandardTime](standardtime.md)要素への XPath 式は、次のように。<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | 夏時間が発生した地域の[バイアス (UTC)](bias-utc.md)の要素で表される UTC 時間からのオフセットを表します。<br/><br/>この要素には、標準時間から夏時間への切り替えが発生した場合についての情報も含まれています。<br/><br/>[DaylightTime](daylighttime.md)要素への XPath 式は、次のように。<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime`<br/><br/>`/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 **DayOrder**要素の値は 1 ~ 5 にできます。 この要素の最大値は 4 または 5、月、年によってのいずれかにできます。 
  
## <a name="remarks"></a>備考

5 の値を持つ**DayOrder**要素、10 の値を持つ[月](month.md)の要素と、日曜日の値を持つ[DayOfWeek (タイムゾーン)](dayofweek-timezone.md)の要素を含む[StandardTime](standardtime.md)要素を意味する (標準時) からの移行夏時間は、10 月の 5 番目の日曜日に発生します。 
  
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

