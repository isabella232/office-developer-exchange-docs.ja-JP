---
title: NumberOfMembersWithNoData
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfMembersWithNoData
api_type:
- schema
ms.assetid: 7ca9c57c-9519-442c-a9f4-dca2b0309716
description: NumberOfMembersWithNoData 要素は、提案された会議の時間と比較するための空き/予約済みパブリッシュされたデータを取得して、配布リストのメンバーの数を表します。 この要素は、メンバー配布リストが大きすぎるのか、なしのデータのステータスを持っているメンバーを表します。
ms.openlocfilehash: f73978df47bd8240dd5dabfbbf74523525e3270f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832637"
---
# <a name="numberofmemberswithnodata"></a>NumberOfMembersWithNoData

**NumberOfMembersWithNoData**要素は、提案された会議の時間と比較するための空き/予約済みパブリッシュされたデータを取得して、配布リストのメンバーの数を表します。 この要素は、メンバー配布リストが大きすぎるのか、**なしのデータ**のステータスを持っているメンバーを表します。 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[SuggestionsResponse](suggestionsresponse.md)
  
[SuggestionDayResultArray](suggestiondayresultarray.md)
  
[SuggestionDayResult](suggestiondayresult.md)
  
[SuggestionArray](suggestionarray.md)
  
[提案](suggestion.md)
  
[AttendeeConflictDataArray](attendeeconflictdataarray.md)
  
[GroupAttendeeConflictData](groupattendeeconflictdata.md)
  
[NumberOfMembersWithNoData](numberofmemberswithnodata.md)
  
```xml
<NumberOfMembersWithNoData>...</NumberOfMembersWithNoData>
```

 **int**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GroupAttendeeConflictData](groupattendeeconflictdata.md) <br/> |利用するユーザーの数、競合を持っているユーザーの数および提案された会議の配布リストの利用可能時間情報を持っていないユーザーの数についての集計の競合に関する情報が含まれています。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]/AttendeeConflictDataArray/GroupAttendeeConflictData` <br/> |
   
## <a name="remarks"></a>備考

メールボックスを持っていないユーザー グループのメンバーは、配布リストのメンバーの予定表のデータを持っていないユーザーの例です。 連絡先には、次の理由により**なしのデータ**の状態があります。 
  
- アクセス許可が十分ではありません。
    
- 展開するには、配布リストが大きすぎます。
    
- Active Directory ディレクトリ サービスでは使用できません。
    
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[ユーザーの状態を取得します。](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

