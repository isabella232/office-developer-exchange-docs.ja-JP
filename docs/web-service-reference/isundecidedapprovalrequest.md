---
title: IsUndecidedApprovalRequest
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90841617-3b83-4124-8125-0293c9470f4a
description: IsUndecidedApprovalRequest 要素は、承認要求メッセージが処理済みであるかどうかを指定します。
ms.openlocfilehash: 82b4624df5b2fe7ca212fdf76248e1ccfa3a081f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832127"
---
# <a name="isundecidedapprovalrequest"></a>IsUndecidedApprovalRequest

**IsUndecidedApprovalRequest**要素は、承認要求メッセージが処理済みであるかどうかを指定します。 
  
```XML
<IsUndecidedApprovalRequest> true | false </IsUndecidedApprovalRequest>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[ApprovalRequestData](approvalrequestdata.md)
  
## <a name="text-value"></a>テキスト値

**承認要求メッセージが処理済みいない場合、 **IsUndecidedApprovalRequest**要素のテキスト値は** **False**の値は、承認要求が決定されたことを示します。 
  
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



[ApprovalRequestData](approvalrequestdata.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

