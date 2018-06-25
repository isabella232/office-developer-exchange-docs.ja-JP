---
title: 状態 (HoldStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fee3f1f9-e868-49fa-a554-7ff096964718
description: 状態の要素は、メールボックスの保留状態を指定します。
ms.openlocfilehash: c40dc865d2b305ac86fa40d536e2d516a14260ab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833579"
---
# <a name="status-holdstatustype"></a>状態 (HoldStatusType)

**状態**の要素は、メールボックスの保留状態を指定します。 
  
```XML
<Status> NotOnHold | Pending | OnHold | PartialHold | Failed </Status>
```

 **HoldStatusType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[MailboxHoldStatus](mailboxholdstatus.md)
  
## <a name="text-value"></a>テキスト値

**状態**の要素のテキスト値は、メールボックスの保留状態です。 **状態**の要素は、次の一覧に値を持つことができます。 
  
> NotOnHold - メールボックスは保留状態にします。
    
> 保留中のメールボックスは、保留中のいずれかが配置または保留中のリリースです。 
    
> OnHold - 保留リストは、メールボックスに正常に適用されました。 
    
> PartialHold - 保留リストには、すべてのメールボックスではなく、一部のメールボックスに正しく適用されました。
    
> 保留に失敗しました - メールボックスに適用できませんでした。
    
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> ||
   

