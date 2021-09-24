---
title: Bias
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Bias
api_type:
- schema
ms.assetid: ae10aa44-e6d3-483d-a3e6-bb9c45966810
description: Bias 要素は、標準時と夏時間の Bias (UTC) 要素で識別される協定世界時 (UTC) オフセットからのオフセットを表します。 この値は分単位です。
ms.openlocfilehash: 557605380dbda8c980272edcf445bb8099e14ada
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516098"
---
# <a name="bias"></a>Bias

**Bias 要素** は、標準時と夏時間の Bias (UTC) 要素で識別される協定世界時 [(UTC)](bias-utc.md)オフセットからのオフセットを表します。 この値は分単位です。 
  
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
|[StandardTime](standardtime.md) <br/> | Bias [(UTC)](bias-utc.md) 要素で表される UTC からの相対時間からのオフセットを表します。 この要素には、夏時間が観測される地域の夏時間からの標準時への移行に関する情報も含みます。<br/><br/>StandardTime 要素の XPath 式を次 [に示](standardtime.md) します。<br/><br/>   `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | 夏時間が観測される地域の [Bias (UTC)](bias-utc.md) 要素で表される UTC からの相対時間からのオフセットを表します。 この要素には、標準時からの夏時間への移行がいつ行われるかについての情報も含みます。  <br/><br/>DaylightTime 要素の XPath 式を [次に示](daylighttime.md) します。<br/><br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/> `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 テキスト値は整数を表します。
  
## <a name="remarks"></a>注釈

現地時間を決定するために使用されるオフセットは、Bias 要素の 1 つによって **のみ指定** できます。 [DaylightTime](daylighttime.md)要素または[StandardTime](standardtime.md)要素と Bias [(UTC)](bias-utc.md)要素によって提供される Bias 要素の値の合計は、現地時間を識別します。 
  
## <a name="example"></a>例

次の例は、UTC からのオフセットを -60 分調整して夏時間を観察するユーザーを識別する XML 要求の一部を示しています。 これにより、UTC から 420 分のバイアスが有効になります。
  
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

