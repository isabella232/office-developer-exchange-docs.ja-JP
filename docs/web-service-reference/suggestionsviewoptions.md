---
title: SuggestionsViewOptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionsViewOptions
api_type:
- schema
ms.assetid: bb04ae38-e62d-4a69-a479-8ff326ca726e
description: SuggestionsViewOptions 要素を取得するためのオプションには、会議の情報を提案します。
ms.openlocfilehash: 09ff317ae0b2ebf1eadc89dc3bb1cf5b3ae19dcb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839627"
---
# <a name="suggestionsviewoptions"></a>SuggestionsViewOptions

**SuggestionsViewOptions**要素を取得するためのオプションには、会議の情報を提案します。 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
```xml
<SuggestionsViewOptions>
   <GoodThreshold>...</GoodThreshold>
   <MaximumResultsByDay>...</MaximumResultsByDay>
   <MaximumNonWorkingHourResultsByDay>...</MaximumNonWorkingHourResultsByDay>
   <MeetingDurationInMinutes>...</MeetingDurationInMinutes>
   <MinimumSuggestionQuality>...</MinimumSuggestionQuality>
   <SuggestionIntervalInMinutes>...</SuggestionIntervalInMinutes>
   <DetailedSuggestionsWindow>...</DetailedSuggestionsWindow>
   <CurrentMeetingTime>...</CurrentMeetingTime>
   <GlobalObjectId>...</GlobalObjectId>
</SuggestionsViewOptions>
```

 **SuggestionsViewOptionsType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[GoodThreshold](goodthreshold.md) <br/> |良い提案された会議の時間と判断するまでの時間を開くまでの時間が必要な出席者の割合を指定します。  <br/> |
|[MaximumResultsByDay](maximumresultsbyday.md) <br/> |応答で返される 1 日あたりの推奨される会議の時刻の数を指定します。  <br/> |
|[MaximumNonWorkHourResultsByDay](maximumnonworkhourresultsbyday.md) <br/> |1 日あたりの通常の勤務時間外の時間を満たすために提示された結果の数を指定します。  <br/> |
|[MeetingDurationInMinutes](meetingdurationinminutes.md) <br/> |提案された会議の長さを指定します。  <br/> |
|[MinimumSuggestionQuality](minimumsuggestionquality.md) <br/> |応答で返される会議の提案の品質を指定します。  <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |提案された会議の時間についての詳細情報を照会する期間を指定します。  <br/> |
|[CurrentMeetingTime](currentmeetingtime.md) <br/> |時間の結果を提案された会議を更新する会議の開始時刻を表します。  <br/> |
|[GlobalObjectId](globalobjectid.md) <br/> |この要素は使用されません。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |ユーザーの利用可能時間情報を取得するための引数が含まれています。 これは、ルート要素です。  <br/> 以下は、この要素の XPath です。  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a>備考

この要素は必須ではなく、発生は一度のみを使用する場合。 [FreeBusyViewOptions](freebusyviewoptions.md)要素の値が null でない場合、この値を null にすることができます。 
  
> [!NOTE]
> MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)


[ユーザーの状態を取得します。](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

