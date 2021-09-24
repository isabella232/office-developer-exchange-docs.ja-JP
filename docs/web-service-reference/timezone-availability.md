---
title: TimeZone (Availability)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TimeZone
api_type:
- schema
ms.assetid: d662ffae-1f93-4c08-85a4-c69de2f7c681
description: TimeZone 要素には、タイム ゾーン情報を識別する要素が含まれています。 この要素には、標準時と夏時間の切り替えに関する情報も含みます。
ms.openlocfilehash: 7ca6f0f2d9950770055d19c04adab9b76b95c295
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538843"
---
# <a name="timezone-availability"></a>TimeZone (Availability)

**TimeZone 要素には**、タイム ゾーン情報を識別する要素が含まれています。 この要素には、標準時と夏時間の切り替えに関する情報も含みます。 
  
```xml
<TimeZone>
   <Bias/>
   <StandardTime/>
   <DaylightTime/>
</TimeZone>
```

 **SerializableTimeZone**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Bias (UTC)](bias-utc.md) <br/> |協定世界時 (UTC) からの一般的なオフセットを表します。 この値は分単位です。  <br/> |
|[StandardTime](standardtime.md) <br/> |Bias [(UTC)](bias-utc.md) 要素で表される UTC からの相対時間からのオフセットを表します。 この要素には、夏時間が観測される地域の夏時間からの標準時への移行に関する情報も含みます。  <br/> |
|[DaylightTime](daylighttime.md) <br/> |夏時間が観測される地域の [Bias (UTC)](bias-utc.md) 要素で表される UTC からの相対時間からのオフセットを表します。 この要素には、標準時からの夏時間への移行がいつ行われるかについての情報も含みます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |ユーザーの可用性情報を取得するために使用される引数を格納します。 これはルート要素です。  <br/> GetUserAvailabilityRequest メッセージの TimeZone 要素は、要求内の DateTime 値が指定されているタイム ゾーンを表します。  可用性サービスによって返される DateTime 値もこのタイム ゾーンに含まれます。  <br/> 次に、この要素の XPath を示します。  <br/>  `/GetUserAvailabilityRequest` <br/> |
|[WorkingHours](workinghours-ex15websvcsotherref.md) <br/> |要求されたメールボックス ユーザーのタイム ゾーン設定と作業時間を表します。  <br/> GetUserAvailabilityResponse メッセージの TimeZone 要素は、要求されたメールボックス ユーザーのタイム ゾーン設定を表します。   <br/> 次に、この要素の XPath を示します。  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours` <br/> |
   
## <a name="remarks"></a>注釈

この要素は [、GetUserAvailabilityRequest 要素で必要](getuseravailabilityrequest.md) です。 この要素は、親要素が [WorkingHours](workinghours-ex15websvcsotherref.md) 要素である場合、少なくとも 1 回、または少なくとも 0 回発生します。 
  
## <a name="example"></a>例

次の例は、クライアント アプリケーションの UTC 8 時間からのオフセットを識別する XML 要求の一部を示しています。
  
```XML
<TimeZone xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)
  
[バイアス](bias.md)


[ユーザーの可用性の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

