---
title: GetDomainSettingsResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 43ebd17b-3a70-4878-9254-97a4c2c87b77
description: GetDomainSettingsResponse 要素は、GetDomainSettings 操作 (SOAP) への応答を表します。これにより、ドメインの設定が返されます。
ms.openlocfilehash: 94cb202948e6a0d5a34f5547132c052d1d1b6a40
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461878"
---
# <a name="getdomainsettingsresponse-soap"></a><span data-ttu-id="f0468-103">GetDomainSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f0468-103">GetDomainSettingsResponse (SOAP)</span></span>

<span data-ttu-id="f0468-104">**Getdomainsettingsresponse**要素は、 [getdomainsettings 操作 (SOAP)](getdomainsettings-operation-soap.md)への応答を表します。これにより、ドメインの設定が返されます。</span><span class="sxs-lookup"><span data-stu-id="f0468-104">The **GetDomainSettingsResponse** element represents the response to a [GetDomainSettings operation (SOAP)](getdomainsettings-operation-soap.md), which returns the domain settings.</span></span>
  
```XML
<GetDomainSettingsResponse>
   <DomainResponses/>
   <ErrorCode/>
   <ErrorMessage/>
</GetDomainSettingsResponse>
```

 <span data-ttu-id="f0468-105">**GetDomainSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="f0468-105">**GetDomainSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0468-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f0468-106">Attributes and elements</span></span>

<span data-ttu-id="f0468-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f0468-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0468-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0468-108">Attributes</span></span>

<span data-ttu-id="f0468-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f0468-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f0468-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f0468-110">Child elements</span></span>

|<span data-ttu-id="f0468-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="f0468-111">**Element**</span></span>|<span data-ttu-id="f0468-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f0468-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0468-113">DomainResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f0468-113">DomainResponses (SOAP)</span></span>](domainresponses-soap.md) <br/> |<span data-ttu-id="f0468-114">要求された各ドメインの設定に対する応答の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="f0468-114">Contains an array of responses for each requested domain's settings.</span></span>  <br/> |
|[<span data-ttu-id="f0468-115">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f0468-115">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="f0468-116">自動検出サービスによって返されるエラーコードを表します。</span><span class="sxs-lookup"><span data-stu-id="f0468-116">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="f0468-117">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f0468-117">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="f0468-118">自動検出サービスによって返されるエラーコードに関連付けられているメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="f0468-118">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f0468-119">親要素</span><span class="sxs-lookup"><span data-stu-id="f0468-119">Parent elements</span></span>

<span data-ttu-id="f0468-120">なし。</span><span class="sxs-lookup"><span data-stu-id="f0468-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f0468-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f0468-121">Text value</span></span>

<span data-ttu-id="f0468-122">なし。</span><span class="sxs-lookup"><span data-stu-id="f0468-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0468-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f0468-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0468-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="f0468-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="f0468-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f0468-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f0468-126">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="f0468-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="f0468-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f0468-127">Validation File</span></span>  <br/> |<span data-ttu-id="f0468-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="f0468-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f0468-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f0468-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="f0468-130">正しい</span><span class="sxs-lookup"><span data-stu-id="f0468-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0468-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="f0468-131">See also</span></span>



[<span data-ttu-id="f0468-132">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="f0468-132">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

