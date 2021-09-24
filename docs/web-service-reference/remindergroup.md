---
title: ReminderGroup
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3e23c2a1-05d8-4fec-897c-f684a5b97e4c
description: ReminderGroup 要素は、予定表アイテムまたはタスクのアラームを指定します。
ms.openlocfilehash: 7ec19505e9237680aee1b3a31332db7fdc4c0dd4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512472"
---
# <a name="remindergroup"></a>ReminderGroup

**ReminderGroup** 要素は、予定表アイテムまたはタスクのアラームを指定します。 
  
```XML
<ReminderGroup> Calendar | Task </ReminderGroup>
```

 **ReminderGroupType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[Reminder](reminder.md)
  
## <a name="text-value"></a>テキスト値

**ReminderGroup** 要素のテキスト値は、アラームのグループの種類です。 Calendar のテキスト **値は** 、アラームが予定表アイテム用である場合に指定します。 Task のテキスト値 **は** 、アラームがタスク アイテム用に指定されます。 
  
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



[Reminder](reminder.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

