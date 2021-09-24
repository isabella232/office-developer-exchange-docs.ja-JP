---
title: SearchItemKind
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 89513c26-b751-4619-a300-0ed8f55b0102
description: SearchItemKind 要素は、FindMailboxStatisticsByKeyword 操作で検索されるアイテムの種類を示します。
ms.openlocfilehash: 93803d181f32d88c30ab0fa9a72bb92f22907dde
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59510856"
---
# <a name="searchitemkind"></a>SearchItemKind

**SearchItemKind** 要素は **、FindMailboxStatisticsByKeyword** 操作で検索されるアイテムの種類を示します。 
  
```XML
<SearchItemKind>Email | Meetings | Tasks | Notes | Docs | Journals | Contacts | Im | Voicemail | Faxes | Posts | Rssfeeds</SearchItemKind>
```

 **SearchItemKindType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[MessageTypes](messagetypes.md)
  
## <a name="text-value"></a>テキスト値

**SearchItemKind 要素のテキスト** 値は、キーワードを検索するアイテムの種類です。 次の一覧には **、SearchItemKind** 要素で使用できるテキスト値が含まれます。 
  
- **[電子** メール] - 電子メール メッセージでキーワードを検索します。 
    
- **[会議** ] - 会議でキーワードを検索します。 
    
- **タスク** - タスクがキーワードを検索する方法を示します。 
    
- **[メモ** ] - メモでキーワードを検索します。 
    
- **Docs** - ドキュメントがキーワードを検索する方法を示します。 
    
- **Journals** - キーワードを検索するジャーナルを示します。 
    
- **連絡先** - 連絡先がキーワードを検索する方法を示します。 
    
- **Im** - インスタント メッセージでキーワードを検索します。 
    
- **ボイス** メール - ボイス メールでキーワードを検索します。 
    
- **FAX -** FAX がキーワードを検索する方法を示します。 
    
- **投稿** - 投稿がキーワードで検索されるかどうかを示します。 
    
- **Rssfeeds** - RSS フィードでキーワードを検索します。 
    
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
   

