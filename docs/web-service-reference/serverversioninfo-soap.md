---
title: ServerVersionInfo (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 8662647b-e50a-4774-9ba3-a951ae6df781
description: ServerVersionInfo 要素には、要求を処理したサーバーのバージョンが含まれています。
ms.openlocfilehash: b02071e4997aba91fb538d52df2612fe6fd32800
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833385"
---
# <a name="serverversioninfo-soap"></a><span data-ttu-id="41d65-103">ServerVersionInfo (SOAP)</span><span class="sxs-lookup"><span data-stu-id="41d65-103">ServerVersionInfo (SOAP)</span></span>

<span data-ttu-id="41d65-104">**ServerVersionInfo**要素には、要求を処理したサーバーのバージョンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="41d65-104">The **ServerVersionInfo** element contains the version of the server that processed the request.</span></span> 
  
```XML
<ServerVersionInfo>
   <MajorVersion/>
   <MinorVersion/>
   <MajorBuildNumber/>
   <MinorBuildNumber/>
   <Version/>
</ServerVersionInfo>
```

 <span data-ttu-id="41d65-105">**ServerVersionInfo**</span><span class="sxs-lookup"><span data-stu-id="41d65-105">**ServerVersionInfo**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="41d65-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="41d65-106">Attributes and elements</span></span>

<span data-ttu-id="41d65-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="41d65-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41d65-108">属性</span><span class="sxs-lookup"><span data-stu-id="41d65-108">Attributes</span></span>

<span data-ttu-id="41d65-109">なし。</span><span class="sxs-lookup"><span data-stu-id="41d65-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="41d65-110">子要素</span><span class="sxs-lookup"><span data-stu-id="41d65-110">Child elements</span></span>

|<span data-ttu-id="41d65-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="41d65-111">**Element**</span></span>|<span data-ttu-id="41d65-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="41d65-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41d65-113">MajorVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="41d65-113">MajorVersion (SOAP)</span></span>](majorversion-soap.md) <br/> |<span data-ttu-id="41d65-114">サーバーのメジャー バージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="41d65-114">The major version number for the server.</span></span>  <br/> |
|[<span data-ttu-id="41d65-115">マイナー バージョン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="41d65-115">MinorVersion (SOAP)</span></span>](minorversion-soap.md) <br/> |<span data-ttu-id="41d65-116">サーバーのマイナー バージョン番号です。</span><span class="sxs-lookup"><span data-stu-id="41d65-116">The minor version number for the server.</span></span>  <br/> |
|[<span data-ttu-id="41d65-117">MajorBuildNumber (SOAP)</span><span class="sxs-lookup"><span data-stu-id="41d65-117">MajorBuildNumber (SOAP)</span></span>](majorbuildnumber-soap.md) <br/> |<span data-ttu-id="41d65-118">サーバーのメジャー ビルド番号。</span><span class="sxs-lookup"><span data-stu-id="41d65-118">The major build number for the server.</span></span>  <br/> |
|[<span data-ttu-id="41d65-119">MinorBuildNumber (SOAP)</span><span class="sxs-lookup"><span data-stu-id="41d65-119">MinorBuildNumber (SOAP)</span></span>](minorbuildnumber-soap.md) <br/> |<span data-ttu-id="41d65-120">サーバーのマイナー ビルド番号。</span><span class="sxs-lookup"><span data-stu-id="41d65-120">The minor build number for the server.</span></span>  <br/> |
|[<span data-ttu-id="41d65-121">バージョン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="41d65-121">Version (SOAP)</span></span>](version-soap.md) <br/> |<span data-ttu-id="41d65-122">サーバー製品のバージョンの説明です。</span><span class="sxs-lookup"><span data-stu-id="41d65-122">A description of the server product version.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="41d65-123">親要素</span><span class="sxs-lookup"><span data-stu-id="41d65-123">Parent elements</span></span>

<span data-ttu-id="41d65-124">なし。</span><span class="sxs-lookup"><span data-stu-id="41d65-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="41d65-125">備考</span><span class="sxs-lookup"><span data-stu-id="41d65-125">Remarks</span></span>

<span data-ttu-id="41d65-126">この要素は、SOAP ヘッダーで返されます。</span><span class="sxs-lookup"><span data-stu-id="41d65-126">This element is returned in the SOAP header.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="41d65-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="41d65-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41d65-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="41d65-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="41d65-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="41d65-129">Schema Name</span></span>  <br/> |<span data-ttu-id="41d65-130">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="41d65-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="41d65-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="41d65-131">Validation File</span></span>  <br/> |<span data-ttu-id="41d65-132">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="41d65-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="41d65-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="41d65-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="41d65-134">True</span><span class="sxs-lookup"><span data-stu-id="41d65-134">True</span></span>  <br/> |
   

