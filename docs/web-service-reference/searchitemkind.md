---
title: SearchItemKind
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 89513c26-b751-4619-a300-0ed8f55b0102
description: SearchItemKind 要素は、FindMailboxStatisticsByKeyword 操作のために検索される項目の種類を示します。
ms.openlocfilehash: 1c099fc49ec882c1672b265ff0e3aa2c71c5f95b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833298"
---
# <a name="searchitemkind"></a>SearchItemKind

**SearchItemKind**要素は、 **FindMailboxStatisticsByKeyword**操作のために検索される項目の種類を示します。 
  
```XML
<SearchItemKind>Email | Meetings | Tasks | Notes | Docs | Journals | Contacts | Im | Voicemail | Faxes | Posts | Rssfeeds</SearchItemKind>
```

 **SearchItemKindType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

[MessageTypes](messagetypes.md)
  
## <a name="text-value"></a>テキスト値

**SearchItemKind**要素のテキスト値は、キーワードの検索対象となる項目の種類です。 次の一覧には、 **SearchItemKind**要素で使用できるテキストの値が含まれています。 
  
- **電子メール**には、キーワードは、電子メール メッセージを検索することを示します。 
    
- **会議**では、キーワードの会議を検索することを示します。 
    
- **タスク**では、キーワードは、タスクを検索することを示します。 
    
- **ノート**には、キーワードの注釈を検索することを示します。 
    
- **ドキュメント**では、キーワードのドキュメントを検索することを示します。 
    
- **仕訳帳**には、キーワードは、仕訳帳を検索することを示します。 
    
- **連絡先**には、キーワードの連絡先を検索することを示します。 
    
- **Im**のでは、インスタント メッセージのキーワードは検索されることを示します。 
    
- **ボイスメール**のでは、ボイス ・ メールでキーワードが検索されることを示します。 
    
- **Fax**には、キーワードは、fax メッセージを検索することを示します。 
    
- **投稿**を - には、キーワードの投稿を検索することを示します。 
    
- **Rssfeeds**では、キーワードの RSS フィードを検索することを示します。 
    
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
   

