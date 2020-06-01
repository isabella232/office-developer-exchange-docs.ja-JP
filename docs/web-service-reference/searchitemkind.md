---
title: SearchItemKind
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 89513c26-b751-4619-a300-0ed8f55b0102
description: SearchItemKind 要素は、FindMailboxStatisticsByKeyword 操作で検索されるアイテムの種類を示します。
ms.openlocfilehash: e0625ac169c3083702494c094da15d38d220fe67
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464001"
---
# <a name="searchitemkind"></a>SearchItemKind

**Searchitemkind**要素は、 **FindMailboxStatisticsByKeyword**操作で検索されるアイテムの種類を示します。 
  
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

**Searchitemkind**要素のテキスト値は、キーワードを検索するアイテムの種類です。 次のリストには、 **Searchitemkind**要素で使用できるテキスト値が含まれています。 
  
- **Email** -キーワードを検索する電子メールメッセージを示します。 
    
- **会議**-キーワードを検索する会議を指定します。 
    
- **タスク**-キーワードを検索するタスクを指定します。 
    
- **メモ**-キーワードに対して notes が検索されることを示します。 
    
- **Docs** -ドキュメントがキーワードで検索されることを示します。 
    
- **ジャーナル**-キーワードに対してジャーナルが検索されることを示します。 
    
- **連絡先**-キーワードを検索することを示します。 
    
- **Im** -キーワードを検索するインスタントメッセージを示します。 
    
- **ボイスメール**-キーワードに対してボイスメールが検索されたことを示します。 
    
- **Fax** -キーワードが検索されたことを示します。 
    
- **投稿**-キーワードに対して投稿が検索されることを示します。 
    
- **Rssfeeds** -RSS フィードがキーワードに対して検索されることを示します。 
    
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
   

