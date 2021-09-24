---
title: MinimumSuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- MinimumSuggestionQuality
api_type:
- schema
ms.assetid: 3725cbd4-9bc1-4f7d-8929-b2c68cb46114
description: MinimumSuggestionQuality 要素は、応答で返される会議の提案の品質を定義します。
ms.openlocfilehash: c1126158f7a521fbefaf34fda906d60dd15c2af4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510933"
---
# <a name="minimumsuggestionquality"></a>MinimumSuggestionQuality

**MinimumSuggestionQuality** 要素は、応答で返される会議の提案の品質を定義します。 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
[MinimumSuggestionQuality](minimumsuggestionquality.md)
  
```xml
<MinimumSuggestionQuality>...</MinimumSuggestionQuality>
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
|[SuggestionsViewOptions](suggestionsviewoptions.md) <br/> |会議の提案情報を取得するためのオプションが含まれる。  <br/> 次に、この要素の XPath を示します。  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 次の表に、この要素で使用できる値を示します。
  
|**値**|**説明**|
|:-----|:-----|
|**優秀** <br/> |出席者の 0% が、提案された会議時間と競合しています。  <br/> |
|**標準** <br/> |良好と見なされるパーセンテージは [、GoodThreshold 要素を使用して設定](goodthreshold.md) されます。  <br/> |
|**Fair** <br/> |公平と見なされる割合は [、GoodThreshold 要素を使用して設定](goodthreshold.md) されます。  <br/> |
|**悪い** <br/> |出席者の 50% 以上が、推奨される会議時間と競合しています。  <br/> |
   
## <a name="remarks"></a>注釈

[SuggestionsViewOptions 要素を使用する場合は、この要素が](suggestionsviewoptions.md)必要です。 
  
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

