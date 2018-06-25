---
title: AssociatedCalendarItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AssociatedCalendarItemId
api_type:
- schema
ms.assetid: 5b29898c-ea59-4e6a-914c-c011ec754032
description: AssociatedCalendarItemId 要素は、MeetingMessage、MeetingRequest、MeetingResponse、MeetingCancellation、または ReminderMessageData に関連付けられている予定表アイテムを表します。
ms.openlocfilehash: 4445da88d6fec42c1e02cd8de4d2e423485a4472
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759448"
---
# <a name="associatedcalendaritemid"></a>AssociatedCalendarItemId

**AssociatedCalendarItemId**要素は、 [MeetingMessage](meetingmessage.md)、 [MeetingRequest](meetingrequest.md)、 [MeetingResponse](meetingresponse.md)、 [MeetingCancellation](meetingcancellation.md)、または[ReminderMessageData](remindermessagedata.md)に関連付けられている予定表アイテムを表します。
  
```XML
<AssociatedCalendarItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |会議に関連付けられている予定表アイテムを識別します。  <br/> |
|**変更キー** <br/> |会議に関連付けられている予定表アイテムの特定のバージョンを識別します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[MeetingMessage](meetingmessage.md) | [MeetingRequest](meetingrequest.md) | [MeetingResponse](meetingresponse.md) | [MeetingCancellation](meetingcancellation.md) | [ReminderMessageData](remindermessagedata.md)
  
## <a name="remarks"></a>備考

Exchange のビルド番号 15.00.0913.09 以降のバージョンでは、 **ReminderMessageData**要素の子要素として**AssociatedCalendarItemId**の要素を含めることができます。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

