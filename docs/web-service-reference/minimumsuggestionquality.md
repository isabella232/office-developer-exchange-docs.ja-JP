---
title: MinimumSuggestionQuality
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MinimumSuggestionQuality
api_type:
- schema
ms.assetid: 3725cbd4-9bc1-4f7d-8929-b2c68cb46114
description: MinimumSuggestionQuality 要素は、応答で返される会議の提案の品質を定義します。
ms.openlocfilehash: ac79682bd761f678f23fc2d698a50fd7704f6fab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832468"
---
# <a name="minimumsuggestionquality"></a>MinimumSuggestionQuality

**MinimumSuggestionQuality**要素は、応答で返される会議の提案の品質を定義します。 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
[MinimumSuggestionQuality](minimumsuggestionquality.md)
  
```xml
<MinimumSuggestionQuality>...</MinimumSuggestionQuality>
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
|[SuggestionsViewOptions](suggestionsviewoptions.md) <br/> |取得するためのオプションが含まれています会議の情報を提案します。  <br/> 以下は、この要素の XPath です。  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 この要素の値を次の表に一覧します。
  
|**値**|**説明**|
|:-----|:-----|
|**たいへん良い** <br/> |出席者の 0% では、提案された会議の時間と競合が存在します。  <br/> |
|**よし** <br/> |良いと考えられている割合は、 [GoodThreshold](goodthreshold.md)要素を使用して設定されています。  <br/> |
|**フェア** <br/> |公平と考えられている割合は、 [GoodThreshold](goodthreshold.md)要素を使用して設定されています。  <br/> |
|**低下** <br/> |50% 以上の参加者の提案された会議の時間との競合があります。  <br/> |
   
## <a name="remarks"></a>備考

[SuggestionsViewOptions](suggestionsviewoptions.md)要素を使用する場合、この要素が必要です。 
  
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

