---
title: FailedMailbox
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d4c9816-54bb-4932-b4ba-f057c9173a1a
description: FailedMailbox 要素は、検索に失敗したメールボックスは、エラー メッセージを指定します。
ms.openlocfilehash: a4f5cd975eba121dd1d8d918b638d34f907588a8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760464"
---
# <a name="failedmailbox"></a><span data-ttu-id="2a5da-103">FailedMailbox</span><span class="sxs-lookup"><span data-stu-id="2a5da-103">FailedMailbox</span></span>

<span data-ttu-id="2a5da-104">**FailedMailbox**要素は、検索に失敗したメールボックスは、エラー メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="2a5da-104">The **FailedMailbox** element specifies the error message for a mailbox that failed on search.</span></span> 
  
```XML
<FailedMailbox>
    <Mailbox/>
    <ErrorCode/>
    <ErrorMessage/>
    <IsArchive/>
</FailedMailbox>
```

 <span data-ttu-id="2a5da-105">**FailedSearchMailboxType**</span><span class="sxs-lookup"><span data-stu-id="2a5da-105">**FailedSearchMailboxType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2a5da-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2a5da-106">Attributes and elements</span></span>

<span data-ttu-id="2a5da-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2a5da-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a5da-108">属性</span><span class="sxs-lookup"><span data-stu-id="2a5da-108">Attributes</span></span>

<span data-ttu-id="2a5da-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2a5da-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2a5da-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2a5da-110">Child elements</span></span>

|<span data-ttu-id="2a5da-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="2a5da-111">**Element**</span></span>|<span data-ttu-id="2a5da-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2a5da-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a5da-113">メールボックス (文字列)</span><span class="sxs-lookup"><span data-stu-id="2a5da-113">Mailbox (string)</span></span>](mailbox-string.md) <br/> |<span data-ttu-id="2a5da-114">メールボックスの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2a5da-114">Contains an identifier for the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="2a5da-115">エラー コード (int)</span><span class="sxs-lookup"><span data-stu-id="2a5da-115">ErrorCode (int)</span></span>](errorcode-int.md) <br/> |<span data-ttu-id="2a5da-116">検索に失敗したメールボックスのエラー コードを指定します。</span><span class="sxs-lookup"><span data-stu-id="2a5da-116">Specifies the error code of the mailbox that failed the search.</span></span>  <br/> |
|[<span data-ttu-id="2a5da-117">エラー メッセージ</span><span class="sxs-lookup"><span data-stu-id="2a5da-117">ErrorMessage</span></span>](errormessage.md) <br/> |<span data-ttu-id="2a5da-118">検証エラーの原因を表します。</span><span class="sxs-lookup"><span data-stu-id="2a5da-118">Represents the reason for the validation error.</span></span>  <br/> |
|[<span data-ttu-id="2a5da-119">IsArchive</span><span class="sxs-lookup"><span data-stu-id="2a5da-119">IsArchive</span></span>](isarchive.md) <br/> |<span data-ttu-id="2a5da-120">メールボックスがアーカイブであるかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="2a5da-120">Specifies a Boolean value that indicates whether the mailbox is an archive.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2a5da-121">親要素</span><span class="sxs-lookup"><span data-stu-id="2a5da-121">Parent elements</span></span>

|<span data-ttu-id="2a5da-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="2a5da-122">**Element**</span></span>|<span data-ttu-id="2a5da-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="2a5da-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a5da-124">FailedMailboxes</span><span class="sxs-lookup"><span data-stu-id="2a5da-124">FailedMailboxes</span></span>](failedmailboxes.md) <br/> |<span data-ttu-id="2a5da-125">失敗したメールボックスの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="2a5da-125">Specifies an array of failed mailboxes.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2a5da-126">備考</span><span class="sxs-lookup"><span data-stu-id="2a5da-126">Remarks</span></span>

<span data-ttu-id="2a5da-127">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2a5da-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2a5da-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2a5da-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2a5da-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="2a5da-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2a5da-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="2a5da-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2a5da-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2a5da-131">Schema Name</span></span>  <br/> |<span data-ttu-id="2a5da-132">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="2a5da-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="2a5da-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2a5da-133">Validation File</span></span>  <br/> |<span data-ttu-id="2a5da-134">types.xsd</span><span class="sxs-lookup"><span data-stu-id="2a5da-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2a5da-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2a5da-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2a5da-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="2a5da-136">See also</span></span>



- [<span data-ttu-id="2a5da-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2a5da-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

