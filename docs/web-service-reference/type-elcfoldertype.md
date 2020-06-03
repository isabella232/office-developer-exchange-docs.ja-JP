---
title: Type (ElcFolderType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6faad98f-1a92-4373-bde5-dd12af61765f
description: Type 要素は、アイテム保持ポリシーで使用されるフォルダーの種類を指定します。
ms.openlocfilehash: f6fcc7942a530ada2d6e72c3e38286a7595b09ec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465108"
---
# <a name="type-elcfoldertype"></a>Type (ElcFolderType)

**Type**要素は、アイテム保持ポリシーで使用されるフォルダーの種類を指定します。 
  
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

[New-retentionpolicytag](retentionpolicytag.md)
  
## <a name="text-value"></a>テキスト値

**Type**要素のテキスト値は、アイテム保持ポリシーで使用されるフォルダーの種類です。 テキスト値には、既定のフォルダーの種類を表す次のいずれかの値を指定できます: Calendar、Contacts、DeletedItems、下書き、受信トレイ、JunkEmail、Journal、Notes、送信トレイ、SentItems、Tasks、All、ManagedCustomFolder、RssSubscriptions、SyncIssues、ConversationHistory、Personal、Ableitems、または NonIpmRoot 
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

