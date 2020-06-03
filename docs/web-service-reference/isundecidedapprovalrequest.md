---
title: Is未確認 Dedapprovalrequest
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 90841617-3b83-4124-8125-0293c9470f4a
description: Is未確認の Dedapprovalrequest 要素は、承認要求メッセージが処理されたかどうかを指定します。
ms.openlocfilehash: 0949cf64b8583c4b3fa5a1700475f01cc480f69f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458174"
---
# <a name="isundecidedapprovalrequest"></a>Is未確認 Dedapprovalrequest

**Is未確認の Dedapprovalrequest**要素は、承認要求メッセージが処理されたかどうかを指定します。 
  
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

承認要求メッセージが処理されていない場合は、 **is不明な Dedapprovalrequest**要素のテキスト値は**true**です。 値が**false**の場合は、承認要求が決定されたことを示します。 
  
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



[ApprovalRequestData](approvalrequestdata.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

