---
title: MeetingSuggestion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: d6012063-eb67-4e83-a4a6-33482685083f
description: MeetingSuggestion 要素は、提案された会議を指定します。
ms.openlocfilehash: 20523a77fc9fcdf22c837f2e4101ed699e1d4a7b
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532490"
---
# <a name="meetingsuggestion"></a>MeetingSuggestion

**MeetingSuggestion 要素** は、提案された会議を指定します。 
  
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

[出席者](attendees.md)  | [場所](location.md)  | [件名](subject.md)  | [MeetingString](meetingstring.md)  | [StartTime](starttime.md)  | [EndTime](endtime.md)
  
### <a name="parent-elements"></a>親要素

[MeetingSuggestions](meetingsuggestions.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> ||
   

