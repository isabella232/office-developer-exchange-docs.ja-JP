---
title: SearchMailboxesResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ddb276c4-6c8a-46ef-a2eb-46b6a0bfce09
description: SearchMailboxesResult 要素には、SearchMailboxes ボックス要求の結果が含まれています。
ms.openlocfilehash: 79d593d99762aedc6290578b5458f9ac3cad3d26
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466704"
---
# <a name="searchmailboxesresult"></a>SearchMailboxesResult

**SearchMailboxesResult**要素には、 **searchmailboxes ボックス**要求の結果が含まれています。 
  
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

[Searchqueries](searchqueries.md)  | [ResultType](resulttype.md)  | [ItemCount](itemcount.md)  | [サイズ (長い)](size-long.md)  | [PageItemCount](pageitemcount.md)  | [Pageitemsize](pageitemsize.md)  | [KeywordStats](keywordstats.md)  | [アイテム (Arrayofsearchプレビュー Itemstype)](items-arrayofsearchpreviewitemstype.md)  | [失敗したメールボックス](failedmailboxes.md)  | [絞り込み条件](refiners.md)  | [MailboxStats](mailboxstats.md)
  
### <a name="parent-elements"></a>親要素

[SearchMailboxesResponseMessage](searchmailboxesresponsemessage.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空にすることができます。  <br/> |false  <br/> |
   

