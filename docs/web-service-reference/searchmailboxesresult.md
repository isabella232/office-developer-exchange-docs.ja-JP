---
title: SearchMailboxesResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: ddb276c4-6c8a-46ef-a2eb-46b6a0bfce09
description: SearchMailboxesResult 要素には、SearchMailboxes 要求の結果が含まれる。
ms.openlocfilehash: dee1e12a6d083ca3f8d3ddb509775b454e3e8fc0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59534406"
---
# <a name="searchmailboxesresult"></a>SearchMailboxesResult

**SearchMailboxesResult** 要素には **、SearchMailboxes 要求の結果が含** まれる。 
  
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
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[SearchQueries](searchqueries.md)  | [ResultType](resulttype.md)  | [ItemCount](itemcount.md)  | [サイズ (長)](size-long.md)  | [PageItemCount](pageitemcount.md)  | [PageItemSize](pageitemsize.md)  | [KeywordStats](keywordstats.md)  | [アイテム (ArrayOfSearchPreviewItemsType)](items-arrayofsearchpreviewitemstype.md)  | [FailedMailboxes](failedmailboxes.md)  | [絞り込み条件](refiners.md)  | [MailboxStats](mailboxstats.md)
  
### <a name="parent-elements"></a>親要素

[SearchMailboxesResponseMessage](searchmailboxesresponsemessage.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空の場合  <br/> |false  <br/> |
   

