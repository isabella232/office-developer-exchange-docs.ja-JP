---
title: IsUndecidedApprovalRequest
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 90841617-3b83-4124-8125-0293c9470f4a
description: IsUndecidedApprovalRequest 要素は、承認要求メッセージが処理されたかどうかを指定します。
ms.openlocfilehash: 5204793490015bd2999322c0f029445c7df91e02
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59511414"
---
# <a name="isundecidedapprovalrequest"></a>IsUndecidedApprovalRequest

**IsUndecidedApprovalRequest** 要素は、承認要求メッセージが処理されたかどうかを指定します。 
  
```XML
<IsUndecidedApprovalRequest> true | false </IsUndecidedApprovalRequest>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[ApprovalRequestData](approvalrequestdata.md)
  
## <a name="text-value"></a>テキスト値

承認要求メッセージが処理されていない **場合、IsUndecidedApprovalRequest** 要素のテキスト値は true です。  false の **値は** 、承認要求が決定されたかどうかを示します。 
  
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



[ApprovalRequestData](approvalrequestdata.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

