---
title: GetRemindersResponse
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b1c7288-2a98-4142-8961-4d2ebca5c37c
description: GetRemindersResponse 要素は、GetReminders 要求への応答を指定します。
ms.openlocfilehash: 1882ab377365908c0bc272059ab4e007c43d788c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760842"
---
# <a name="getremindersresponse"></a>GetRemindersResponse

**GetRemindersResponse**要素は、 **GetReminders**要求への応答を指定します。 
  
```XML
<GetRemindersResponse>
   <Reminders></Reminders>
</GetRemindersResponse>

```

 **GetRemindersResponseMessageType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[Reminders](reminders.md)
  
### <a name="parent-elements"></a>親要素

[ResponseMessages](responsemessages.md)
  
## <a name="remarks"></a>Remarks

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



[ResponseMessages](responsemessages.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

