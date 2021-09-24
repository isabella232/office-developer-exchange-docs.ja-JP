---
title: CurrentMeetingTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CurrentMeetingTime
api_type:
- schema
ms.assetid: 1ff68154-24b5-465a-a31c-3d3bab0d491e
description: CurrentMeetingTime 要素は、会議出席者が提案した会議の時刻で更新する会議の開始時刻を表します。
ms.openlocfilehash: ef208d232a376d3a7fcffc08db1b8864635c0d0a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59536156"
---
# <a name="currentmeetingtime"></a>CurrentMeetingTime

**CurrentMeetingTime** 要素は、会議出席者が提案した会議の時刻で更新する会議の開始時刻を表します。 
  
[GetUserAvailabilityRequest](getuseravailabilityrequest.md)
  
[SuggestionsViewOptions](suggestionsviewoptions.md)
  
[CurrentMeetingTime](currentmeetingtime.md)
  
```xml
<CurrentMeetingTime>...</CurrentMeetingTime>
```

 **DateTime**
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
   
## <a name="remarks"></a>注釈

この要素は必須ではありません。
  
> [!NOTE]
> この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの /EWS/ ディレクトリにあります。 
  
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

