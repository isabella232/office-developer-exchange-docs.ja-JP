---
title: 失敗したメールボックス
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d4c9816-54bb-4932-b4ba-f057c9173a1a
description: 失敗した Mailbox 要素は、検索で失敗したメールボックスのエラーメッセージを指定します。
ms.openlocfilehash: 404084bc342eb555db61c4216e936bee6ced9c36
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461962"
---
# <a name="failedmailbox"></a><span data-ttu-id="f8348-103">失敗したメールボックス</span><span class="sxs-lookup"><span data-stu-id="f8348-103">FailedMailbox</span></span>

<span data-ttu-id="f8348-104">失敗した**mailbox**要素は、検索で失敗したメールボックスのエラーメッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="f8348-104">The **FailedMailbox** element specifies the error message for a mailbox that failed on search.</span></span> 
  
```XML
<FailedMailbox>
    <Mailbox/>
    <ErrorCode/>
    <ErrorMessage/>
    <IsArchive/>
</FailedMailbox>
```

 <span data-ttu-id="f8348-105">**FailedSearchMailboxType**</span><span class="sxs-lookup"><span data-stu-id="f8348-105">**FailedSearchMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f8348-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f8348-106">Attributes and elements</span></span>

<span data-ttu-id="f8348-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f8348-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f8348-108">属性</span><span class="sxs-lookup"><span data-stu-id="f8348-108">Attributes</span></span>

<span data-ttu-id="f8348-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f8348-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f8348-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f8348-110">Child elements</span></span>

|<span data-ttu-id="f8348-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="f8348-111">**Element**</span></span>|<span data-ttu-id="f8348-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f8348-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8348-113">メールボックス (文字列)</span><span class="sxs-lookup"><span data-stu-id="f8348-113">Mailbox (string)</span></span>](mailbox-string.md) <br/> |<span data-ttu-id="f8348-114">メールボックスの識別子を含みます。</span><span class="sxs-lookup"><span data-stu-id="f8348-114">Contains an identifier for the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="f8348-115">ErrorCode (int)</span><span class="sxs-lookup"><span data-stu-id="f8348-115">ErrorCode (int)</span></span>](errorcode-int.md) <br/> |<span data-ttu-id="f8348-116">検索に失敗したメールボックスのエラーコードを指定します。</span><span class="sxs-lookup"><span data-stu-id="f8348-116">Specifies the error code of the mailbox that failed the search.</span></span>  <br/> |
|[<span data-ttu-id="f8348-117">ErrorMessage</span><span class="sxs-lookup"><span data-stu-id="f8348-117">ErrorMessage</span></span>](errormessage.md) <br/> |<span data-ttu-id="f8348-118">検証エラーの理由を表します。</span><span class="sxs-lookup"><span data-stu-id="f8348-118">Represents the reason for the validation error.</span></span>  <br/> |
|[<span data-ttu-id="f8348-119">IsArchive</span><span class="sxs-lookup"><span data-stu-id="f8348-119">IsArchive</span></span>](isarchive.md) <br/> |<span data-ttu-id="f8348-120">メールボックスがアーカイブであるかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="f8348-120">Specifies a Boolean value that indicates whether the mailbox is an archive.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f8348-121">親要素</span><span class="sxs-lookup"><span data-stu-id="f8348-121">Parent elements</span></span>

|<span data-ttu-id="f8348-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="f8348-122">**Element**</span></span>|<span data-ttu-id="f8348-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="f8348-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f8348-124">失敗したメールボックス</span><span class="sxs-lookup"><span data-stu-id="f8348-124">FailedMailboxes</span></span>](failedmailboxes.md) <br/> |<span data-ttu-id="f8348-125">エラーが発生したメールボックスの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="f8348-125">Specifies an array of failed mailboxes.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f8348-126">注釈</span><span class="sxs-lookup"><span data-stu-id="f8348-126">Remarks</span></span>

<span data-ttu-id="f8348-127">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f8348-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f8348-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f8348-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f8348-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f8348-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f8348-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="f8348-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f8348-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f8348-131">Schema Name</span></span>  <br/> |<span data-ttu-id="f8348-132">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="f8348-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="f8348-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f8348-133">Validation File</span></span>  <br/> |<span data-ttu-id="f8348-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f8348-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f8348-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f8348-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f8348-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="f8348-136">See also</span></span>



- [<span data-ttu-id="f8348-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f8348-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

