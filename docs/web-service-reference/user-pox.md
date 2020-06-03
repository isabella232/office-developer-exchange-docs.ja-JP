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
description: User 要素は、ユーザー固有の情報を提供します。
ms.openlocfilehash: 8f53319bcf34595305748adafc9aa1e25283611e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530219"
---
# <a name="user-pox"></a><span data-ttu-id="fbefe-103">ユーザー (POX)</span><span class="sxs-lookup"><span data-stu-id="fbefe-103">User (POX)</span></span>

<span data-ttu-id="fbefe-104">**User**要素は、ユーザー固有の情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="fbefe-104">The **User** element provides user-specific information.</span></span> 
  
[<span data-ttu-id="fbefe-105">自動検出 (POX)</span><span class="sxs-lookup"><span data-stu-id="fbefe-105">AutoDiscover (POX)</span></span>](autodiscover-pox.md)
  
[<span data-ttu-id="fbefe-106">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="fbefe-106">Response (POX)</span></span>](response-pox.md)
  
[<span data-ttu-id="fbefe-107">ユーザー (POX)</span><span class="sxs-lookup"><span data-stu-id="fbefe-107">User (POX)</span></span>](user-pox.md)
  
```xml
<User>
   <DisplayName/>
   <LegacyDN/>
   <DeploymentId/>
   <AutoDiscoverSMTPAddress/>
</User>
```

## <a name="attributes-and-elements"></a><span data-ttu-id="fbefe-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fbefe-108">Attributes and elements</span></span>

<span data-ttu-id="fbefe-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fbefe-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fbefe-110">属性</span><span class="sxs-lookup"><span data-stu-id="fbefe-110">Attributes</span></span>

<span data-ttu-id="fbefe-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fbefe-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fbefe-112">子要素</span><span class="sxs-lookup"><span data-stu-id="fbefe-112">Child elements</span></span>

|<span data-ttu-id="fbefe-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="fbefe-113">**Element**</span></span>|<span data-ttu-id="fbefe-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="fbefe-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fbefe-115">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="fbefe-115">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="fbefe-116">ユーザーの表示名を表します。</span><span class="sxs-lookup"><span data-stu-id="fbefe-116">Represents the user's display name.</span></span>  <br/> |
|[<span data-ttu-id="fbefe-117">LegacyDN (POX)</span><span class="sxs-lookup"><span data-stu-id="fbefe-117">LegacyDN (POX)</span></span>](legacydn-pox.md) <br/> |<span data-ttu-id="fbefe-118">従来の識別名でユーザーのメールボックスを識別します。</span><span class="sxs-lookup"><span data-stu-id="fbefe-118">Identifies a user's mailbox by legacy distinguished name.</span></span>  <br/> |
|[<span data-ttu-id="fbefe-119">DeploymentId (POX)</span><span class="sxs-lookup"><span data-stu-id="fbefe-119">DeploymentId (POX)</span></span>](deploymentid-pox.md) <br/> |<span data-ttu-id="fbefe-120">Exchange フォレストを一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="fbefe-120">Uniquely identifies the Exchange forest.</span></span>  <br/> |
|[<span data-ttu-id="fbefe-121">AutoDiscoverSMTPAddress (POX)</span><span class="sxs-lookup"><span data-stu-id="fbefe-121">AutoDiscoverSMTPAddress (POX)</span></span>](autodiscoversmtpaddress-pox.md) <br/> |<span data-ttu-id="fbefe-122">自動検出プロセスで使用されるユーザーの SMTP アドレスが含まれます。</span><span class="sxs-lookup"><span data-stu-id="fbefe-122">Contains the user's SMTP address that is used for the Autodiscover process.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fbefe-123">親要素</span><span class="sxs-lookup"><span data-stu-id="fbefe-123">Parent elements</span></span>

|<span data-ttu-id="fbefe-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="fbefe-124">**Element**</span></span>|<span data-ttu-id="fbefe-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="fbefe-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fbefe-126">応答 (POX)</span><span class="sxs-lookup"><span data-stu-id="fbefe-126">Response (POX)</span></span>](response-pox.md) <br/> |<span data-ttu-id="fbefe-127">自動検出サービスからの応答を含みます。</span><span class="sxs-lookup"><span data-stu-id="fbefe-127">Contains the response from the Autodiscover service.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fbefe-128">注釈</span><span class="sxs-lookup"><span data-stu-id="fbefe-128">Remarks</span></span>

<span data-ttu-id="fbefe-129">自動検出要求と応答は、UTF-8 でエンコードする必要があります。</span><span class="sxs-lookup"><span data-stu-id="fbefe-129">Autodiscover requests and responses must be UTF-8 encoded.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="fbefe-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="fbefe-130">See also</span></span>



[<span data-ttu-id="fbefe-131">Exchange の POX 自動検出 XML 要素</span><span class="sxs-lookup"><span data-stu-id="fbefe-131">POX Autodiscover XML elements for Exchange</span></span>](pox-autodiscover-xml-elements-for-exchange.md)

