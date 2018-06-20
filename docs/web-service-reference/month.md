---
title: Month
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Month
api_type:
- schema
ms.assetid: b12ac64f-b230-4573-be05-c86a428c4965
description: 月要素は、標準時間と夏時間との間の切り替えの月を表します。
ms.openlocfilehash: 73d052ef16bc51cd574eb8b04e21546f97347258
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832476"
---
# <a name="month"></a>Month

**月**要素は、標準時間と夏時間との間の切り替えの月を表します。 
  
```xml
<Month>...</Month>
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
|[StandardTime](standardtime.md) <br/> | 基準にして世界協定時刻 (UTC)[バイアス (UTC)](bias-utc.md)の要素で表される時間からのオフセットを表します。 この要素は、夏時間が発生した地域で夏時間から切り替えに関する情報を標準時も含みます。 <br/> <br/>  [StandardTime](standardtime.md)要素への XPath 式は、次のように。 <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/StandardTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/StandardTime` <br/> |
|[DaylightTime](daylighttime.md) <br/> | 夏時間が発生した地域の[バイアス (UTC)](bias-utc.md)の要素で表される UTC 時間からのオフセットを表します。 この要素には、標準時間から夏時間への切り替えが発生した場合についての情報も含まれています。  <br/><br/>  [DaylightTime](daylighttime.md)要素への XPath 式は、次のように。  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/TimeZone/DaylightTime` <br/><br/>  `/GetUserAvailabilityRequest/TimeZone/DaylightTime` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 値が現れることにより、月の順序のランクを表す、1 から 12 までの数値である必要があります。 これは、short 型の整数データ型です。
  
## <a name="remarks"></a>備考

5 の値を持つ[DayOrder](dayorder.md)要素、10 の値を持つ**月**の要素と、日曜日の値を持つ[DayOfWeek (タイムゾーン)](dayofweek-timezone.md)の要素を含む[StandardTime](standardtime.md)要素を意味する (標準時) からの移行夏時間は、10 月の 5 番目の日曜日に発生します。 
  
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

