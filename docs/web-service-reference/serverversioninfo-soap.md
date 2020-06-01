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
ms.openlocfilehash: b54b4833361ec78c7f8213473af4638965c7ddae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467649"
---
# <a name="serverversioninfo-soap"></a><span data-ttu-id="73eaf-103">ServerVersionInfo (SOAP)</span><span class="sxs-lookup"><span data-stu-id="73eaf-103">ServerVersionInfo (SOAP)</span></span>

<span data-ttu-id="73eaf-104">**ServerVersionInfo**要素には、要求を処理したサーバーのバージョンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="73eaf-104">The **ServerVersionInfo** element contains the version of the server that processed the request.</span></span> 
  
```XML
<ServerVersionInfo>
   <MajorVersion/>
   <MinorVersion/>
   <MajorBuildNumber/>
   <MinorBuildNumber/>
   <Version/>
</ServerVersionInfo>
```

 <span data-ttu-id="73eaf-105">**ServerVersionInfo**</span><span class="sxs-lookup"><span data-stu-id="73eaf-105">**ServerVersionInfo**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="73eaf-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="73eaf-106">Attributes and elements</span></span>

<span data-ttu-id="73eaf-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="73eaf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="73eaf-108">属性</span><span class="sxs-lookup"><span data-stu-id="73eaf-108">Attributes</span></span>

<span data-ttu-id="73eaf-109">なし。</span><span class="sxs-lookup"><span data-stu-id="73eaf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="73eaf-110">子要素</span><span class="sxs-lookup"><span data-stu-id="73eaf-110">Child elements</span></span>

|<span data-ttu-id="73eaf-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="73eaf-111">**Element**</span></span>|<span data-ttu-id="73eaf-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="73eaf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="73eaf-113">MajorVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="73eaf-113">MajorVersion (SOAP)</span></span>](majorversion-soap.md) <br/> |<span data-ttu-id="73eaf-114">サーバーのメジャーバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="73eaf-114">The major version number for the server.</span></span>  <br/> |
|[<span data-ttu-id="73eaf-115">MinorVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="73eaf-115">MinorVersion (SOAP)</span></span>](minorversion-soap.md) <br/> |<span data-ttu-id="73eaf-116">サーバーのマイナーバージョン番号。</span><span class="sxs-lookup"><span data-stu-id="73eaf-116">The minor version number for the server.</span></span>  <br/> |
|[<span data-ttu-id="73eaf-117">MajorBuildNumber (SOAP)</span><span class="sxs-lookup"><span data-stu-id="73eaf-117">MajorBuildNumber (SOAP)</span></span>](majorbuildnumber-soap.md) <br/> |<span data-ttu-id="73eaf-118">サーバーのメジャービルド番号。</span><span class="sxs-lookup"><span data-stu-id="73eaf-118">The major build number for the server.</span></span>  <br/> |
|[<span data-ttu-id="73eaf-119">MinorBuildNumber/(SOAP)</span><span class="sxs-lookup"><span data-stu-id="73eaf-119">MinorBuildNumber (SOAP)</span></span>](minorbuildnumber-soap.md) <br/> |<span data-ttu-id="73eaf-120">サーバーのマイナービルド番号。</span><span class="sxs-lookup"><span data-stu-id="73eaf-120">The minor build number for the server.</span></span>  <br/> |
|[<span data-ttu-id="73eaf-121">バージョン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="73eaf-121">Version (SOAP)</span></span>](version-soap.md) <br/> |<span data-ttu-id="73eaf-122">サーバー製品バージョンの説明。</span><span class="sxs-lookup"><span data-stu-id="73eaf-122">A description of the server product version.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="73eaf-123">親要素</span><span class="sxs-lookup"><span data-stu-id="73eaf-123">Parent elements</span></span>

<span data-ttu-id="73eaf-124">なし。</span><span class="sxs-lookup"><span data-stu-id="73eaf-124">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="73eaf-125">注釈</span><span class="sxs-lookup"><span data-stu-id="73eaf-125">Remarks</span></span>

<span data-ttu-id="73eaf-126">この要素は、SOAP ヘッダーで返されます。</span><span class="sxs-lookup"><span data-stu-id="73eaf-126">This element is returned in the SOAP header.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="73eaf-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="73eaf-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="73eaf-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="73eaf-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="73eaf-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="73eaf-129">Schema Name</span></span>  <br/> |<span data-ttu-id="73eaf-130">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="73eaf-130">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="73eaf-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="73eaf-131">Validation File</span></span>  <br/> |<span data-ttu-id="73eaf-132">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="73eaf-132">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="73eaf-133">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="73eaf-133">Can be Empty</span></span>  <br/> |<span data-ttu-id="73eaf-134">はい</span><span class="sxs-lookup"><span data-stu-id="73eaf-134">True</span></span>  <br/> |
   

