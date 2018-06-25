---
title: VotingResponse
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7dae4db5-28d3-4b81-b071-458c814c36b9
description: VotingResponse 要素は、送信された投票を指定します。 この要素があるだけ返信要求メッセージへの応答で、承認への応答ではなく。
ms.openlocfilehash: 865b24a4f7ec1cc7b53d4928b04f071cddf5fbfc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839996"
---
# <a name="votingresponse"></a>VotingResponse

**VotingResponse**要素は、送信された投票を指定します。 この要素があるだけ返信要求メッセージへの応答で、承認への応答ではなく。 
  
```XML
<VotingResponse />
```

 **string**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[VotingInformation](votinginformation.md)
  
## <a name="text-value"></a>テキスト値

**VotingResponse**要素のテキスト値は、票を送信します。 
  
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



[VotingInformation](votinginformation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

