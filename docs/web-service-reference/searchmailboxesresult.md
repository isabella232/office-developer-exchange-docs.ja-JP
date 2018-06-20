---
title: SearchMailboxesResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb276c4-6c8a-46ef-a2eb-46b6a0bfce09
description: SearchMailboxesResult 要素には、SearchMailboxes 要求の結果が含まれています。
ms.openlocfilehash: 93e5837216ef8942b77ac2a91f5ef5f0ad001756
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833300"
---
# <a name="searchmailboxesresult"></a>SearchMailboxesResult

**SearchMailboxesResult**要素には、 **SearchMailboxes**要求の結果が含まれています。 
  
```XML
<SearchMailboxesResult>
   <SearchQueries/>
   <ResultType/>
   <ItemCount/>
   <Size/>
   <PageItemCount/>
   <PageItemSize/>
   <KeywordStats/>
   <Items/>
   <FailedMailboxes/>
   <Refiners/>
   <MailboxStats/>
</SearchMailboxesResult>
```

 **SearchMailboxesResultType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[SearchQueries](searchqueries.md) | [結果](resulttype.md) | [ItemCount](itemcount.md) | [サイズ (長)](size-long.md) | [PageItemCount](pageitemcount.md) | [PageItemSize](pageitemsize.md) | [KeywordStats](keywordstats.md) | [(の項目ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md) | [FailedMailboxes](failedmailboxes.md) | [絞り込み条件](refiners.md) | [MailboxStats](mailboxstats.md)
  
### <a name="parent-elements"></a>親要素

[SearchMailboxesResponseMessage](searchmailboxesresponsemessage.md)
  
## <a name="remarks"></a>備考

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

