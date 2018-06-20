---
title: SuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SuggestionQuality
api_type:
- schema
ms.assetid: 734f1a58-adda-4830-973e-e84bf7b870d5
description: SuggestionQuality 要素は、提案された会議の時間の品質を表します。
ms.openlocfilehash: e67e0149226b36c22cdd00acd78f6582f826dd3e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839624"
---
# <a name="suggestionquality"></a>SuggestionQuality

**SuggestionQuality**要素は、提案された会議の時間の品質を表します。 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[SuggestionsResponse](suggestionsresponse.md)
  
[SuggestionDayResultArray](suggestiondayresultarray.md)
  
[SuggestionDayResult](suggestiondayresult.md)
  
[SuggestionArray](suggestionarray.md)
  
[提案](suggestion.md)
  
[SuggestionQuality](suggestionquality.md)
  
```xml
<SuggestionQuality>Excellent or Good or Fair or Poor</SuggestionQuality>
```

 **SuggestionQuality**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[提案](suggestion.md) <br/> |単一会議の時間を提案します。  <br/> この要素への XPath 式は、次のようにします。  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a>テキスト値

**SuggestionQuality**の値を表す文字列値は、必要があります。 指定可能な値は次のいずれかです。 
  
- **優れた**ユーザーおよびリソースの 100% は、推奨される会議の時刻を使用できます。 
    
- **良い**ユーザーおよびリソースの利用可能な最小の割合は、 [GoodThreshold](goodthreshold.md)要素の値に 50 を加えたよりも同等以上です。 
    
- **フェア**ユーザーおよび提案された会議の時間に利用できるリソースの最大の割合は、 [GoodThreshold](goodthreshold.md)要素の値に 50 を加算した値です。 **公正な**品質会議の時間の最小値は、50% です。 
    
- **低下**ユーザーおよびリソースの 50% 未満の場合は、提案された会議の時間を利用できます。 
    
## <a name="remarks"></a>備考

**SuggestionQuality**型は、また、 [DayQuality](dayquality.md)と[MinimumSuggestionQuality](minimumsuggestionquality.md)の要素の型です。 
  
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

