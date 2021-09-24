---
title: IsOrganizer
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: a31ac268-5061-4272-a433-ffaea2fbcfa9
description: IsOrganizer 要素は、このユーザーが会議の開催者であるかどうかを示すブール値を指定します。
ms.openlocfilehash: a60485146e333e69391dc1771b2c72ef25043a8b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518268"
---
# <a name="isorganizer"></a>IsOrganizer

**IsOrganizer** 要素は、このユーザーが会議の開催者であるかどうかを示すブール値を指定します。 
  
```XML
<IsOrganizer>true | false</IsOrganizer>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |会議メッセージを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

**IsOrganizer** 要素 **のテキスト値が true** の場合は、予定表アイテムまたは会議メッセージがユーザーによって作成されたかどうかを示します。 false の **値は** 、予定表アイテムまたは会議メッセージが作成されていない bv ユーザーを示します。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |types.xsd  <br/> |
|空にできる  <br/> ||
   
## <a name="see-also"></a>関連項目



- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

