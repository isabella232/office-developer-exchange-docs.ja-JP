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
description: GroupAttendeeConflictData 要素にはでの利用の競合を持っているユーザーの数と、配布に利用可能時間情報を持たないユーザーの数を一覧表示するユーザーの数についての集計の競合に関する情報が含まれます、ミーティング時間を提示します。
ms.openlocfilehash: 382b4d866c95de98bd444cd6226d71813889d4f4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831757"
---
# <a name="groupattendeeconflictdata"></a>GroupAttendeeConflictData

**GroupAttendeeConflictData**要素には、使用可能であるユーザーの数、競合を持っているユーザーの数および配布リストの利用可能時間情報を持っていないユーザーの数についての集計の競合に関する情報が含まれています。提案された会議の時間です。 
  
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

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[NumberOfMembers](numberofmembers.md) <br/> |ユーザー、リソース、およびパブリック フォルダーの配布リストの数を表します。  <br/> |
|[NumberOfMembersAvailable](numberofmembersavailable.md) <br/> |提案された会議の時間を利用した配布リストのメンバーの数を表します。 この要素は、対象となる状態は、**無料**のメンバーを表します。  <br/> |
|[NumberOfMembersWithConflict](numberofmemberswithconflict.md) <br/> |提案された会議の時間との競合を持つ配布リストのメンバーの数を表します。 この要素では、**ビジー**、**不在時**、または**仮承諾**のステータスを持っているメンバーを表します。  <br/> |
|[NumberOfMembersWithNoData](numberofmemberswithnodata.md) <br/> |提案された会議の時間と比較するための空き/予約済みパブリッシュされたデータを持っていないグループ メンバーの数を表します。 この要素は、メンバー配布リストが大きすぎるのか、**なしのデータ**のステータスを持っているメンバーを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AttendeeConflictDataArray](attendeeconflictdataarray.md) <br/> |[GetUserAvailability 操作](getuseravailability-operation.md)で指定されたクエリを実行した出席者のために競合データの配列が含まれています。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray` <br/> |
   
## <a name="remarks"></a>備考

**GroupAttendeeConflictData**要素は、 [GetUserAvailabilityRequest](getuseravailabilityrequest.md)の出席者が配布リストを解決するときの応答であります。 **GroupAttendeeConflictData**要素は、配布リストのメンバーの 3 つの状態を識別: 利用可能な競合した場合、またはデータがありません。 配布リストの展開では、最大 100 個のメンバーをサポートします。 したがって、 [NumberOfMembers](numberofmembers.md)要素は、最大 100 のメンバーを含めることができます。 配布リストの展開は、再帰的です。 配布リストには、100 を超えるメンバーを親の合計のメンバーシップを展開する子の配布リストが含まれている、子の配布リストは展開されていないと、 [NumberOfMembersWithNoData](numberofmemberswithnodata.md)の要素数の 1 つのエントリとしてカウントされます。 子の配布リストを展開することができます、100 を超えるメンバーを親の合計のメンバーシップを展開しない場合は、そのメンバーシップは展開し、メンバー数は、 **GroupAttendeeConflictData**要素の子要素に追加されます。 
  
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

