---
title: ReminderType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfaf84eb-271a-4728-84fc-a20205a100bd
description: ReminderType 要素は、返される通知の種類を指定します。
ms.openlocfilehash: 4ac20143bbfb29fb8f962515f2faba224b2f973f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465528"
---
# <a name="remindertype"></a>ReminderType

**ReminderType**要素は、返される通知の種類を指定します。 
  
```XML
<ReminderType> All | Current | Old </ReminderType>
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[GetReminders](getreminders.md)
  
## <a name="text-value"></a>テキスト値

**ReminderType**要素のテキスト値は、返される通知の種類 ( **All**、 **Current**、または**Old**) です。 **All**は、この要素に推奨される値です。 **ReminderType**要素と[Begintime](begintime.md)および[EndTime](endtime-remindermessagedatatype.md)要素の関係の詳細については、「 [getreminders 操作](getreminders-operation.md)」を参照してください。
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetReminders](getreminders.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

