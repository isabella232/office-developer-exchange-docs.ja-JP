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
description: AssociatedCalendarItemId 要素は、会議のメッセージ、会議の依頼、会議の応答、会議の取り消し、または ReminderMessageData に関連付けられている予定表アイテムを表します。
ms.openlocfilehash: 816372c38243ba0fe5a7606c264dd1c5107350f2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460884"
---
# <a name="associatedcalendaritemid"></a>AssociatedCalendarItemId

**AssociatedCalendarItemId**要素は、[会議のメッセージ](meetingmessage.md)、[会議の依頼](meetingrequest.md)、会議の[応答](meetingresponse.md)、会議の[取り消し](meetingcancellation.md)、または[ReminderMessageData](remindermessagedata.md)に関連付けられている予定表アイテムを表します。
  
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

[会議メッセージ](meetingmessage.md)  | [会議の要求](meetingrequest.md)  | [会議の応答](meetingresponse.md)  | [会議のキャンセル](meetingcancellation.md)  | [ReminderMessageData](remindermessagedata.md)
  
## <a name="remarks"></a>注釈

ビルド番号15.00.0913.09 以降のバージョンの Exchange では、 **ReminderMessageData**要素の子要素として**AssociatedCalendarItemId**要素を含めることができます。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

