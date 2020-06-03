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
description: Error 要素には、自動検出エラー応答が含まれます。
ms.openlocfilehash: 1a1a3e83898674e605921cb75371036a8a561a95
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530650"
---
# <a name="error-pox"></a><span data-ttu-id="acf04-103">エラー (POX)</span><span class="sxs-lookup"><span data-stu-id="acf04-103">Error (POX)</span></span>

<span data-ttu-id="acf04-104">**Error**要素には、自動検出エラー応答が含まれます。</span><span class="sxs-lookup"><span data-stu-id="acf04-104">The **Error** element contains an Autodiscover error response.</span></span> 
  
[<span data-ttu-id="acf04-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="acf04-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="acf04-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="acf04-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="acf04-107">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="acf04-107">Account (POX)</span></span>](account-pox.md)
  
[<span data-ttu-id="acf04-108">エラー (POX)</span><span class="sxs-lookup"><span data-stu-id="acf04-108">Error (POX)</span></span>](error-pox.md)
  
```xml
<Error Time="" Id="">
   <ErrorCode/>
   <Message/>
   <DebugData/>
</Error>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="acf04-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="acf04-109">Attributes and elements</span></span>

<span data-ttu-id="acf04-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="acf04-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="acf04-111">属性</span><span class="sxs-lookup"><span data-stu-id="acf04-111">Attributes</span></span>

|<span data-ttu-id="acf04-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="acf04-112">**Attribute**</span></span>|<span data-ttu-id="acf04-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="acf04-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="acf04-114">Time</span><span class="sxs-lookup"><span data-stu-id="acf04-114">Time</span></span>  <br/> |<span data-ttu-id="acf04-115">エラー応答が返された時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="acf04-115">Represents the time when the error response was returned.</span></span>  <br/> |
|<span data-ttu-id="acf04-116">ID</span><span class="sxs-lookup"><span data-stu-id="acf04-116">Id</span></span>  <br/> |<span data-ttu-id="acf04-117">クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの名前のハッシュを表します。</span><span class="sxs-lookup"><span data-stu-id="acf04-117">Represents a hash of the name of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="acf04-118">子要素</span><span class="sxs-lookup"><span data-stu-id="acf04-118">Child elements</span></span>

|<span data-ttu-id="acf04-119">**Element**</span><span class="sxs-lookup"><span data-stu-id="acf04-119">**Element**</span></span>|<span data-ttu-id="acf04-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="acf04-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="acf04-121">ErrorCode (POX)</span><span class="sxs-lookup"><span data-stu-id="acf04-121">ErrorCode (POX)</span></span>](errorcode-pox.md) <br/> |<span data-ttu-id="acf04-122">エラー自動検出応答のエラーコードが含まれています。</span><span class="sxs-lookup"><span data-stu-id="acf04-122">Contains the error code for an error Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="acf04-123">メッセージ (POX)</span><span class="sxs-lookup"><span data-stu-id="acf04-123">Message (POX)</span></span>](message-pox.md) <br/> |<span data-ttu-id="acf04-124">エラー自動検出応答のエラーメッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="acf04-124">Contains the error message for an error Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="acf04-125">DebugData (POX)</span><span class="sxs-lookup"><span data-stu-id="acf04-125">DebugData (POX)</span></span>](debugdata-pox.md) <br/> |<span data-ttu-id="acf04-126">エラー自動検出応答のデバッグデータが保存されています。</span><span class="sxs-lookup"><span data-stu-id="acf04-126">Contains the debug data for an error Autodiscover response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="acf04-127">親要素</span><span class="sxs-lookup"><span data-stu-id="acf04-127">Parent elements</span></span>

|<span data-ttu-id="acf04-128">**要素**</span><span class="sxs-lookup"><span data-stu-id="acf04-128">**Element**</span></span>|<span data-ttu-id="acf04-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="acf04-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="acf04-130">アカウント (POX)</span><span class="sxs-lookup"><span data-stu-id="acf04-130">Account (POX)</span></span>](account-pox.md) <br/> |<span data-ttu-id="acf04-131">自動検出エラー応答を格納します。</span><span class="sxs-lookup"><span data-stu-id="acf04-131">Contains an Autodiscover error response.</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="acf04-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="acf04-132">See also</span></span>



[<span data-ttu-id="acf04-133">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="acf04-133">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

