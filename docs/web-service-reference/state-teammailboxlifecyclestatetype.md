---
title: 状態 (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: State 要素には、サイトのメールボックスに設定されているライフ サイクル状態が含まれています。
ms.openlocfilehash: accd70d36cc34e7364387b98a2e94c56b91f012f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833571"
---
# <a name="state-teammailboxlifecyclestatetype"></a>状態 (TeamMailboxLifecycleStateType)

**State**要素には、サイトのメールボックスに設定されているライフ サイクル状態が含まれています。 
  
```XML
<State> Active | Closed | Unlinked | PendingDelete </State>
```

**TeamMailboxLifecycleStateType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[SetTeamMailbox](setteammailbox.md)
  
## <a name="text-value"></a>テキスト値

**状態**の要素のテキスト値は、サイトのメールボックスに設定されているライフ サイクル状態です。 **作業中**のテキスト値は、サイトのメールボックスが使用中でことを示します。 **終了**のテキスト値は、サイトのメールボックスが閉じられたアクティブな使用されていないことを示します。 **リンクのない**のテキスト値は、サイトのメールボックスが、web ベースのコラボレーション環境にリンクされていないことを示します。 **アクティブ**、**終了**、および**PendingDelete**の値は、相互に排他的ですが、**リンクのない**値は互いに他の値を除く。 **PendingDelete**のテキスト値は、サイトのメールボックスが削除は保留されていることを示します。 サイトのメールボックスには**PendingDelete**に設定することができます前に閉じる。
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> ||
   

