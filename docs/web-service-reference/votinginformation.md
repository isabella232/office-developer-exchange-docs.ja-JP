---
title: VotingInformation
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 351c8dfe-cf8c-45ba-a07d-d764f8189773
description: VotingInformation 要素は、投票メッセージと承認要求メッセージに関する投票情報を指定します。ここでApproveandRejectare the voting options.
ms.openlocfilehash: 7e5aedddbfe97bba935aa56b3583e2fb8b081320
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59543857"
---
# <a name="votinginformation"></a>VotingInformation

**VotingInformation** 要素は、投票メッセージと承認要求メッセージに関する投票情報を指定します。ここで、"承認" と "拒否" は投票オプションです。 
  
```XML
<VotingInformation
   <UserOptions/>
   <VotingResponse/>
</VotingInformation>
```

 **VotingInformationType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[UserOptions](useroptions.md)  | [VotingResponse](votingresponse.md)
  
### <a name="parent-elements"></a>親要素

[Message](message-ex15websvcsotherref.md)
  
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



[Message](message-ex15websvcsotherref.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

