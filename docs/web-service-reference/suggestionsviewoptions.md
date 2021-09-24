---
title: SuggestionsViewOptions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SuggestionsViewOptions
api_type:
- schema
ms.assetid: bb04ae38-e62d-4a69-a479-8ff326ca726e
description: SuggestionsViewOptions 要素には、会議の提案情報を取得するためのオプションが含まれている。
ms.openlocfilehash: ba3591b88e581d45c811100a53b0a74e4bb8e010
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59522615"
---
# <a name="suggestionsviewoptions"></a>SuggestionsViewOptions

**SuggestionsViewOptions 要素** には、会議の提案情報を取得するためのオプションが含まれている。 
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[GoodThreshold](goodthreshold.md) <br/> |推奨される会議時間として資格を得る期間を開く必要がある出席者の割合を指定します。  <br/> |
|[MaximumResultsByDay](maximumresultsbyday.md) <br/> |応答で返される 1 日あたりの推奨される会議時間の数を指定します。  <br/> |
|[MaximumNonWorkHourResultsByDay](maximumnonworkhourresultsbyday.md) <br/> |1 日の通常の勤務時間外の会議時間に対して推奨される結果の数を指定します。  <br/> |
|[MeetingDurationInMinutes](meetingdurationinminutes.md) <br/> |提案する会議の長さを指定します。  <br/> |
|[MinimumSuggestionQuality](minimumsuggestionquality.md) <br/> |応答で返される会議の提案の品質を指定します。  <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |推奨される会議時間に関する詳細情報を照会する期間を識別します。  <br/> |
|[CurrentMeetingTime](currentmeetingtime.md) <br/> |推奨される会議時間の結果で更新する会議の開始時刻を表します。  <br/> |
|[GlobalObjectId](globalobjectid.md) <br/> |この要素は使用されません。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |ユーザーの可用性情報を取得するために使用される引数を格納します。 これはルート要素です。  <br/> 次に、この要素の XPath を示します。  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a>注釈

この要素は必須ではなく、使用する場合は 1 回だけ発生します。 [FreeBusyViewOptions](freebusyviewoptions.md)要素の値が null でない場合、この値は null になります。 
  
> [!NOTE]
> この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)


[ユーザーの可用性の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

