---
title: ReminderType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bfaf84eb-271a-4728-84fc-a20205a100bd
description: ReminderType 要素は、取得するのにはアラームの種類を指定します。
ms.openlocfilehash: 11739d2068a1009b2840b2169e86b113151cbfa9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833077"
---
# <a name="remindertype"></a>ReminderType

**ReminderType**要素は、取得するのにはアラームの種類を指定します。 
  
```XML
<ReminderType> All | Current | Old </ReminderType>
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[GetReminders](getreminders.md)
  
## <a name="text-value"></a>テキスト値

**ReminderType**要素のテキスト値は、戻るには、**すべて**、**現在**、または**以前**のいずれかのアラームの種類です。 **すべて**は、この要素に推奨される値です。 **ReminderType**要素と[形式の BeginTime](begintime.md)と[終了時刻](endtime-remindermessagedatatype.md)の要素間のリレーションシップの詳細については、 [GetReminders の操作](getreminders-operation.md)を参照してください。
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetReminders](getreminders.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

