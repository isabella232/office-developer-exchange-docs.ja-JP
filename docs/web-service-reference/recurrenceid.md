---
title: RecurrenceId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RecurrenceId
api_type:
- schema
ms.assetid: 9ef3569d-ee56-4b22-b008-609fb3337da7
description: RecurrenceId 要素は、定期的な予定表アイテムの特定のインスタンスを識別するために使用されます。
ms.openlocfilehash: 58a379f2cffa7ff37181e93ad1c45c9752e84f1d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461612"
---
# <a name="recurrenceid"></a>RecurrenceId

**RecurrenceId**要素は、定期的な予定表アイテムの特定のインスタンスを識別するために使用されます。 
  
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
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |会議メッセージを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |会議出席依頼の返信を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |会議の取り消しを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、予定表の発生を識別する日付/時刻の値を表します。
  
## <a name="remarks"></a>注釈

このプロパティは、定期的な予定表アイテムの特定のインスタンスを識別するために、 [UID](uid.md)プロパティと共に使用されます。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

