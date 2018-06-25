---
title: GoodThreshold
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GoodThreshold
api_type:
- schema
ms.assetid: 68f607f5-7271-46a6-8ffc-91878185a683
description: GoodThreshold 要素は、適切な提案された会議の時間として修飾するまでの時間のために開くまでの時間が必要な出席者の割合を指定します。
ms.openlocfilehash: 8044cb2b52cb572fad8731253dffa34de9d097fa
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831746"
---
# <a name="goodthreshold"></a>GoodThreshold

**GoodThreshold**要素は、適切な提案された会議の時間として修飾するまでの時間のために開くまでの時間が必要な出席者の割合を指定します。 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
[GoodThreshold](goodthreshold.md)
  
```xml
<GoodThreshold>...</GoodThreshold>
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
|[SuggestionsViewOptions](suggestionsviewoptions.md) <br/> |取得するためのオプションが含まれています会議の情報を提案します。  <br/> 以下は、この要素の XPath です。  <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。 整数型の値は 0 から 50 です。
  
## <a name="remarks"></a>備考

[SuggestionsViewOptions](suggestionsviewoptions.md)要素を使用する場合、この要素が必要です。 **GoodThreshold**要素は、どのような会議は公正と見なされますも決定します。 競合している参加者の割合は、以下より適切なしきい値と、50% よりも高い提案された会議の時間として修飾公平にします。 適切なしきい値を加えた 50 な公平としきい値を定義している割合に相当します。 
  
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

