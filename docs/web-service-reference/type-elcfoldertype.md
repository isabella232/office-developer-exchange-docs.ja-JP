---
title: Type (ElcFolderType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 6faad98f-1a92-4373-bde5-dd12af61765f
description: Type 要素は、アイテム保持ポリシーで使用されるフォルダーの種類を指定します。
ms.openlocfilehash: 09e958d56a97b5a169832fe8842276ba0b122243
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517519"
---
# <a name="type-elcfoldertype"></a>Type (ElcFolderType)

**Type 要素** は、アイテム保持ポリシーで使用されるフォルダーの種類を指定します。 
  
```XML
<Type> Calendar | Contacts | DeletedItems | Drafts | Inbox | JunkEmail | Journal | Notes | Outbox | SentItems | Tasks | All | ManagedCustomFolder | RssSubscriptions | SyncIssues | ConversationHistory | Personal | RecoverableItems | NonIpmRoot <Type>
```

 **ElcFolderType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>テキスト値

Type 要素のテキスト **値** は、アイテム保持ポリシーで使用されるフォルダーの種類です。 テキスト値には、予定表、連絡先、DeletedItems、下書き、受信トレイ、JunkEmail、Journal、Notes、Outbox、SentItems、Tasks、All、ManagedCustomFolder、RssSubscriptions、SyncIssues、ConversationHistory、Personal、RecoverableItems、または NonIpmRoot を表す次のいずれかの値を指定できます。 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

