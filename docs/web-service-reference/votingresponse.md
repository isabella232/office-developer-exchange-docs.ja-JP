---
title: VotingResponse
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7dae4db5-28d3-4b81-b071-458c814c36b9
description: VotingResponse 要素は、送信される投票を指定します。 この要素は、承認に対する応答に対してではなく、投票要求メッセージへの応答にのみ存在します。
ms.openlocfilehash: ed7caff79d1ff2946800630c167350fe866e29dc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466466"
---
# <a name="votingresponse"></a>VotingResponse

**VotingResponse**要素は、送信される投票を指定します。 この要素は、承認に対する応答に対してではなく、投票要求メッセージへの応答にのみ存在します。 
  
```XML
<VotingResponse />
```

 **string**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[VotingInformation](votinginformation.md)
  
## <a name="text-value"></a>テキスト値

**VotingResponse**要素のテキスト値は、送信される投票です。 
  
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



[VotingInformation](votinginformation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

