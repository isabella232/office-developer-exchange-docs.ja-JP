---
title: 時刻
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Time
api_type:
- schema
ms.assetid: c4b98be7-141c-4ba8-97ef-9ad1ed19f61f
description: Time 要素は、標準時と夏時間の間の移行時刻を表します。
ms.openlocfilehash: d9cd83a7dcb0a296693e3daa1874b12294de5857
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513270"
---
# <a name="time"></a>Time

**Time 要素** は、標準時と夏時間の間の移行時刻を表します。 
  
```xml
<Time>...</Time>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Bias (UTC) 要素で表される協定世界時 [(UTC)](bias-utc.md) を基準にした時刻からのオフセットを表します。 この要素には、夏時間が観測される地域の夏時間からの標準時への移行に関する情報も含みます。  <br/><br/>  StandardTime 要素の XPath 式を次 [に示](standardtime.md) します。 <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime`<br/> <br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | 夏時間が観測される地域の [Bias (UTC)](bias-utc.md) 要素で表される UTC からの相対時間からのオフセットを表します。 この要素には、標準時からの夏時間への移行がいつ行われるかについての情報も含みます。  <br/><br/>  DaylightTime 要素の XPath 式を [次に示](daylighttime.md) します。  <br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、hh:mm:ss という形式の時間、分、および秒を表します。
  
## <a name="remarks"></a>注釈

Time 要素 **が DaylightTime** [](daylighttime.md)要素で発生すると、夏時間から標準時への移行が発生する時刻を表します。 [StandardTime](standardtime.md) [要素で](time.md)Time 要素が発生すると、標準時から夏時間への移行が発生する時刻を表します。 
  
この要素の最小出現回数は 0 で、最大出現回数は 1 です。
  
## <a name="example"></a>例

要求の次の部分は、2 A.M の移行時間を表します。 標準時から夏時間まで。
  
```xml
<StandardTime>
   <Bias>0</Bias>
   <Time>02:00:00</Time>
   <DayOrder>5</DayOrder>
   <Month>10</Month>
   <DayOfWeek>Sunday</DayOfWeek>
</StandardTime
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

