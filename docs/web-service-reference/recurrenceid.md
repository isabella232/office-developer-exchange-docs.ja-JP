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
description: RecurrenceId 要素を使用して、定期的な予定表アイテムの特定のインスタンスを識別します。
ms.openlocfilehash: 078bec85e1ca1530137f9935365d7dd3e530ea34
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833005"
---
# <a name="recurrenceid"></a>RecurrenceId

**RecurrenceId**要素を使用して、定期的な予定表アイテムの特定のインスタンスを識別します。 
  
```xml
<RecurrenceId/>
```

 **dateTime**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |会議メッセージを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |会議の返信を表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |会議の取り消し通知を表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は、予定表アイテムを識別するための日付/時刻値を表します。
  
## <a name="remarks"></a>備考

このプロパティは、定期的な予定表アイテムの特定のインスタンスを識別する[UID](uid.md)プロパティを使用して使用します。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

