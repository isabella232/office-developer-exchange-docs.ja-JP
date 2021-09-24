---
title: Periods
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Periods
api_type:
- schema
ms.assetid: 7920d81d-abba-4232-8bfe-49267b6c9a36
description: Periods 要素は、タイム ゾーンの異なるステージでのタイム オフセットを定義する期間の配列を表します。
ms.openlocfilehash: e4a614c71e7194dd85db740da1796b69d9f25d69
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515314"
---
# <a name="periods"></a>Periods

**Periods 要素** は、タイム ゾーンの異なるステージでのタイム オフセットを定義する期間の配列を表します。 
  
```xml
<Periods>
   <Period/>
</Periods>
```

 **NonEmptyArrayOfPeriodsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Period](period.md) <br/> |タイム ゾーンの特定のステージの名前、タイム オフセット、および一意の識別子を定義します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[StartTimeZone](starttimezone.md) <br/> |[CalendarItem](calendaritem.md)または MeetingRequest の開始時刻のタイム ゾーン[を定義します](meetingrequest.md)。  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |[CalendarItem](calendaritem.md)または MeetingRequest の終了時刻のタイム ゾーン[を定義します](meetingrequest.md)。  <br/> |
|[TimeZoneDefinition](timezonedefinition.md) <br/> |タイム ゾーンを定義します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされているコンピューター Microsoft Exchange Server EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

