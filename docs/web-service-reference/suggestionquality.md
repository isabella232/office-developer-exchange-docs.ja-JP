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
ms.openlocfilehash: 3f8c15ccabd03687dc386a0328020cbc0bc802c4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457978"
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[提案](suggestion.md) <br/> |1つの会議時間の提案を表します。  <br/> この要素の XPath 式を次に示します。  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse/SuggestionDayResultArray/SuggestionDayResult[i]/SuggestionArray/Suggestion[i]` <br/> |
   
## <a name="text-value"></a>テキスト値

**SuggestionQuality**値を表すテキスト値が必要です。 指定可能な値は次のいずれかです。 
  
- 推奨される会議時間について、ユーザーとリソース**の 100%** が利用可能です。 
    
- **適切な**使用可能なユーザーとリソースの最小パーセンテージは、 [GoodThreshold](goodthreshold.md)要素の値に50を加えた値と等しいか、それよりも大きくなっています。 
    
- **公正**提案された会議の時間に対して使用できるユーザーとリソースの最大パーセンテージは、 [GoodThreshold](goodthreshold.md)要素の値と50に等しくなります。 **フェア**クオリティ会議の時間の最小値は50% です。 
    
- **低**提案された会議の時間について、ユーザーとリソースの50% 未満が利用可能です。 
    
## <a name="remarks"></a>注釈

**SuggestionQuality**型は、 [Dayquality](dayquality.md)および[MinimumSuggestionQuality](minimumsuggestionquality.md)要素の型でもあります。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[ユーザーの空き時間情報の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

