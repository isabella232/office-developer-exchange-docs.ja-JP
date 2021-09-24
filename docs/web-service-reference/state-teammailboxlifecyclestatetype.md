---
title: State (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: State 要素には、サイト メールボックスに設定されているライフサイクル状態が含まれる。
ms.openlocfilehash: 5189ee8573fd33d2265fd60c47bb40d17b16b8fe
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59538969"
---
# <a name="state-teammailboxlifecyclestatetype"></a>State (TeamMailboxLifecycleStateType)

**State 要素** には、サイト メールボックスに設定されているライフサイクル状態が含まれる。 
  
```XML
<State> Active | Closed | Unlinked | PendingDelete </State>
```

**TeamMailboxLifecycleStateType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[SetTeamMailbox](setteammailbox.md)
  
## <a name="text-value"></a>テキスト値

State 要素のテキスト **値** は、サイト メールボックスに設定されているライフサイクル状態です。 Active のテキスト値 **は** 、サイト メールボックスがアクティブに使用されている状態を示します。 [閉じた] の **テキスト値** は、サイト メールボックスが閉じ、アクティブに使用されていない状態を示します。 [リンク解除] の **テキスト値は** 、サイト メールボックスが Web ベースのコラボレーション環境にリンクされていない状態を示します。  **Active、Closed、** および **PendingDelete** の値は相互に排他的ですが、リンクされていない値は他の値と相互に排他的ではありません。 **PendingDelete のテキスト値は**、サイト メールボックスが削除待ち状態を示します。 サイト メールボックスを PendingDelete として設定するには、その前に **サイト メールボックスを閉じる必要があります**。
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> ||
   

