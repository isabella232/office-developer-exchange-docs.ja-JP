---
title: Status (HoldStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: Status 要素は、メールボックスの保留状態を指定します。
ms.openlocfilehash: a055dde61ae52c266f2349036c881d2b00557171
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59521236"
---
# <a name="status-holdstatustype"></a>Status (HoldStatusType)

**Status 要素** は、メールボックスの保留状態を指定します。 
  
```XML
<Status> NotOnHold | Pending | OnHold | PartialHold | Failed </Status>
```

 **HoldStatusType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[MailboxHoldStatus](mailboxholdstatus.md)
  
## <a name="text-value"></a>テキスト値

Status 要素のテキスト **値** は、メールボックスの保留状態です。 **Status 要素には**、次の一覧の値を指定できます。 
  
> NotOnHold - メールボックスが保留ではありません。
    
> Pending - メールボックスは保留または保留状態で解放されています。 
    
> OnHold - 保留はメールボックスに正常に適用されました。 
    
> PartialHold - 保留は一部のメールボックスに正常に適用されましたが、すべてのメールボックスには適用されません。
    
> Failed - 保持がメールボックスに適用できなかった。
    
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> ||
   

