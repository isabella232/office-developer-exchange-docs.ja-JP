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
description: ResolveNamesResponse 要素は、ResolveNames 要求に対する応答を定義します。
ms.openlocfilehash: 29ae2d20db9f2d689f315f66d62385252046c055
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455605"
---
# <a name="resolvenamesresponse"></a><span data-ttu-id="19444-103">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="19444-103">ResolveNamesResponse</span></span>

<span data-ttu-id="19444-104">**ResolveNamesResponse**要素は、ResolveNames 要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="19444-104">The **ResolveNamesResponse** element defines a response to a ResolveNames request.</span></span> 
  
```xml
<ResolveNamesResponse>
   <ResponseMessages/>
</ResolveNamesResponse>
```

 <span data-ttu-id="19444-105">**ResolveNamesResponseType**</span><span class="sxs-lookup"><span data-stu-id="19444-105">**ResolveNamesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="19444-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="19444-106">Attributes and elements</span></span>

<span data-ttu-id="19444-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="19444-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="19444-108">属性</span><span class="sxs-lookup"><span data-stu-id="19444-108">Attributes</span></span>

<span data-ttu-id="19444-109">なし。</span><span class="sxs-lookup"><span data-stu-id="19444-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="19444-110">子要素</span><span class="sxs-lookup"><span data-stu-id="19444-110">Child elements</span></span>

|<span data-ttu-id="19444-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="19444-111">**Element**</span></span>|<span data-ttu-id="19444-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="19444-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="19444-113">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="19444-113">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="19444-114">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="19444-114">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="19444-115">親要素</span><span class="sxs-lookup"><span data-stu-id="19444-115">Parent elements</span></span>

<span data-ttu-id="19444-116">なし。</span><span class="sxs-lookup"><span data-stu-id="19444-116">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="19444-117">注釈</span><span class="sxs-lookup"><span data-stu-id="19444-117">Remarks</span></span>

<span data-ttu-id="19444-118">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="19444-118">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="19444-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="19444-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="19444-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="19444-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="19444-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="19444-121">Schema name</span></span>  <br/> |<span data-ttu-id="19444-122">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="19444-122">messages schema</span></span>  <br/> |
|<span data-ttu-id="19444-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="19444-123">Validation file</span></span>  <br/> |<span data-ttu-id="19444-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="19444-124">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="19444-125">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="19444-125">Can be empty</span></span>  <br/> |<span data-ttu-id="19444-126">正しくない</span><span class="sxs-lookup"><span data-stu-id="19444-126">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="19444-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="19444-127">See also</span></span>



[<span data-ttu-id="19444-128">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="19444-128">ResolveNames</span></span>](resolvenames.md)
  
[<span data-ttu-id="19444-129">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="19444-129">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
[<span data-ttu-id="19444-130">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="19444-130">ResolveNames operation</span></span>](resolvenames-operation.md)

