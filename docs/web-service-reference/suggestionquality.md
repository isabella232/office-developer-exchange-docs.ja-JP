---
title: SuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- SuggestionQuality
api_type:
- schema
ms.assetid: 734f1a58-adda-4830-973e-e84bf7b870d5
description: SuggestionQuality 要素は、提案された会議時間の品質を表します。
ms.openlocfilehash: 4d8a504e60e8f043bfb120080a89733e78b16b9e
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531553"
---
# <a name="suggestionquality"></a>SuggestionQuality

**SuggestionQuality 要素** は、提案された会議時間の品質を表します。 
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[提案](suggestion.md) <br/> |1 つの会議時間の提案を表します。  <br/> 次に、この要素の XPath 式を示します。  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a>テキスト値

**SuggestionQuality** 値を表すテキスト値が必要です。 指定可能な値は次のいずれかです。 
  
- **優** れた 100% のユーザーとリソースが、推奨される会議時間に利用できます。 
    
- **良い** 使用可能なユーザーとリソースの最小割合は [、GoodThreshold](goodthreshold.md) 要素の値に 50 を加えた値以上です。 
    
- **Fair** 推奨される会議時間に使用できるユーザーとリソースの最大割合は [、GoodThreshold](goodthreshold.md) 要素の値に 50 を加えた値と等しくなります。 公正な品質の会議 **時間の** 最小値は 50% です。 
    
- **貧しい** 推奨される会議時間に使用できるユーザーとリソースの 50% 未満。 
    
## <a name="remarks"></a>注釈

**SuggestionQuality 型** は [、DayQuality](dayquality.md)要素と [MinimumSuggestionQuality 要素の型](minimumsuggestionquality.md)です。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[ユーザーの可用性の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

