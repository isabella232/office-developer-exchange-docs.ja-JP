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
description: SuggestionsViewOptions 要素には、会議提案情報を取得するためのオプションが含まれています。
ms.openlocfilehash: f584b19997f98760bd4e438dcd48a5c18cc63e4b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44433995"
---
# <a name="suggestionsviewoptions"></a>SuggestionsViewOptions

**SuggestionsViewOptions**要素には、会議提案情報を取得するためのオプションが含まれています。 
  
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
|[GoodThreshold](goodthreshold.md) <br/> |適切な会議の時間として評価される期間に、期間を開いておく必要がある出席者の割合を指定します。  <br/> |
|[MaximumResultsByDay](maximumresultsbyday.md) <br/> |応答で返される1日あたりの提案された会議時間数を指定します。  <br/> |
|[Maximumnonwork 時間の日付](maximumnonworkhourresultsbyday.md) <br/> |通常の稼働時間外の1日の会議時間について提案される結果の数を指定します。  <br/> |
|[MeetingDurationInMinutes](meetingdurationinminutes.md) <br/> |提案される会議の長さを指定します。  <br/> |
|[MinimumSuggestionQuality](minimumsuggestionquality.md) <br/> |応答で返される会議の提案の品質を指定します。  <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |提案された会議時間に関する詳細情報について、クエリされる期間を指定します。  <br/> |
|[Current会議時間](currentmeetingtime.md) <br/> |提案された会議時間の結果で更新する会議の開始時刻を表します。  <br/> |
|[GlobalObjectId](globalobjectid.md) <br/> |この要素は使用されません。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[GetUserAvailabilityRequest](getuseravailabilityrequest.md) <br/> |ユーザーの空き時間情報を取得するために使用する引数が含まれています。 これはルート要素です。  <br/> この要素の XPath を次に示します。  <br/>  `/GetUserAvailabilityRequest` <br/> |
   
## <a name="remarks"></a>注釈

この要素は必須ではなく、使用されている場合に1回だけ発生します。 [FreeBusyViewOptions](freebusyviewoptions.md)要素の値が null でない場合は、この値を null にすることができます。 
  
> [!NOTE]
> この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)


[ユーザーの空き時間情報の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

