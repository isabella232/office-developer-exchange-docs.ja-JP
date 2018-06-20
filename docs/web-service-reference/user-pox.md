---
title: ユーザー (POX)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 7c42b516-77f6-4aee-99d8-b866d82d793a
description: ユーザーの要素は、ユーザー固有の情報を提供します。
ms.openlocfilehash: 3f90ff0cc00170170c7304f2a19fe1d7abd9d1bc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839920"
---
# <a name="user-pox"></a><span data-ttu-id="50772-103">ユーザー (POX)</span><span class="sxs-lookup"><span data-stu-id="50772-103">User (POX)</span></span>

<span data-ttu-id="50772-104">**ユーザー**の要素は、ユーザー固有の情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="50772-104">The **User** element provides user-specific information.</span></span> 
  
[<span data-ttu-id="50772-105">(POX) を自動検出</span><span class="sxs-lookup"><span data-stu-id="50772-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="50772-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="50772-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="50772-107">ユーザー (POX)</span><span class="sxs-lookup"><span data-stu-id="50772-107">User (POX)</span></span>](user-pox.md)
  
```xml
<User>
   <DisplayName/>
   <LegacyDN/>
   <DeploymentId/>
   <AutoDiscoverSMTPAddress/>
</User>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="50772-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="50772-108">Attributes and elements</span></span>

<span data-ttu-id="50772-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="50772-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="50772-110">属性</span><span class="sxs-lookup"><span data-stu-id="50772-110">Attributes</span></span>

<span data-ttu-id="50772-111">なし。</span><span class="sxs-lookup"><span data-stu-id="50772-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="50772-112">子要素</span><span class="sxs-lookup"><span data-stu-id="50772-112">Child elements</span></span>

|<span data-ttu-id="50772-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="50772-113">**Element**</span></span>|<span data-ttu-id="50772-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="50772-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50772-115">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="50772-115">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="50772-116">ユーザーの表示名を表します。</span><span class="sxs-lookup"><span data-stu-id="50772-116">Represents the user's display name.</span></span>  <br/> |
|[<span data-ttu-id="50772-117">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="50772-117">LegacyDN (POX)</span></span>](legacydn-pox.md) <br/> |<span data-ttu-id="50772-118">従来の識別名によって、ユーザーのメールボックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="50772-118">Identifies a user's mailbox by legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="50772-119">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="50772-119">DeploymentId (POX)</span></span>](deploymentid-pox.md) <br/> |<span data-ttu-id="50772-120">Exchange フォレストを一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="50772-120">Uniquely identifies the Exchange forest.</span></span>  <br/> |
|[<span data-ttu-id="50772-121">AutoDiscoverSMTPAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="50772-121">AutoDiscoverSMTPAddress (POX)</span></span>](autodiscoversmtpaddress-pox.md) <br/> |<span data-ttu-id="50772-122">自動検出プロセスで使用されるユーザーの SMTP アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="50772-122">Contains the user's SMTP address that is used for the Autodiscover process.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="50772-123">親要素</span><span class="sxs-lookup"><span data-stu-id="50772-123">Parent elements</span></span>

|<span data-ttu-id="50772-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="50772-124">**Element**</span></span>|<span data-ttu-id="50772-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="50772-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="50772-126">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="50772-126">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="50772-127">自動検出サービスからの応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="50772-127">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="50772-128">備考</span><span class="sxs-lookup"><span data-stu-id="50772-128">Remarks</span></span>

<span data-ttu-id="50772-129">自動検出の要求と応答は、UTF-8 エンコードである必要があります。</span><span class="sxs-lookup"><span data-stu-id="50772-129">Autodiscover requests and responses must be UTF-8 encoded.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="50772-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="50772-130">See also</span></span>



[<span data-ttu-id="50772-131">交換の POX の自動検出の XML 要素</span><span class="sxs-lookup"><span data-stu-id="50772-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

