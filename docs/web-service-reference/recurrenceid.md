---
title: RecurrenceId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- RecurrenceId
api_type:
- schema
ms.assetid: 9ef3569d-ee56-4b22-b008-609fb3337da7
description: RecurrenceId 要素は、定期的な予定表アイテムの特定のインスタンスを識別するために使用されます。
ms.openlocfilehash: 863673f7439c12ce4c74e8e0ef4ddea996fb4eb5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59527565"
---
# <a name="recurrenceid"></a>RecurrenceId

**RecurrenceId 要素は**、定期的な予定表アイテムの特定のインスタンスを識別するために使用されます。 
  
```xml
<RecurrenceId/>
```

 **dateTime**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |会議メッセージを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |会議の応答を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |会議のキャンセルを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、予定表の出現を識別する日付/時刻の値を表します。
  
## <a name="remarks"></a>注釈

このプロパティは、定期的な予定表アイテムの特定のインスタンスを識別するために [UID](uid.md) プロパティと一緒に使用されます。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

