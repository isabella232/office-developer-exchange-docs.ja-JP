---
title: MeetingSuggestion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d6012063-eb67-4e83-a4a6-33482685083f
description: 会議提案要素は、提案された会議を指定します。
ms.openlocfilehash: 132ed907886c0ee9f3c4f46cc835d4b4fc6aa621
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466312"
---
# <a name="meetingsuggestion"></a>MeetingSuggestion

会議**提案**要素は、提案された会議を指定します。 
  
```XML
<MeetingSuggestion>
   <Attendees/>
   <Location/>
   <Subject/>
   <MeetingString/>
   <StartTime/>
   <EndTime/>
</MeetingSuggestion>
```

 **MeetingSuggestionType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[出席者](attendees.md)  | [場所](location.md)  | [件名](subject.md)  | [会議の文字列](meetingstring.md)  | [StartTime](starttime.md)  | [EndTime](endtime.md)
  
### <a name="parent-elements"></a>親要素

[MeetingSuggestions](meetingsuggestions.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   

