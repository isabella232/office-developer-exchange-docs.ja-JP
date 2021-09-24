---
title: NewReminderTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ff1b6b1c-3557-41d4-8aa6-9528fdb3a21a
description: NewReminderTime 要素は、アラームの新しい時刻を指定します。
ms.openlocfilehash: 9e6cb75396f35f606bcd974e374f24957ee5d1ec
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59515447"
---
# <a name="newremindertime"></a>NewReminderTime

**NewReminderTime** 要素は、アラームの新しい時刻を指定します。 
  
```XML
<NewReminderTime/>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[ReminderItemAction](reminderitemaction.md)
  
## <a name="text-value"></a>テキスト値

**NewReminderTime** 要素のテキスト値は、アラームの新しい時刻です。 **NewReminderTime** 要素は、アラームを遅延するために [ActionType](actiontype-reminderactiontype.md)要素が **Snooze** に設定されている場合に使用されます。 **NewReminderTime** の値は [、GetReminders](getreminders-operation.md)操作によって返される [ReminderTime](remindertime.md)よりも大きくする必要があります。
  
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



[ReminderItemAction](reminderitemaction.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

