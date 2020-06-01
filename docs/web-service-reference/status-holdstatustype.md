---
title: 状態 (HoldStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: Status 要素は、メールボックスの保留状態を指定します。
ms.openlocfilehash: cecfdfaf67b00b6f8cf02188e7a4df7062a732e4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459988"
---
# <a name="status-holdstatustype"></a>状態 (HoldStatusType)

**Status**要素は、メールボックスの保留状態を指定します。 
  
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

**Status**要素のテキスト値は、メールボックスの保持状態です。 **Status**要素には、次のリストの値を指定できます。 
  
> NotOnHold-メールボックスは保持されていません。
    
> 保留中-メールボックスは保留中または保留中のどちらかが保留中です。 
    
> OnHold-メールボックスに保留が正常に適用されました。 
    
> PartialHold-一部のメールボックスに対して保留が正常に適用されましたが、すべてのメールボックスに適用されていません。
    
> Failed-保留リストをメールボックスに適用できませんでした。
    
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> ||
   

