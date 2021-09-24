---
title: SendPrompt
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 22cb5a30-75d9-49a8-9d98-255f2e8a722d
description: SendPrompt 要素は、投票オプションで許可されるアクションの種類を指定します。
ms.openlocfilehash: 32537210aadce91911d1fb5002fbafcaa70aa9ab
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532133"
---
# <a name="sendprompt"></a>SendPrompt

**SendPrompt 要素は**、投票オプションで許可されるアクションの種類を指定します。 
  
```XML
<SendPrompt> None | Send | VotingOption </SendPrompt>
```

 **SendPromptType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[VotingOptionData](votingoptiondata.md)
  
## <a name="text-value"></a>テキスト値

**SendPrompt** 要素のテキスト値は、投票オプション アクションです。 次の表に、この要素に使用できる値を示します。 
  
****

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |アクションなし。  <br/> |
|Send  <br/> |応答は直ちに送信されます。  <br/> |
|VotingOption  <br/> |承認者は、承認または拒否中にコメントを入力できます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[VotingOptionData](votingoptiondata.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

