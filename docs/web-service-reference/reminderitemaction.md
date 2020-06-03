---
title: ReminderItemAction
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fe67512c-5b15-4f07-8628-74cf873c2d71
description: ReminderItemAction 要素は、アラームアイテムのアクションを指定します。
ms.openlocfilehash: 60722235ed3e73e6a9923df8d3c63a6fc123599a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466228"
---
# <a name="reminderitemaction"></a>ReminderItemAction

**ReminderItemAction**要素は、アラームアイテムのアクションを指定します。 
  
```XML
<ReminderItemAction>
   <ActionType></ActionType>
   <ItemId></ItemId>
   <NewReminderTime></NewReminderTime>
</ReminderItemAction>
```

 **ReminderItemActionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[ActionType (ReminderActionType)](actiontype-reminderactiontype.md)  | [ItemId](itemid.md)  | [NewReminderTime](newremindertime.md)
  
### <a name="parent-elements"></a>親要素

[ReminderItemActions](reminderitemactions.md)
  
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



[ReminderItemActions](reminderitemactions.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

