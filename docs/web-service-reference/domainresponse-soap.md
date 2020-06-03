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
description: DomainResponse 要素には、指定されたドメインに対して要求された設定が含まれています。
ms.openlocfilehash: dea6e36c51ceea53201b668cfba616c03a44df86
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456963"
---
# <a name="domainresponse-soap"></a><span data-ttu-id="6ea96-103">DomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6ea96-103">DomainResponse (SOAP)</span></span>

<span data-ttu-id="6ea96-104">**Domainresponse**要素には、指定されたドメインに対して要求された設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6ea96-104">The **DomainResponse** element contains the requested settings for the specified domain.</span></span> 
  
```XML
<DomainResponse>
   <DomainSettingErrors/>
   <DomainSettings/>
   <RedirectTarget/>
   <ErrorCode/>
   <ErrorMessage/>
</DomainResponse>
```

 <span data-ttu-id="6ea96-105">**DomainResponse**</span><span class="sxs-lookup"><span data-stu-id="6ea96-105">**DomainResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6ea96-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6ea96-106">Attributes and elements</span></span>

<span data-ttu-id="6ea96-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6ea96-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6ea96-108">属性</span><span class="sxs-lookup"><span data-stu-id="6ea96-108">Attributes</span></span>

<span data-ttu-id="6ea96-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6ea96-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6ea96-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6ea96-110">Child elements</span></span>

|<span data-ttu-id="6ea96-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="6ea96-111">**Element**</span></span>|<span data-ttu-id="6ea96-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6ea96-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ea96-113">DomainSettingErrors (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6ea96-113">DomainSettingErrors (SOAP)</span></span>](domainsettingerrors-soap.md) <br/> |<span data-ttu-id="6ea96-114">返すことができなかった設定に関するエラー情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6ea96-114">Contains error information for settings that could not be returned.</span></span>  <br/> |
|[<span data-ttu-id="6ea96-115">DomainSettings (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6ea96-115">DomainSettings (SOAP)</span></span>](domainsettings-soap.md) <br/> |<span data-ttu-id="6ea96-116">自動検出要求で送信された、または自動検出応答によって返されたドメイン設定を表します。</span><span class="sxs-lookup"><span data-stu-id="6ea96-116">Represents the domain settings that were submitted in an Autodiscover request or returned by an Autodiscover response.</span></span>  <br/> |
|[<span data-ttu-id="6ea96-117">RedirectTarget (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6ea96-117">RedirectTarget (SOAP)</span></span>](redirecttarget-soap.md) <br/> |<span data-ttu-id="6ea96-118">リダイレクトのターゲットを識別します。</span><span class="sxs-lookup"><span data-stu-id="6ea96-118">Identifies the target of the redirection.</span></span> <span data-ttu-id="6ea96-119">ターゲットには、URL または電子メールアドレスのいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="6ea96-119">The target can be either a URL or an e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="6ea96-120">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6ea96-120">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="6ea96-121">特定の要求に関連付けられているエラーコードを指定します。</span><span class="sxs-lookup"><span data-stu-id="6ea96-121">Specifies the error code that is associated with the specific request.</span></span>  <br/> |
|[<span data-ttu-id="6ea96-122">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6ea96-122">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="6ea96-123">特定の要求に関連付けられているエラーメッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="6ea96-123">Specifies the error message that is associated with the specific request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6ea96-124">親要素</span><span class="sxs-lookup"><span data-stu-id="6ea96-124">Parent elements</span></span>

|<span data-ttu-id="6ea96-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="6ea96-125">**Element**</span></span>|<span data-ttu-id="6ea96-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="6ea96-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6ea96-127">ArrayOfDomainResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6ea96-127">ArrayOfDomainResponse (SOAP)</span></span>](arrayofdomainresponse-soap.md) <br/> |<span data-ttu-id="6ea96-128">**Domainresponse**要素の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="6ea96-128">Contains an array of **DomainResponse** elements.</span></span> <span data-ttu-id="6ea96-129">各**Domainresponse**要素には、指定されたユーザーに対して要求された設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6ea96-129">Each **DomainResponse** element contains the requested settings for the specified user.</span></span>  <br/> |
|[<span data-ttu-id="6ea96-130">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6ea96-130">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="6ea96-131">各ドメインの応答を含みます。</span><span class="sxs-lookup"><span data-stu-id="6ea96-131">Contains the responses for each domain.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6ea96-132">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6ea96-132">Text value</span></span>

<span data-ttu-id="6ea96-133">なし。</span><span class="sxs-lookup"><span data-stu-id="6ea96-133">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6ea96-134">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6ea96-134">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6ea96-135">Namespace</span><span class="sxs-lookup"><span data-stu-id="6ea96-135">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="6ea96-136">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6ea96-136">Schema Name</span></span>  <br/> |<span data-ttu-id="6ea96-137">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="6ea96-137">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="6ea96-138">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6ea96-138">Validation File</span></span>  <br/> |<span data-ttu-id="6ea96-139">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="6ea96-139">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6ea96-140">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6ea96-140">Can be Empty</span></span>  <br/> |<span data-ttu-id="6ea96-141">正しい</span><span class="sxs-lookup"><span data-stu-id="6ea96-141">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6ea96-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="6ea96-142">See also</span></span>

- [<span data-ttu-id="6ea96-143">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6ea96-143">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

