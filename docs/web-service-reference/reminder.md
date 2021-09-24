---
title: Reminder
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 54dd748a-23a5-4ea2-88f2-b74c68a3c48f
description: Reminder 要素は、タスクまたは予定表アイテムのアラームを指定します。
ms.openlocfilehash: 97b4a1dfb2739ff9ea335bca1e61e264715ced30
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512493"
---
# <a name="reminder"></a>Reminder

**Reminder 要素** は、タスクまたは予定表アイテムのアラームを指定します。 
  
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
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[Reminders](reminders.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

