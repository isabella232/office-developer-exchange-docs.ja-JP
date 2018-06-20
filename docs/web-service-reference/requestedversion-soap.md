---
title: RequestedVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 962036c9-9b13-4669-bed2-2502c0f5aabe
description: RequestedVersion 要素は、クライアントが要求の処理を依頼する最低限のサービスのバージョンを指定します。
ms.openlocfilehash: 0d8682c33790d2d26001512ad9e2191ae52074d0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833134"
---
# <a name="requestedversion-soap"></a><span data-ttu-id="7e83f-103">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7e83f-103">RequestedVersion (SOAP)</span></span>

<span data-ttu-id="7e83f-104">**RequestedVersion**要素は、クライアントが要求の処理を依頼する最低限のサービスのバージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="7e83f-104">The **RequestedVersion** element specifies the minimum service version that the client wants the request to be processed on.</span></span> 
  
```XML
<RequestedVersion/>
```

 <span data-ttu-id="7e83f-105">**ExchangeVersion**</span><span class="sxs-lookup"><span data-stu-id="7e83f-105">**ExchangeVersion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e83f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7e83f-106">Attributes and elements</span></span>

<span data-ttu-id="7e83f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7e83f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e83f-108">属性</span><span class="sxs-lookup"><span data-stu-id="7e83f-108">Attributes</span></span>

<span data-ttu-id="7e83f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7e83f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e83f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7e83f-110">Child elements</span></span>

<span data-ttu-id="7e83f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7e83f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7e83f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7e83f-112">Parent elements</span></span>

|<span data-ttu-id="7e83f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="7e83f-113">**Element**</span></span>|<span data-ttu-id="7e83f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e83f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e83f-115">要求 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7e83f-115">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="7e83f-116">要求された構成設定とユーザーを対象に含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e83f-116">Contains the requested configuration settings and the target users.</span></span>  <br/> |
|[<span data-ttu-id="7e83f-117">要求 (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7e83f-117">Request (GetDomainSettings) (SOAP)</span></span>](request-getdomainsettingssoap.md) <br/> |<span data-ttu-id="7e83f-118">ドメインの設定を取得する要求を表します。</span><span class="sxs-lookup"><span data-stu-id="7e83f-118">Represents a request to get domain settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7e83f-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7e83f-119">Text value</span></span>

<span data-ttu-id="7e83f-120">**RequestedVersion**要素のテキスト値には、Exchange2010、Exchange2010_SP1、Exchange2010_SP2、または Exchange2013 を指定できます。</span><span class="sxs-lookup"><span data-stu-id="7e83f-120">The text value for the **RequestedVersion** element can be Exchange2010, Exchange2010_SP1, Exchange2010_SP2, or Exchange2013.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7e83f-121">備考</span><span class="sxs-lookup"><span data-stu-id="7e83f-121">Remarks</span></span>

<span data-ttu-id="7e83f-122">この要素が存在しない場合は、サービスの最新バージョンが使用されます。</span><span class="sxs-lookup"><span data-stu-id="7e83f-122">If this element is not present, the latest service version is used.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e83f-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="7e83f-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e83f-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="7e83f-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="7e83f-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7e83f-125">Schema Name</span></span>  <br/> |<span data-ttu-id="7e83f-126">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="7e83f-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="7e83f-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7e83f-127">Validation File</span></span>  <br/> |<span data-ttu-id="7e83f-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7e83f-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7e83f-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7e83f-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e83f-130">False</span><span class="sxs-lookup"><span data-stu-id="7e83f-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e83f-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="7e83f-131">See also</span></span>



[<span data-ttu-id="7e83f-132">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7e83f-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="7e83f-133">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="7e83f-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

