---
title: State (TeamMailboxLifecycleStateType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3b1bc531-6988-41c3-9aad-3f5ad5b732a9
description: State 要素には、サイトメールボックスに設定されているライフサイクル状態が含まれます。
ms.openlocfilehash: 597946b48649d997f8dd57823b4e0fcc091a6f84
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465164"
---
# <a name="state-teammailboxlifecyclestatetype"></a>State (TeamMailboxLifecycleStateType)

**State**要素には、サイトメールボックスに設定されているライフサイクル状態が含まれます。 
  
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

**State**要素のテキスト値は、サイトメールボックスに設定されているライフサイクル状態です。 **Active**のテキスト値は、サイトメールボックスがアクティブに使用されていることを示します。 テキスト値**closed**は、サイトメールボックスが閉じられていて、使用中ではないことを示します。 **リンク**のないテキスト値は、サイトメールボックスが web ベースのグループ作業環境にリンクされていないことを示します。 **アクティブ**、**クローズ**、および**PendingDelete**の値は相互に排他的ですが、**リンク**されていない値は他の値を相互排他的にすることはできません。 テキスト値の**PendingDelete**は、サイトメールボックスが削除を保留していることを示します。 サイトメールボックスは、 **PendingDelete**として設定する前に閉じる必要があります。
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> ||
   

