---
title: SearchQueries
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 67328dab-321b-45ad-929e-cd83e65ad87e
description: SearchQueries 要素には、メールボックス、および検索に関連するクエリの一覧が含まれています。
ms.openlocfilehash: 182f1ba63b4226ea4ff6445ae9f039197dec38a5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833316"
---
# <a name="searchqueries"></a>SearchQueries

**SearchQueries**要素には、メールボックス、および検索に関連するクエリの一覧が含まれています。 
  
```XML
<SearchQueries>
   <MailboxQuery/>
</SearchQueries>
```

 ****
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[MailboxQuery](mailboxquery.md)
  
### <a name="parent-elements"></a>親要素

[SearchMailboxes](searchmailboxes.md) | [SearchMailboxesResult](searchmailboxesresult.md)
  
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
   

