---
title: エラー (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 91c63b62-ab68-4c32-a2f7-5a87c188335b
description: Error 要素には、自動検出エラー応答が含まれています。
ms.openlocfilehash: 3135a352365fe3000ce2d202ad78452d5c8ccc7f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760318"
---
# <a name="error-pox"></a><span data-ttu-id="99762-103">エラー (POX)</span><span class="sxs-lookup"><span data-stu-id="99762-103">Error (POX)</span></span>

<span data-ttu-id="99762-104">**Error**要素には、自動検出エラー応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="99762-104">The **Error** element contains an Autodiscover error response.</span></span> 
  
[<span data-ttu-id="99762-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="99762-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="99762-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="99762-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="99762-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="99762-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="99762-108">エラー (POX)</span><span class="sxs-lookup"><span data-stu-id="99762-108">Error (POX)</span></span>](error-pox.md)
  
```xml
<Error Time="" Id="">
   <ErrorCode/>
   <Message/>
   <DebugData/>
</Error>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="99762-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="99762-109">Attributes and elements</span></span>

<span data-ttu-id="99762-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="99762-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="99762-111">属性</span><span class="sxs-lookup"><span data-stu-id="99762-111">Attributes</span></span>

|<span data-ttu-id="99762-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="99762-112">**Attribute**</span></span>|<span data-ttu-id="99762-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="99762-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="99762-114">時刻型 (Time)</span><span class="sxs-lookup"><span data-stu-id="99762-114">Time</span></span>  <br/> |<span data-ttu-id="99762-115">エラー応答が返された時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="99762-115">Represents the time when the error response was returned.</span></span>  <br/> |
|<span data-ttu-id="99762-116">ID</span><span class="sxs-lookup"><span data-stu-id="99762-116">Id</span></span>  <br/> |<span data-ttu-id="99762-117">クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの名前のハッシュを表します。</span><span class="sxs-lookup"><span data-stu-id="99762-117">Represents a hash of the name of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="99762-118">子要素</span><span class="sxs-lookup"><span data-stu-id="99762-118">Child elements</span></span>

|<span data-ttu-id="99762-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="99762-119">**Element**</span></span>|<span data-ttu-id="99762-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="99762-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99762-121">エラー コード (POX)</span><span class="sxs-lookup"><span data-stu-id="99762-121">ErrorCode (POX)</span></span>](errorcode-pox.md) <br/> |<span data-ttu-id="99762-122">エラー自動検出応答のエラー コードが含まれています。</span><span class="sxs-lookup"><span data-stu-id="99762-122">Contains the error code for an error Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="99762-123">メッセージ (POX)</span><span class="sxs-lookup"><span data-stu-id="99762-123">Message (POX)</span></span>](message-pox.md) <br/> |<span data-ttu-id="99762-124">エラー自動検出応答のエラー メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="99762-124">Contains the error message for an error Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="99762-125">DebugData (POX)</span><span class="sxs-lookup"><span data-stu-id="99762-125">DebugData (POX)</span></span>](debugdata-pox.md) <br/> |<span data-ttu-id="99762-126">自動検出応答エラーのデバッグ データを格納します。</span><span class="sxs-lookup"><span data-stu-id="99762-126">Contains the debug data for an error Autodiscover response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="99762-127">親要素</span><span class="sxs-lookup"><span data-stu-id="99762-127">Parent elements</span></span>

|<span data-ttu-id="99762-128">**要素**</span><span class="sxs-lookup"><span data-stu-id="99762-128">**Element**</span></span>|<span data-ttu-id="99762-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="99762-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="99762-130">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="99762-130">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="99762-131">自動検出エラー応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="99762-131">Contains an Autodiscover error response.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="99762-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="99762-132">See also</span></span>



[<span data-ttu-id="99762-133">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="99762-133">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

