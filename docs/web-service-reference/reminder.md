---
title: Reminder
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 54dd748a-23a5-4ea2-88f2-b74c68a3c48f
description: アラーム要素は、タスクまたは予定表アイテムの事前通知を指定します。
ms.openlocfilehash: 71e54d920a169b8060d22bb7d7d294208c344c2e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457488"
---
# <a name="reminder"></a>Reminder

**アラーム**要素は、タスクまたは予定表アイテムの事前通知を指定します。 
  
```XML
<Reminder>
   <Subject></Subject>
   <Location></Location>
   <ReminderTime></ReminderTime>
   <StartDate></StartDate>
   <EndDate></EndDate>
   <ItemId></ItemId>
   <RecurringMasterItemId></RecurringMasterItemId>
   <ReminderGroup></ReminderGroup>
   <UID></UID>
</Reminder>

```

 **ReminderType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[件名](subject.md)  | [場所](location.md)  | [ReminderTime](remindertime.md)  | [StartDate](startdate.md)  | [EndDate (ReminderType)](enddate-remindertype.md)  | [ItemId](itemid.md)  | [RecurringMasterItemId (ItemIdType)](recurringmasteritemid-itemidtype.md)  | [ReminderGroup](remindergroup.md)  | [UID](uid.md)
  
### <a name="parent-elements"></a>親要素

[Reminders](reminders.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[Reminders](reminders.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

