---
title: ActionType (ReminderActionType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 0ffcdcf4-8ea3-483c-bb7f-0cd84126120c
description: ActionType 要素は、アラームに対して実行するアクションを指定します。
ms.openlocfilehash: d78725c75ad13a71d69d7749f0a71cd99d606929
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522258"
---
# <a name="actiontype-reminderactiontype"></a>ActionType (ReminderActionType)

**ActionType 要素** は、アラームに対して実行するアクションを指定します。 
  
```XML
<ActionType> Dismiss | Snooze </ActionType>
```

 **ReminderActionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[ReminderItemAction](reminderitemaction.md)
  
## <a name="text-value"></a>テキスト値

ActionType 要素の **テキスト値** は、アラームに対して実行するアクションを指定します。 [却下] のテキスト **値は** 、アラームを閉じるべきかどうかを示します。 **Snooze のテキスト値は**[、NewReminderTime](newremindertime.md)要素で指定された時刻までアラームを遅延させる必要があります。 
  
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

- [ReminderItemAction](reminderitemaction.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

