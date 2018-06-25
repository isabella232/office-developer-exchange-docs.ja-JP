---
title: タイムゾーン (可用性)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZone
api_type:
- schema
ms.assetid: d662ffae-1f93-4c08-85a4-c69de2f7c681
description: タイム ゾーン要素には、タイム ゾーン情報を識別する要素が含まれています。 この要素には、標準時と夏時間の切り替えに関する情報も含まれています。
ms.openlocfilehash: dc2466e8039819edc82294ff05f1746ada64cb43
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839717"
---
# <a name="timezone-availability"></a>タイムゾーン (可用性)

**タイム ゾーン**要素には、タイム ゾーン情報を識別する要素が含まれています。 この要素には、標準時と夏時間の切り替えに関する情報も含まれています。 
  
```xml
<TimeZone>
   <Bias/>
   <StandardTime/>
   <DaylightTime/>
</TimeZone>
```

 **SerializableTimeZone**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[バイアス (UTC)](bias-utc.md) <br/> |世界協定時刻 (UTC) から一般のオフセットを表します。 この値は分単位です。  <br/> |
|[StandardTime](standardtime.md) <br/> |[バイアス (UTC)](bias-utc.md)の要素で表される UTC 時間からのオフセットを表します。 この要素は、夏時間が発生した地域で夏時間から切り替えに関する情報を標準時も含みます。  <br/> |
|[DaylightTime](daylighttime.md) <br/> |夏時間が発生した地域の[バイアス (UTC)](bias-utc.md)の要素で表される UTC 時間からのオフセットを表します。 この要素には、標準時間から夏時間への切り替えが発生した場合についての情報も含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |ユーザーの利用可能時間情報を取得するための引数が含まれています。 これは、ルート要素です。  <br/> GetUserAvailabilityRequest メッセージの**タイム ゾーン**の要素は、要求内の DateTime 値が指定されているタイム ゾーンを表します。 可用性サービスによって返される DateTime 値は、このタイム ゾーンでもあります。  <br/> 以下は、この要素の XPath です。  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |要求されたメールボックスのユーザーの作業時間とタイム ゾーンの設定を表します。  <br/> GetUserAvailabilityResponse メッセージの**タイム ゾーン**の要素は、要求されたメールボックス ユーザーのタイム ゾーンの設定を表します。  <br/> 以下は、この要素の XPath です。  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a>備考

[GetUserAvailabilityRequest](getuseravailabilityrequest.md)要素では、この要素が必要です。 0 回以上すると、親要素は、 [WorkingHours](workinghours-ex15websvcsotherref.md)要素またはこの要素は最大で 1 回に発生します。 
  
## <a name="example"></a>例

次の使用例は、クライアント アプリケーションで 8 時間の UTC からのオフセットを識別する XML 要求の一部を示しています。
  
```XML
<TimeZone xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
  <Bias>480</Bias>
  <StandardTime>
    <Bias>0</Bias>
    <Time>02:00:00</Time>
    <DayOrder>1</DayOrder>
    <Month>11</Month>
    <DayOfWeek>Sunday</DayOfWeek>
  </StandardTime>
  <DaylightTime>
    <Bias>-60</Bias>
    <Time>02:00:00</Time>
    <DayOrder>2</DayOrder>
    <Month>3</Month>
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



[GetUserAvailability 操作](getuseravailability-operation.md)
  
[Bias](bias.md)


[ユーザーの状態を取得します。](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

