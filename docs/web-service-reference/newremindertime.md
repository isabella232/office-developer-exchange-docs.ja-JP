---
title: NewReminderTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ff1b6b1c-3557-41d4-8aa6-9528fdb3a21a
description: NewReminderTime 要素は、新しいアラームの時刻を指定します。
ms.openlocfilehash: 9f3f509942c673c916cc646cd9519240aef6ea06
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832531"
---
# <a name="newremindertime"></a>NewReminderTime

**NewReminderTime**要素は、新しいアラームの時刻を指定します。 
  
```XML
<NewReminderTime/>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[ReminderItemAction](reminderitemaction.md)
  
## <a name="text-value"></a>テキスト値

**NewReminderTime**要素のテキスト値とは、新しいアラームの時刻です。 **NewReminderTime**要素は、[ファイアウォール](actiontype-reminderactiontype.md)の要素に設定すると**再通知**、アラームを延期するために使用されます。 **NewReminderTime**の値は、 [GetReminders 操作](getreminders-operation.md)によって返される[ReminderTime](remindertime.md)よりも大きい必要があります。
  
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



[ReminderItemAction](reminderitemaction.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

