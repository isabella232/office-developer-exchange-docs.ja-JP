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
description: ApplyConversationActionResponse 要素は、ApplyConversationAction 操作要求への応答を定義します。
ms.openlocfilehash: 22955378f8982c92b4cd0e9b8880b6907f47aa0c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461675"
---
# <a name="applyconversationactionresponse"></a><span data-ttu-id="a4333-103">ApplyConversationActionResponse</span><span class="sxs-lookup"><span data-stu-id="a4333-103">ApplyConversationActionResponse</span></span>

<span data-ttu-id="a4333-104">**ApplyConversationActionResponse**要素は、 [ApplyConversationAction 操作](applyconversationaction-operation.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="a4333-104">The **ApplyConversationActionResponse** element defines a response to an [ApplyConversationAction operation](applyconversationaction-operation.md) request.</span></span> 
  
[<span data-ttu-id="a4333-105">ApplyConversationActionResponse</span><span class="sxs-lookup"><span data-stu-id="a4333-105">ApplyConversationActionResponse</span></span>](applyconversationactionresponse.md)
  
```XML
<ApplyConversationActionResponse>
   <ResponseMessages/>
</ApplyConversationActionResponse>
```

 <span data-ttu-id="a4333-106">**ApplyConversationActionResponseType**</span><span class="sxs-lookup"><span data-stu-id="a4333-106">**ApplyConversationActionResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a4333-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a4333-107">Attributes and elements</span></span>

<span data-ttu-id="a4333-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a4333-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a4333-109">属性</span><span class="sxs-lookup"><span data-stu-id="a4333-109">Attributes</span></span>

<span data-ttu-id="a4333-110">なし。</span><span class="sxs-lookup"><span data-stu-id="a4333-110">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a4333-111">子要素</span><span class="sxs-lookup"><span data-stu-id="a4333-111">Child elements</span></span>

|<span data-ttu-id="a4333-112">**Element**</span><span class="sxs-lookup"><span data-stu-id="a4333-112">**Element**</span></span>|<span data-ttu-id="a4333-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="a4333-113">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a4333-114">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a4333-114">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a4333-115">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="a4333-115">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a4333-116">親要素</span><span class="sxs-lookup"><span data-stu-id="a4333-116">Parent elements</span></span>

<span data-ttu-id="a4333-117">なし。</span><span class="sxs-lookup"><span data-stu-id="a4333-117">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="a4333-118">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a4333-118">Text value</span></span>

<span data-ttu-id="a4333-119">なし。</span><span class="sxs-lookup"><span data-stu-id="a4333-119">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a4333-120">注釈</span><span class="sxs-lookup"><span data-stu-id="a4333-120">Remarks</span></span>

<span data-ttu-id="a4333-121">この要素は Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a4333-121">This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a4333-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a4333-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a4333-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="a4333-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a4333-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a4333-124">Schema name</span></span>  <br/> |<span data-ttu-id="a4333-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="a4333-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a4333-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a4333-126">Validation file</span></span>  <br/> |<span data-ttu-id="a4333-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a4333-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a4333-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a4333-128">Can be empty</span></span>  <br/> |<span data-ttu-id="a4333-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="a4333-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a4333-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="a4333-130">See also</span></span>

- [<span data-ttu-id="a4333-131">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="a4333-131">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="a4333-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a4333-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

