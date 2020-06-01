---
title: バイアス
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bias
api_type:
- schema
ms.assetid: ae10aa44-e6d3-483d-a3e6-bb9c45966810
description: Bias 要素は、標準時および夏時間時に Bias (UTC) 要素によって識別される協定世界時 (UTC) オフセットからのオフセットを表します。 この値は分単位です。
ms.openlocfilehash: 6c9dce88f3eece9c793fb018114f07a85c7cb89b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460240"
---
# <a name="bias"></a>バイアス

**Bias**要素は、標準時および夏時間時に[bias (utc)](bias-utc.md)要素によって識別される協定世界時 (utc) オフセットからのオフセットを表します。 この値は分単位です。 
  
```xml
<Bias>...</Bias>
```

**int**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | [Bias (utc)](bias-utc.md)要素で表される utc を基準とした時間からのオフセットを表します。 この要素には、夏時間が計測される地域で夏時間から標準時への切り替えに関する情報も含まれます。<br/><br/>[Standardtime](standardtime.md)要素に対する XPath 式を次に示します。<br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | 夏時間が計測される地域で、 [Bias (utc)](bias-utc.md)要素によって表される utc を基準とした時刻からのオフセットを表します。 この要素には、標準時から夏時間への切り替えが行われるタイミングに関する情報も含まれています。  <br/><br/>[Daylighttime](daylighttime.md)要素の XPath 式を次に示します。<br/><br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は、整数を表します。
  
## <a name="remarks"></a>注釈

現地時刻を決定するために使用されるオフセットは、 **Bias**要素のいずれかによってのみ提供されます。 [Daylighttime](daylighttime.md)要素、 [standardtime](standardtime.md)要素、および[bias (UTC)](bias-utc.md)要素によって提供される bias 要素の値の合計は、現地時刻を示します。 
  
## <a name="example"></a>例

次の例は、UTC を60分間で調整して夏時間を管理するユーザーを識別する、XML 要求の一部を示しています。 これにより、実質的に UTC から420分のずれが生じます。
  
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

