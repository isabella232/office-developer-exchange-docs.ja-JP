---
title: ApplyConversationActionResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationActionResponse
api_type:
- schema
ms.assetid: 682d47a6-f9fe-4cc6-a56c-c5db835d5ec6
description: ApplyConversationActionResponse 要素は、ApplyConversationAction の操作要求に対する応答を定義します。
ms.openlocfilehash: 39f7344596de7376e770ed98dbe372a590057deb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759412"
---
# <a name="applyconversationactionresponse"></a><span data-ttu-id="45bcb-103">ApplyConversationActionResponse</span><span class="sxs-lookup"><span data-stu-id="45bcb-103">ApplyConversationActionResponse</span></span>

<span data-ttu-id="45bcb-104">**ApplyConversationActionResponse**要素は、 [ApplyConversationAction 操作](applyconversationaction-operation.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="45bcb-104">The **ApplyConversationActionResponse** element defines a response to an [ApplyConversationAction operation](applyconversationaction-operation.md) request.</span></span> 
  
[<span data-ttu-id="45bcb-105">ApplyConversationActionResponse</span><span class="sxs-lookup"><span data-stu-id="45bcb-105">ApplyConversationActionResponse</span></span>](applyconversationactionresponse.md)
  
```XML
<ApplyConversationActionResponse>
   <ResponseMessages/>
</ApplyConversationActionResponse>
```

 <span data-ttu-id="45bcb-106">**ApplyConversationActionResponseType**</span><span class="sxs-lookup"><span data-stu-id="45bcb-106">**ApplyConversationActionResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="45bcb-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="45bcb-107">Attributes and elements</span></span>

<span data-ttu-id="45bcb-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="45bcb-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="45bcb-109">属性</span><span class="sxs-lookup"><span data-stu-id="45bcb-109">Attributes</span></span>

<span data-ttu-id="45bcb-110">なし。</span><span class="sxs-lookup"><span data-stu-id="45bcb-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="45bcb-111">子要素</span><span class="sxs-lookup"><span data-stu-id="45bcb-111">Child elements</span></span>

|<span data-ttu-id="45bcb-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="45bcb-112">**Element**</span></span>|<span data-ttu-id="45bcb-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="45bcb-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="45bcb-114">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="45bcb-114">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="45bcb-115">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="45bcb-115">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="45bcb-116">親要素</span><span class="sxs-lookup"><span data-stu-id="45bcb-116">Parent elements</span></span>

<span data-ttu-id="45bcb-117">なし。</span><span class="sxs-lookup"><span data-stu-id="45bcb-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="45bcb-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="45bcb-118">Text value</span></span>

<span data-ttu-id="45bcb-119">なし。</span><span class="sxs-lookup"><span data-stu-id="45bcb-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="45bcb-120">備考</span><span class="sxs-lookup"><span data-stu-id="45bcb-120">Remarks</span></span>

<span data-ttu-id="45bcb-121">この要素は Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="45bcb-121">This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="45bcb-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="45bcb-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="45bcb-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="45bcb-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="45bcb-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="45bcb-124">Schema name</span></span>  <br/> |<span data-ttu-id="45bcb-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="45bcb-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="45bcb-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="45bcb-126">Validation file</span></span>  <br/> |<span data-ttu-id="45bcb-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="45bcb-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="45bcb-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="45bcb-128">Can be empty</span></span>  <br/> |<span data-ttu-id="45bcb-129">False</span><span class="sxs-lookup"><span data-stu-id="45bcb-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="45bcb-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="45bcb-130">See also</span></span>

- [<span data-ttu-id="45bcb-131">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="45bcb-131">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="45bcb-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="45bcb-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

