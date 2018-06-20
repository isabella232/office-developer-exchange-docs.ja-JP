---
title: ResolveNamesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNamesResponse
api_type:
- schema
ms.assetid: 5e7be1e2-44ea-403f-9135-2388d030078c
description: ResolveNamesResponse 要素は、ResolveNames 要求への応答を定義します。
ms.openlocfilehash: 686a7b2799f32ab9017cfe786f6dff8c67f0b98c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833164"
---
# <a name="resolvenamesresponse"></a><span data-ttu-id="f47a0-103">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="f47a0-103">ResolveNamesResponse</span></span>

<span data-ttu-id="f47a0-104">**ResolveNamesResponse**要素は、ResolveNames 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="f47a0-104">The **ResolveNamesResponse** element defines a response to a ResolveNames request.</span></span> 
  
```xml
<ResolveNamesResponse>
   <ResponseMessages/>
</ResolveNamesResponse>
```

 <span data-ttu-id="f47a0-105">**ResolveNamesResponseType**</span><span class="sxs-lookup"><span data-stu-id="f47a0-105">**ResolveNamesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f47a0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f47a0-106">Attributes and elements</span></span>

<span data-ttu-id="f47a0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f47a0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f47a0-108">属性</span><span class="sxs-lookup"><span data-stu-id="f47a0-108">Attributes</span></span>

<span data-ttu-id="f47a0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f47a0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f47a0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f47a0-110">Child elements</span></span>

|<span data-ttu-id="f47a0-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="f47a0-111">**Element**</span></span>|<span data-ttu-id="f47a0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f47a0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f47a0-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="f47a0-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="f47a0-114">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f47a0-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f47a0-115">親要素</span><span class="sxs-lookup"><span data-stu-id="f47a0-115">Parent elements</span></span>

<span data-ttu-id="f47a0-116">なし。</span><span class="sxs-lookup"><span data-stu-id="f47a0-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f47a0-117">備考</span><span class="sxs-lookup"><span data-stu-id="f47a0-117">Remarks</span></span>

<span data-ttu-id="f47a0-118">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="f47a0-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f47a0-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="f47a0-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f47a0-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="f47a0-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f47a0-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f47a0-121">Schema name</span></span>  <br/> |<span data-ttu-id="f47a0-122">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="f47a0-122">messages schema</span></span>  <br/> |
|<span data-ttu-id="f47a0-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f47a0-123">Validation file</span></span>  <br/> |<span data-ttu-id="f47a0-124">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f47a0-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f47a0-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f47a0-125">Can be empty</span></span>  <br/> |<span data-ttu-id="f47a0-126">False</span><span class="sxs-lookup"><span data-stu-id="f47a0-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f47a0-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="f47a0-127">See also</span></span>



[<span data-ttu-id="f47a0-128">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="f47a0-128">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="f47a0-129">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="f47a0-129">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="f47a0-130">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="f47a0-130">ResolveNames operation</span></span>](resolvenames-operation.md)

