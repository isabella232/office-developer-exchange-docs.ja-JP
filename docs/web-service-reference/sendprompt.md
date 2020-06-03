---
title: SendPrompt
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 22cb5a30-75d9-49a8-9d98-255f2e8a722d
description: SendPrompt 要素は、投票オプションに対して許可されるアクションの種類を指定します。
ms.openlocfilehash: 98ffc69cdc94c3f7b9c325bee0c1ebaeb407ee96
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462102"
---
# <a name="sendprompt"></a>SendPrompt

**Sendprompt**要素は、投票オプションに対して許可されるアクションの種類を指定します。 
  
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

**Sendprompt**要素のテキスト値は、投票オプションのアクションです。 次の表に、この要素で使用できる値を示します。 
  
****

|**値**|**説明**|
|:-----|:-----|
|なし  <br/> |何も実行しません。  <br/> |
|送信  <br/> |応答はすぐに送信されます。  <br/> |
|VotingOption  <br/> |承認者は、承認または拒否の際にコメントを入力できます。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[VotingOptionData](votingoptiondata.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

