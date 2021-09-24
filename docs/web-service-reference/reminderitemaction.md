---
title: ReminderItemAction
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fe67512c-5b15-4f07-8628-74cf873c2d71
description: ReminderItemAction 要素は、アラーム アイテムのアクションを指定します。
ms.openlocfilehash: 7cd6898bb44ecd442a02f162008225d904396ba0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512465"
---
# <a name="reminderitemaction"></a>ReminderItemAction

**ReminderItemAction** 要素は、アラーム アイテムのアクションを指定します。 
  
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
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[ReminderItemActions](reminderitemactions.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

