---
title: FindMailboxStatisticsByKeywordsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: af1dd9bf-df47-473d-a2ce-ab9a01a37606
description: FindMailboxStatisticsByKeywordsResponse 要素は、FindMailboxStatisticsByKeywords 要求への応答を指定します。
ms.openlocfilehash: 43d3a9c4d5ca312f380fed65eb906543f25e5a1c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760514"
---
# <a name="findmailboxstatisticsbykeywordsresponse"></a><span data-ttu-id="2cb2a-103">FindMailboxStatisticsByKeywordsResponse</span><span class="sxs-lookup"><span data-stu-id="2cb2a-103">FindMailboxStatisticsByKeywordsResponse</span></span>

<span data-ttu-id="2cb2a-104">**FindMailboxStatisticsByKeywordsResponse**要素は、 **FindMailboxStatisticsByKeywords**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="2cb2a-104">The **FindMailboxStatisticsByKeywordsResponse** element specifies the response to a **FindMailboxStatisticsByKeywords** request.</span></span> 
  
```XML
<FindMailboxStatisticsByKeywordsResponse>
    <ResponseMessages/>
</FindMailboxStatisticsByKeywordsResponse>
```

 <span data-ttu-id="2cb2a-105">**FindMailboxStatisticsByKeywordsResponseType**</span><span class="sxs-lookup"><span data-stu-id="2cb2a-105">**FindMailboxStatisticsByKeywordsResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2cb2a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2cb2a-106">Attributes and elements</span></span>

<span data-ttu-id="2cb2a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2cb2a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2cb2a-108">属性</span><span class="sxs-lookup"><span data-stu-id="2cb2a-108">Attributes</span></span>

<span data-ttu-id="2cb2a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2cb2a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2cb2a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2cb2a-110">Child elements</span></span>

|<span data-ttu-id="2cb2a-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="2cb2a-111">**Element**</span></span>|<span data-ttu-id="2cb2a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2cb2a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cb2a-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2cb2a-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="2cb2a-114">Exchange Web サービス (EWS) 要求の応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2cb2a-114">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2cb2a-115">親要素</span><span class="sxs-lookup"><span data-stu-id="2cb2a-115">Parent elements</span></span>

<span data-ttu-id="2cb2a-116">なし。</span><span class="sxs-lookup"><span data-stu-id="2cb2a-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2cb2a-117">備考</span><span class="sxs-lookup"><span data-stu-id="2cb2a-117">Remarks</span></span>

<span data-ttu-id="2cb2a-118">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2cb2a-118">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2cb2a-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="2cb2a-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2cb2a-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="2cb2a-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2cb2a-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2cb2a-121">Schema Name</span></span>  <br/> |<span data-ttu-id="2cb2a-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="2cb2a-122">Message schema</span></span>  <br/> |
|<span data-ttu-id="2cb2a-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2cb2a-123">Validation File</span></span>  <br/> |<span data-ttu-id="2cb2a-124">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2cb2a-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2cb2a-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2cb2a-125">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2cb2a-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="2cb2a-126">See also</span></span>



- [<span data-ttu-id="2cb2a-127">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2cb2a-127">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

