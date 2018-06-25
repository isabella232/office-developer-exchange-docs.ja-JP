---
title: DomainResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 6aa319be-3a01-4044-8dfc-8fa1318524c3
description: DomainResponse 要素には、指定したドメインの指定された設定が含まれています。
ms.openlocfilehash: c40f33a278b5032913329a7cd64346b572f5df2f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760149"
---
# <a name="domainresponse-soap"></a><span data-ttu-id="e3abc-103">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3abc-103">DomainResponse (SOAP)</span></span>

<span data-ttu-id="e3abc-104">**DomainResponse**要素には、指定したドメインの指定された設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e3abc-104">The **DomainResponse** element contains the requested settings for the specified domain.</span></span> 
  
```XML
<DomainResponse>
   <DomainSettingErrors/>
   <DomainSettings/>
   <RedirectTarget/>
   <ErrorCode/>
   <ErrorMessage/>
</DomainResponse>
```

 <span data-ttu-id="e3abc-105">**DomainResponse**</span><span class="sxs-lookup"><span data-stu-id="e3abc-105">**DomainResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3abc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e3abc-106">Attributes and elements</span></span>

<span data-ttu-id="e3abc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e3abc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3abc-108">属性</span><span class="sxs-lookup"><span data-stu-id="e3abc-108">Attributes</span></span>

<span data-ttu-id="e3abc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e3abc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e3abc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e3abc-110">Child elements</span></span>

|<span data-ttu-id="e3abc-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="e3abc-111">**Element**</span></span>|<span data-ttu-id="e3abc-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e3abc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3abc-113">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3abc-113">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md) <br/> |<span data-ttu-id="e3abc-114">返されませんでしたの設定に関するエラー情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e3abc-114">Contains error information for settings that could not be returned.</span></span>  <br/> |
|[<span data-ttu-id="e3abc-115">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3abc-115">DomainSettings (SOAP)</span></span>](domainsettings-soap.md) <br/> |<span data-ttu-id="e3abc-116">自動検出要求の送信、または、自動検出応答によって返されるドメインの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="e3abc-116">Represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="e3abc-117">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3abc-117">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md) <br/> |<span data-ttu-id="e3abc-118">リダイレクトのターゲットを識別します。</span><span class="sxs-lookup"><span data-stu-id="e3abc-118">Identifies the target of the redirection.</span></span> <span data-ttu-id="e3abc-119">ターゲットは、URL または電子メール アドレスのいずれかを使用できます。</span><span class="sxs-lookup"><span data-stu-id="e3abc-119">The target can be either a URL or an e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="e3abc-120">エラー コード (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3abc-120">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="e3abc-121">特定の要求に関連付けられているエラー コードを指定します。</span><span class="sxs-lookup"><span data-stu-id="e3abc-121">Specifies the error code that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="e3abc-122">エラー メッセージ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3abc-122">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="e3abc-123">特定の要求に関連付けられているエラー メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="e3abc-123">Specifies the error message that is associated with the specific request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e3abc-124">親要素</span><span class="sxs-lookup"><span data-stu-id="e3abc-124">Parent elements</span></span>

|<span data-ttu-id="e3abc-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="e3abc-125">**Element**</span></span>|<span data-ttu-id="e3abc-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="e3abc-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3abc-127">ArrayOfDomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3abc-127">ArrayOfDomainResponse (SOAP)</span></span>](arrayofdomainresponse-soap.md) <br/> |<span data-ttu-id="e3abc-128">**DomainResponse**要素の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e3abc-128">Contains an array of **DomainResponse** elements.</span></span> <span data-ttu-id="e3abc-129">**DomainResponse**の各要素には、指定したユーザーの要求された設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e3abc-129">Each **DomainResponse** element contains the requested settings for the specified user.</span></span>  <br/> |
|[<span data-ttu-id="e3abc-130">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3abc-130">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="e3abc-131">ドメインごとの応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e3abc-131">Contains the responses for each domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e3abc-132">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e3abc-132">Text value</span></span>

<span data-ttu-id="e3abc-133">なし。</span><span class="sxs-lookup"><span data-stu-id="e3abc-133">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3abc-134">要素情報</span><span class="sxs-lookup"><span data-stu-id="e3abc-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3abc-135">名前空間</span><span class="sxs-lookup"><span data-stu-id="e3abc-135">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="e3abc-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e3abc-136">Schema Name</span></span>  <br/> |<span data-ttu-id="e3abc-137">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="e3abc-137">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="e3abc-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e3abc-138">Validation File</span></span>  <br/> |<span data-ttu-id="e3abc-139">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e3abc-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e3abc-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e3abc-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="e3abc-141">True</span><span class="sxs-lookup"><span data-stu-id="e3abc-141">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e3abc-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="e3abc-142">See also</span></span>

- [<span data-ttu-id="e3abc-143">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="e3abc-143">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

