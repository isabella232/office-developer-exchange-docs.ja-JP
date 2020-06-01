---
title: FindMailboxStatisticsByKeywordsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af1dd9bf-df47-473d-a2ce-ab9a01a37606
description: FindMailboxStatisticsByKeywordsResponse 要素は、FindMailboxStatisticsByKeywords 要求に対する応答を指定します。
ms.openlocfilehash: a0595ec9ee0cedf5150852dc39eca50b598e15aa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460989"
---
# <a name="findmailboxstatisticsbykeywordsresponse"></a><span data-ttu-id="85d0f-103">FindMailboxStatisticsByKeywordsResponse</span><span class="sxs-lookup"><span data-stu-id="85d0f-103">FindMailboxStatisticsByKeywordsResponse</span></span>

<span data-ttu-id="85d0f-104">**FindMailboxStatisticsByKeywordsResponse**要素は、 **FindMailboxStatisticsByKeywords**要求に対する応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="85d0f-104">The **FindMailboxStatisticsByKeywordsResponse** element specifies the response to a **FindMailboxStatisticsByKeywords** request.</span></span> 
  
```XML
<FindMailboxStatisticsByKeywordsResponse>
    <ResponseMessages/>
</FindMailboxStatisticsByKeywordsResponse>
```

 <span data-ttu-id="85d0f-105">**FindMailboxStatisticsByKeywordsResponseType**</span><span class="sxs-lookup"><span data-stu-id="85d0f-105">**FindMailboxStatisticsByKeywordsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="85d0f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="85d0f-106">Attributes and elements</span></span>

<span data-ttu-id="85d0f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="85d0f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="85d0f-108">属性</span><span class="sxs-lookup"><span data-stu-id="85d0f-108">Attributes</span></span>

<span data-ttu-id="85d0f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="85d0f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="85d0f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="85d0f-110">Child elements</span></span>

|<span data-ttu-id="85d0f-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="85d0f-111">**Element**</span></span>|<span data-ttu-id="85d0f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="85d0f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="85d0f-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="85d0f-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="85d0f-114">Exchange Web サービス (EWS) 要求に対する応答メッセージが保存されています。</span><span class="sxs-lookup"><span data-stu-id="85d0f-114">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="85d0f-115">親要素</span><span class="sxs-lookup"><span data-stu-id="85d0f-115">Parent elements</span></span>

<span data-ttu-id="85d0f-116">なし。</span><span class="sxs-lookup"><span data-stu-id="85d0f-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="85d0f-117">注釈</span><span class="sxs-lookup"><span data-stu-id="85d0f-117">Remarks</span></span>

<span data-ttu-id="85d0f-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="85d0f-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="85d0f-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="85d0f-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="85d0f-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="85d0f-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="85d0f-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="85d0f-121">Schema Name</span></span>  <br/> |<span data-ttu-id="85d0f-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="85d0f-122">Message schema</span></span>  <br/> |
|<span data-ttu-id="85d0f-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="85d0f-123">Validation File</span></span>  <br/> |<span data-ttu-id="85d0f-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="85d0f-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="85d0f-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="85d0f-125">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="85d0f-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="85d0f-126">See also</span></span>



- [<span data-ttu-id="85d0f-127">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="85d0f-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

