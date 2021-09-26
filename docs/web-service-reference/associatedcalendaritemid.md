---
title: AssociatedCalendarItemId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- AssociatedCalendarItemId
api_type:
- schema
ms.assetid: 5b29898c-ea59-4e6a-914c-c011ec754032
description: AssociatedCalendarItemId 要素は、MeetingMessage、MeetingRequest、MeetingResponse、MeetingCancellation、または ReminderMessageData に関連付けられている予定表アイテムを表します。
ms.openlocfilehash: 5a51c5e3e43a25ebe676bc85e80c2a6ab3705c4d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543689"
---
# <a name="associatedcalendaritemid"></a>AssociatedCalendarItemId

**AssociatedCalendarItemId** 要素は [、MeetingMessage、MeetingRequest、MeetingResponse、MeetingCancellation、](meetingrequest.md)または [ReminderMessageData](remindermessagedata.md)に関連付けられている予定表アイテムを表します。 [](meetingmessage.md) [](meetingresponse.md) [](meetingcancellation.md)
  
```XML
<AssociatedCalendarItemId Id="" ChangeKey=""/>
```

 **ItemIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**Id** <br/> |会議に関連付けられている予定表アイテムを識別します。  <br/> |
|**ChangeKey** <br/> |会議に関連付けられている予定表アイテムの特定のバージョンを識別します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[MeetingMessage](meetingmessage.md)  | [MeetingRequest](meetingrequest.md)  | [MeetingResponse](meetingresponse.md)  | [MeetingCancellation](meetingcancellation.md)  | [ReminderMessageData](remindermessagedata.md)
  
## <a name="remarks"></a>注釈

ビルド番号 15.00.0913.09 から始まる Exchange のバージョンには **、ReminderMessageData** 要素の子要素として **AssociatedCalendarItemId** 要素を含めできます。 
  
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

