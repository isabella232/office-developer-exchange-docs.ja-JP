---
title: SendPrompt
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22cb5a30-75d9-49a8-9d98-255f2e8a722d
description: SendPrompt 要素は、返信のオプションで使用できるアクションの種類を指定します。
ms.openlocfilehash: f3220d957482ea04c46b014cdf1c67025d5ec21a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833346"
---
# <a name="sendprompt"></a>SendPrompt

**SendPrompt**要素は、返信のオプションで使用できるアクションの種類を指定します。 
  
```XML
<SendPrompt> None | Send | VotingOption </SendPrompt>
```

 **SendPromptType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[VotingOptionData](votingoptiondata.md)
  
## <a name="text-value"></a>テキスト値

**SendPrompt**要素のテキスト値は、返信のオプション操作です。 次の表は、この要素の有効な値を一覧します。 
  
****

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |操作はありません。  <br/> |
|送信  <br/> |応答が直ちに送信されます。  <br/> |
|VotingOption  <br/> |承認者は、承認または却下の中にコメントを入力できます。  <br/> |
   
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |True  <br/> |
   
## <a name="see-also"></a>関連項目



[VotingOptionData](votingoptiondata.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

