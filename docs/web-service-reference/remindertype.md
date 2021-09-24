---
title: ReminderType
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: bfaf84eb-271a-4728-84fc-a20205a100bd
description: ReminderType 要素は、取得するアラームの種類を指定します。
ms.openlocfilehash: ab10db372efb935b335868f5d212ded84b29e6eb
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518002"
---
# <a name="remindertype"></a>ReminderType

**ReminderType** 要素は、取得するアラームの種類を指定します。 
  
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

**ReminderType** 要素のテキスト値は、すべて、現在、または Old のいずれかである、取得するアラームの **種類です**。 **All** は、この要素の推奨値です。 ReminderType 要素と **BeginTime** 要素と [EndTime](begintime.md)要素 [](endtime-remindermessagedatatype.md)の関係の詳細については [、「GetReminders 操作」を参照してください](getreminders-operation.md)。
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetReminders](getreminders.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

