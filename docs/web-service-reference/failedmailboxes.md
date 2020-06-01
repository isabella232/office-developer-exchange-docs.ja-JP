---
title: 失敗したメールボックス
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f34fb6f6-057e-4ae3-8e10-bc92112eafba
description: Failed メールボックス要素は、検索で失敗したメールボックスの配列を指定します。
ms.openlocfilehash: 10f10d3f2ac4379d7ddcb3a13019d17a17bb676a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461955"
---
# <a name="failedmailboxes"></a><span data-ttu-id="93800-103">失敗したメールボックス</span><span class="sxs-lookup"><span data-stu-id="93800-103">FailedMailboxes</span></span>

<span data-ttu-id="93800-104">Failed**メールボックス**要素は、検索で失敗したメールボックスの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="93800-104">The **FailedMailboxes** element specifies an array of mailboxes that failed on search.</span></span> 
  
```XML
<FailedMailboxes>
    <FailedMailbox/>
<FailedMailboxes>
```

 <span data-ttu-id="93800-105">**ArrayOfFailedSearchMailboxesType**</span><span class="sxs-lookup"><span data-stu-id="93800-105">**ArrayOfFailedSearchMailboxesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93800-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="93800-106">Attributes and elements</span></span>

<span data-ttu-id="93800-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="93800-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93800-108">属性</span><span class="sxs-lookup"><span data-stu-id="93800-108">Attributes</span></span>

<span data-ttu-id="93800-109">なし。</span><span class="sxs-lookup"><span data-stu-id="93800-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="93800-110">子要素</span><span class="sxs-lookup"><span data-stu-id="93800-110">Child elements</span></span>

|<span data-ttu-id="93800-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="93800-111">**Element**</span></span>|<span data-ttu-id="93800-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="93800-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93800-113">失敗したメールボックス</span><span class="sxs-lookup"><span data-stu-id="93800-113">FailedMailbox</span></span>](failedmailbox.md) <br/> |<span data-ttu-id="93800-114">検索で失敗したメールボックスのエラーメッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="93800-114">Specifies the error message for a mailbox that failed on search.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="93800-115">親要素</span><span class="sxs-lookup"><span data-stu-id="93800-115">Parent elements</span></span>

|<span data-ttu-id="93800-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="93800-116">**Element**</span></span>|<span data-ttu-id="93800-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="93800-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93800-118">SearchMailboxesResult</span><span class="sxs-lookup"><span data-stu-id="93800-118">SearchMailboxesResult</span></span>](searchmailboxesresult.md) <br/> |<span data-ttu-id="93800-119">**Searchmailboxes ボックス**要求の結果が含まれます。</span><span class="sxs-lookup"><span data-stu-id="93800-119">Contains the result of the **SearchMailboxes** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="93800-120">注釈</span><span class="sxs-lookup"><span data-stu-id="93800-120">Remarks</span></span>

<span data-ttu-id="93800-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="93800-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="93800-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="93800-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93800-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="93800-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93800-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="93800-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="93800-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="93800-125">Schema Name</span></span>  <br/> |<span data-ttu-id="93800-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="93800-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="93800-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="93800-127">Validation File</span></span>  <br/> |<span data-ttu-id="93800-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="93800-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="93800-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="93800-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="93800-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="93800-130">See also</span></span>



- [<span data-ttu-id="93800-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="93800-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

