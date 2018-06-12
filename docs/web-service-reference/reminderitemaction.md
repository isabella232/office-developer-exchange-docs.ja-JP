---
title: ReminderItemAction
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fe67512c-5b15-4f07-8628-74cf873c2d71
description: ReminderItemAction 要素は、アラームのアイテムのアクションを指定します。
ms.openlocfilehash: f44e8d354aedca2c1f950238d87ab5c2d6387954
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833069"
---
# <a name="reminderitemaction"></a>ReminderItemAction

**ReminderItemAction**要素は、アラームのアイテムのアクションを指定します。 
  
```XML
<ReminderItemAction>
   <ActionType></ActionType>
   <ItemId></ItemId>
   <NewReminderTime></NewReminderTime>
</ReminderItemAction>
```

 **ReminderItemActionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[ファイアウォール (ReminderActionType)](actiontype-reminderactiontype.md) | [アイテム Id](itemid.md) | [NewReminderTime](newremindertime.md)
  
### <a name="parent-elements"></a>親要素

[ReminderItemActions](reminderitemactions.md)
  
## <a name="remarks"></a>Remarks

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[ReminderItemActions](reminderitemactions.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

