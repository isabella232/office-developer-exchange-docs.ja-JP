---
title: NewReminderTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ff1b6b1c-3557-41d4-8aa6-9528fdb3a21a
description: NewReminderTime 要素は、アラームの新しい時刻を指定します。
ms.openlocfilehash: a10f7e481b474501f33dba4c09060766568952b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465955"
---
# <a name="newremindertime"></a>NewReminderTime

**NewReminderTime**要素は、アラームの新しい時刻を指定します。 
  
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

**NewReminderTime**要素のテキスト値は、アラームの新しい時刻です。 **NewReminderTime**要素は、[アラームを遅延させるために[ActionType](actiontype-reminderactiontype.md)要素を再**通知**する] に設定されている場合に使用します。 **NewReminderTime**の値は、 [getreminders 操作](getreminders-operation.md)によって返される[ReminderTime](remindertime.md)より大きい必要があります。
  
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



[ReminderItemAction](reminderitemaction.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

