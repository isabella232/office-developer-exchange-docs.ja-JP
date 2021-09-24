---
title: TransitionsGroups
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- TransitionsGroups
api_type:
- schema
ms.assetid: ad0849f8-5158-4a23-9c36-a49f5be1d1e1
description: TransitionsGroups 要素は、タイム ゾーン移行グループの配列を表します。
ms.openlocfilehash: cd394d0ec333f639542c44cef6c992b24b69f65c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515124"
---
# <a name="transitionsgroups"></a>TransitionsGroups

**TransitionsGroups 要素** は、タイム ゾーン移行グループの配列を表します。 
  
```XML
<TransitionsGroups>
   <TransitionsGroup/>
</TransitionsGroups>
```

 **ArrayOfTransitionsGroupsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[TransitionsGroup](transitionsgroup.md) <br/> |タイム ゾーン遷移の配列を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[StartTimeZone](starttimezone.md) <br/> |[CalendarItem](calendaritem.md)または MeetingRequest の開始時刻のタイム ゾーン[を定義します](meetingrequest.md)。  <br/> |
|[EndTimeZone](endtimezone.md) <br/> |[CalendarItem](calendaritem.md)または MeetingRequest の終了時刻のタイム ゾーン[を定義します](meetingrequest.md)。  <br/> |
|[TimeZoneDefinition](timezonedefinition.md) <br/> |タイム ゾーンを定義します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

