---
title: AttendeeConflictDataArray
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AttendeeConflictDataArray
api_type:
- schema
ms.assetid: 1d758547-28c5-4649-8334-427480c282d6
description: AttendeeConflictDataArray 要素には、GetUserAvailability 操作で識別された、クエリを実行した出席者の競合データの配列が含まれています。
ms.openlocfilehash: 770e8c00ca248ec3562180dc9d3626fd5b58f4d9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455801"
---
# <a name="attendeeconflictdataarray"></a>AttendeeConflictDataArray

**AttendeeConflictDataArray**要素には、 [getuseravailability 操作](getuseravailability-operation.md)で識別された、クエリを実行した出席者の競合データの配列が含まれています。
  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
- [SuggestionsResponse](suggestionsresponse.md)
  
- [SuggestionDayResultArray](suggestiondayresultarray.md)
  
- [SuggestionDayResult](suggestiondayresult.md)
  
- [SuggestionArray](suggestionarray.md)
  
- [提案](suggestion.md)
  
- [AttendeeConflictDataArray](attendeeconflictdataarray.md)
  
```xml
<ArrayOfAttendeeConflictData>
   <UnknownAttendeeConflictData>...</UnknownAttendeeConflictData>
   <IndividualAttendeeConflictData>...</IndividualAttendeeConflictData>
   <TooBigGroupAttendeeConflictData>...</TooBigGroupAttendeeConflictData>
   <GroupAttendeeConflictData>...</GroupAttendeeConflictData>
</ArrayOfAttendeeConflictData>
```

 **ArrayOfAttendeeConflictData**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[UnknownAttendeeConflictData](unknownattendeeconflictdata.md) <br/> |非解決の出席者またはユーザー、配布リスト、または連絡先ではない出席者を表します。  <br/> |
|[IndividualAttendeeConflictData](individualattendeeconflictdata.md) <br/> |[提案](suggestion.md)要素で特定された会議の時間と同時に発生する時間枠のユーザーまたは連絡先の空き時間状態を格納します。  <br/> |
|[TooBigGroupAttendeeConflictData](toobiggroupattendeeconflictdata.md) <br/> |展開するには大きすぎる配布リストとして解決された出席者を表します。  <br/> |
|[GroupAttendeeConflictData](groupattendeeconflictdata.md) <br/> |利用可能なユーザー数、競合しているユーザーの数、および推奨される会議時間の配布リストに空き時間情報を持たないユーザーの数についての集約競合情報を格納します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[提案](suggestion.md) <br/> |1つの会議時間の提案を表します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="remarks"></a>注釈

**AttendeeConflictDataArray**の各要素の位置は、 [MailboxDataArray](mailboxdataarray.md)要素の中でクエリを行った出席者の位置に対応します。 クエリを行った各出席者は、 **AttendeeConflictDataArray**子要素のいずれかに対応している必要があります。 これらの要素は、[提案](suggestion.md)要素で特定された会議の推奨時間との単一の競合を表します。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserAvailability 操作](getuseravailability-operation.md) 
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [ユーザーの空き時間情報の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

