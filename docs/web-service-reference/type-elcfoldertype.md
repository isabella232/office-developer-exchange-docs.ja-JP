---
title: 型 (ElcFolderType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6faad98f-1a92-4373-bde5-dd12af61765f
description: 型の要素では、リテンション ・ ポリシーで使用されているフォルダーの種類を指定します。
ms.openlocfilehash: f679a9237a577d26d4b28e1b25f3e135f7193903
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839756"
---
# <a name="type-elcfoldertype"></a>型 (ElcFolderType)

**型**の要素では、リテンション ・ ポリシーで使用されているフォルダーの種類を指定します。 
  
```XML
<Type> Calendar | Contacts | DeletedItems | Drafts | Inbox | JunkEmail | Journal | Notes | Outbox | SentItems | Tasks | All | ManagedCustomFolder | RssSubscriptions | SyncIssues | ConversationHistory | Personal | RecoverableItems | NonIpmRoot <Type>
```

 **ElcFolderType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[RetentionPolicyTag](retentionpolicytag.md)
  
## <a name="text-value"></a>テキスト値

**型**の要素のテキスト値は、リテンション ・ ポリシーで使用されているフォルダーの種類です。 テキスト値には、既定のフォルダーの種類を表す次の値のいずれかを指定できます: 予定表、連絡先、DeletedItems、下書き、受信トレイ、JunkEmail、ジャーナル、メモ、送信トレイ、送信済みアイテム、タスク、すべて、ManagedCustomFolder、RssSubscriptions、SyncIssues、ConversationHistory、個人、RecoverableItems、または NonIpmRoot 
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

