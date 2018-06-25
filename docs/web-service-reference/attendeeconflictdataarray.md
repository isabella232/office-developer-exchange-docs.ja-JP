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
description: AttendeeConflictDataArray 要素には、GetUserAvailability 操作で指定されたクエリを実行した出席者のための競合データの配列が含まれています。
ms.openlocfilehash: 169312b8a3d37c014ba58fbfe094d786b134fc90
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759459"
---
# <a name="attendeeconflictdataarray"></a>AttendeeConflictDataArray

**AttendeeConflictDataArray**要素には、 [GetUserAvailability の操作](getuseravailability-operation.md)で指定されたクエリを実行した出席者のための競合データの配列が含まれています。
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[UnknownAttendeeConflictData](unknownattendeeconflictdata.md) <br/> |解決できない出席者やユーザー、配布リスト、または取引先担当者ではない出席者を表します。  <br/> |
|[IndividualAttendeeConflictData](individualattendeeconflictdata.md) <br/> |示したと同時に発生するタイム ・ ウィンドウのユーザーまたは連絡先の空き時間状況が含まれています会議[提案](suggestion.md)の要素で指定された時刻。  <br/> |
|[TooBigGroupAttendeeConflictData](toobiggroupattendeeconflictdata.md) <br/> |配布リストを展開するのには大きすぎるとして解決する出席者を表します。  <br/> |
|[GroupAttendeeConflictData](groupattendeeconflictdata.md) <br/> |可能なユーザー数、競合を持っているユーザーの数および提案された会議の配布リストの利用可能時間情報を持っていないユーザーの数についての集計の競合に関する情報が含まれています。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[提案](suggestion.md) <br/> |単一会議の時間を提案します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="remarks"></a>備考

**AttendeeConflictDataArray**内の各要素の位置は、 [MailboxDataArray](mailboxdataarray.md)要素でクエリを実行した出席者の位置に対応します。 各クエリを実行した出席者は、 **AttendeeConflictDataArray**の子要素の 1 つに対応しなければなりません。 これらの要素は、[提案](suggestion.md)の要素で識別される候補の会議の時刻に 1 つの競合を表します。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserAvailability 操作](getuseravailability-operation.md) 
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [ユーザーの状態を取得します。](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

