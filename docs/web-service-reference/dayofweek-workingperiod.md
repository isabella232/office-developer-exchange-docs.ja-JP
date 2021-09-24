---
title: DayOfWeek (WorkingPeriod)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- DayOfWeek
api_type:
- schema
ms.assetid: 7a8a8cc1-392b-4db5-bb76-710477e31396
description: DayOfWeek 要素には、メールボックス ユーザーにスケジュールされた作業日の一覧が含まれる。
ms.openlocfilehash: 97950d7f2d6db76ac76253979e9187bddc5c99e1
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59529007"
---
# <a name="dayofweek-workingperiod"></a>DayOfWeek (WorkingPeriod)

**DayOfWeek** 要素には、メールボックス ユーザーにスケジュールされた作業日の一覧が含まれる。 
  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)  
- [FreeBusyResponseArray](freebusyresponsearray.md)  
- [FreeBusyResponse](freebusyresponse.md)  
- [FreeBusyView](freebusyview.md)  
- [WorkingHours](workinghours-ex15websvcsotherref.md)  
- [WorkingPeriodArray](workingperiodarray.md) 
- [WorkingPeriod](workingperiod.md)  
- [DayOfWeek (WorkingPeriod)](dayofweek-workingperiod.md)
  
```xml
<DayOfWeek>Sunday Monday Tuesday Wednesday Thursday Friday Saturday</DayOfWeek>
```

**DaysOfWeek**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[WorkingPeriod](workingperiod.md) <br/> |メールボックス ユーザーの作業週の日と時間が含まれる。<br/><br/>次に、この要素の XPath 式を示します。<br/><br/>`/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/WorkingHours/WorkingPeriodArray/WorkingPeriod[i[` <br/> |
   
## <a name="text-value"></a>テキスト値

メールボックス ユーザーに、作業週を表す日数が設定されている場合は、テキスト値が返されます。 この要素で使用できる値は次のとおりです。
  
- 日曜日    
- 月曜日    
- 火曜日    
- 水曜日    
- 木曜日    
- 金曜日    
- 土曜日 
    
テキスト値は、その順序で返されます。
  
## <a name="remarks"></a>注釈

この要素と可用性 [DayOfWeek (TimeZone)](dayofweek-timezone.md) 要素の違いは型です。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserAvailability 操作](getuseravailability-operation.md)  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [ユーザーの可用性の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

