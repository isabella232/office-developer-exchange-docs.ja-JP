---
title: GroupAttendeeConflictData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GroupAttendeeConflictData
api_type:
- schema
ms.assetid: fd8bf19a-298b-4135-93e8-ead3db7e1142
description: GroupAttendeeConflictData 要素には、使用可能なユーザー数、競合しているユーザーの数、および推奨される会議時間の配布リストの空き時間情報を持っていないユーザーの数についての集約競合情報が含まれています。
ms.openlocfilehash: c75a4e6f8fdff7fb2514f448350fee9f1acb9775
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462930"
---
# <a name="groupattendeeconflictdata"></a>GroupAttendeeConflictData

**GroupAttendeeConflictData**要素には、使用可能なユーザー数、競合しているユーザーの数、および推奨される会議時間の配布リストの空き時間情報を持っていないユーザーの数についての集約競合情報が含まれています。 
  
- [GetUserAvailabilityResponse](getuseravailabilityresponse.md)
- [SuggestionsResponse](suggestionsresponse.md)
- [SuggestionDayResultArray](suggestiondayresultarray.md)
- [SuggestionDayResult](suggestiondayresult.md)
- [SuggestionArray](suggestionarray.md)
- [提案](suggestion.md)
- [AttendeeConflictDataArray](attendeeconflictdataarray.md)
- [GroupAttendeeConflictData](groupattendeeconflictdata.md)
  
```xml
<GroupAttendeeConflictData>
   <NumberOfMembers>...</NumberOfMembers>
   <NumberOfMembersAvailable>...</NumberOfMembersAvailable>
   <NumberOfMembersWithConflict>...</NumberOfMembersWithConflict>
   <NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
</GroupAttendeeConflictData>
```

**GroupAttendeeConflictData**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[NumberOfMembers](numberofmembers.md) <br/> |配布リスト内のユーザー、リソース、ルームの数を表します。  <br/> |
|[NumberOfMembersAvailable](numberofmembersavailable.md) <br/> |提案された会議の時間に使用できる配布リストのメンバーの数を表します。 この要素は、状態が "**フリー**" であるメンバーを表します。  <br/> |
|[NumberOfMembersWithConflict](numberofmemberswithconflict.md) <br/> |提案された会議時間と競合している配布リストメンバーの数を表します。 この要素は、**取り込み中**、 **OOF**、または**仮承諾**状態のメンバーを表します。  <br/> |
|[NumberOfMembersWithNoData](numberofmemberswithnodata.md) <br/> |公開されている空き時間情報データを持たないグループメンバーのうち、提案された会議の時刻と比較するものの数を表します。 この要素は、大きすぎる、またはデータの状態を持た**ない**メンバーを表す配布リストのメンバーを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AttendeeConflictDataArray](attendeeconflictdataarray.md) <br/> |[Getuseravailability 操作](getuseravailability-operation.md)で識別された、クエリを実行した出席者の競合データの配列を格納します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a>注釈

[GetUserAvailabilityRequest](getuseravailabilityrequest.md)内の出席者が配布リストに解決された場合、 **GroupAttendeeConflictData**要素は応答内に存在します。 **GroupAttendeeConflictData**要素は、配布リストのメンバーの3つの状態を示します。使用可能、競合している、またはデータがありません。 配布リストの展開は最大100のメンバーをサポートします。 そのため、 [numberofmembers](numberofmembers.md)要素には最大で100のメンバーを含めることができます。 配布リストの展開は再帰的です。 配布リストに親メンバーシップの合計を100のメンバーまで展開する子配布リストが含まれている場合、子配布リストは展開されず、 [Numberofmemberswithnodata](numberofmemberswithnodata.md)要素数の1つのエントリとしてカウントされます。 子配布リストを展開でき、親メンバーシップの合計が100を超えるメンバーに展開されていない場合は、そのメンバーシップが展開され、メンバー数が**GroupAttendeeConflictData**要素の子要素に追加されます。 
  
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

