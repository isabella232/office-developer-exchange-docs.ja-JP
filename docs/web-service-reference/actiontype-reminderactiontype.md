---
title: ファイアウォール (ReminderActionType)
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0ffcdcf4-8ea3-483c-bb7f-0cd84126120c
description: ファイアウォールの要素では、アラームを実行するアクションを指定します。
ms.openlocfilehash: 361259f733756995fae2c2c2390013a728e475a4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759269"
---
# <a name="actiontype-reminderactiontype"></a>ファイアウォール (ReminderActionType)

**ファイアウォール**の要素では、アラームを実行するアクションを指定します。 
  
```XML
<ActionType> Dismiss | Snooze </ActionType>
```

 **ReminderActionType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[ReminderItemAction](reminderitemaction.md)
  
## <a name="text-value"></a>テキスト値

**ファイアウォール**の要素のテキスト値は、アラームを実行するアクションを指定します。 **アラームを消す**は、テキスト値では、アラームを終了することを示します。 **再通知**のテキスト値では、アラームを[NewReminderTime](newremindertime.md)要素で指定された時刻まで遅延するかを示します。 
  
## <a name="remarks"></a>備考

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

- [ReminderItemAction](reminderitemaction.md)
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

