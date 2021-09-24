---
title: Month
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Month
api_type:
- schema
ms.assetid: b12ac64f-b230-4573-be05-c86a428c4965
description: Month 要素は、標準時と夏時間の間の移行月を表します。
ms.openlocfilehash: aca81faf2767e17dab956db9a208245fbd0b7d83
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59520431"
---
# <a name="month"></a>Month

**Month 要素** は、標準時と夏時間の間の移行月を表します。 
  
```xml
<Month>...</Month>
```

 **Short**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[StandardTime](standardtime.md) <br/> | Bias (UTC) 要素で表される協定世界時 [(UTC)](bias-utc.md) を基準にした時刻からのオフセットを表します。 この要素には、夏時間が観測される地域の夏時間からの標準時への移行に関する情報も含みます。 <br/> <br/>  StandardTime 要素の XPath 式を次 [に示](standardtime.md) します。 <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | 夏時間が観測される地域の [Bias (UTC)](bias-utc.md) 要素で表される UTC からの相対時間からのオフセットを表します。 この要素には、標準時からの夏時間への移行がいつ行われるかについての情報も含みます。  <br/><br/>  DaylightTime 要素の XPath 式を [次に示](daylighttime.md) します。  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 この値は、出現回数別の月の序数ランクを表し、1 ~ 12 の数値である必要があります。 これは短い整数データ型です。
  
## <a name="remarks"></a>注釈

値が 5 の[DayOrder](dayorder.md)要素、値が 10の Month 要素、日曜日の値を持つ[DayOfWeek (TimeZone)](dayofweek-timezone.md)要素を含む StandardTime 要素は、標準時から夏時間への移行が 10 か月目の第 5 日曜日に発生します。 [](standardtime.md) 
  
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

