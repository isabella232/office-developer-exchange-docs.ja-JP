---
title: RequestServerVersion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RequestServerVersion
api_type:
- schema
ms.assetid: af4032d5-42b3-463e-9d0a-8236d78e5b75
description: RequestServerVersion 要素には、要求に対してターゲットとするスキーマバージョンを識別するバージョン管理情報が含まれています。
ms.openlocfilehash: c4ae59a03c812d21153e4338734185d933d914ec
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468321"
---
# <a name="requestserverversion"></a><span data-ttu-id="1ad4b-103">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="1ad4b-103">RequestServerVersion</span></span>

<span data-ttu-id="1ad4b-104">**RequestServerVersion**要素には、要求に対してターゲットとするスキーマバージョンを識別するバージョン管理情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1ad4b-104">The **RequestServerVersion** element contains the versioning information that identifies the schema version to target for a request.</span></span> 
  
```XML
<RequestServerVersion Version=""/>
```

 <span data-ttu-id="1ad4b-105">**ExchangeVersionType**</span><span class="sxs-lookup"><span data-stu-id="1ad4b-105">**ExchangeVersionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ad4b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1ad4b-106">Attributes and elements</span></span>

<span data-ttu-id="1ad4b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1ad4b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ad4b-108">属性</span><span class="sxs-lookup"><span data-stu-id="1ad4b-108">Attributes</span></span>

|<span data-ttu-id="1ad4b-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="1ad4b-109">**Attribute**</span></span>|<span data-ttu-id="1ad4b-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ad4b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1ad4b-111">Version</span><span class="sxs-lookup"><span data-stu-id="1ad4b-111">Version</span></span>  <br/> |<span data-ttu-id="1ad4b-112">要求の対象となるバージョンを示します。</span><span class="sxs-lookup"><span data-stu-id="1ad4b-112">Describes the version to target for the request.</span></span> <span data-ttu-id="1ad4b-113">この属性は、ターゲットサーバーのバージョンが Exchange Server 2010 以降の Exchange のバージョンである場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="1ad4b-113">This attribute is required when the target server version is a version of Exchange starting with Exchange Server 2010.</span></span>  <br/> |
   
#### <a name="version-attribute-values"></a><span data-ttu-id="1ad4b-114">バージョン属性の値</span><span class="sxs-lookup"><span data-stu-id="1ad4b-114">Version attribute values</span></span>

|<span data-ttu-id="1ad4b-115">**値**</span><span class="sxs-lookup"><span data-stu-id="1ad4b-115">**Value**</span></span>|<span data-ttu-id="1ad4b-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ad4b-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1ad4b-117">Exchange2007</span><span class="sxs-lookup"><span data-stu-id="1ad4b-117">Exchange2007</span></span>  <br/> |<span data-ttu-id="1ad4b-118">Exchange 2007 の最初のリリースバージョンのスキーマファイルをターゲットにします。</span><span class="sxs-lookup"><span data-stu-id="1ad4b-118">Target the schema files for the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="1ad4b-119">Exchange2007_SP1</span><span class="sxs-lookup"><span data-stu-id="1ad4b-119">Exchange2007_SP1</span></span>  <br/> |<span data-ttu-id="1ad4b-120">Exchange 2007 Service Pack 1 (SP1)、Exchange 2007 Service Pack 2 (SP2)、および Exchange 2007 Service Pack 3 (SP3) のスキーマファイルを対象とします。</span><span class="sxs-lookup"><span data-stu-id="1ad4b-120">Target the schema files for Exchange 2007 Service Pack 1 (SP1), Exchange 2007 Service Pack 2 (SP2), and Exchange 2007 Service Pack 3 (SP3).</span></span>  <br/> |
|<span data-ttu-id="1ad4b-121">Exchange2010</span><span class="sxs-lookup"><span data-stu-id="1ad4b-121">Exchange2010</span></span>  <br/> |<span data-ttu-id="1ad4b-122">Exchange 2010 のスキーマファイルをターゲットにします。</span><span class="sxs-lookup"><span data-stu-id="1ad4b-122">Target the schema files for Exchange 2010.</span></span>  <br/> |
|<span data-ttu-id="1ad4b-123">Exchange2010_SP1</span><span class="sxs-lookup"><span data-stu-id="1ad4b-123">Exchange2010_SP1</span></span>  <br/> |<span data-ttu-id="1ad4b-124">Exchange 2010 Service Pack 1 (SP1) のスキーマファイルをターゲットにします。</span><span class="sxs-lookup"><span data-stu-id="1ad4b-124">Target the schema files for Exchange 2010 Service Pack 1 (SP1).</span></span>  <br/> |
|<span data-ttu-id="1ad4b-125">Exchange2010_SP2</span><span class="sxs-lookup"><span data-stu-id="1ad4b-125">Exchange2010_SP2</span></span>  <br/> |<span data-ttu-id="1ad4b-126">Exchange 2010 Service Pack 2 (SP2) および Exchange 2010 Service Pack 3 (SP3) のスキーマファイルを対象とします。</span><span class="sxs-lookup"><span data-stu-id="1ad4b-126">Target the schema files for Exchange 2010 Service Pack 2 (SP2) and Exchange 2010 Service Pack 3 (SP3).</span></span>  <br/> |
|<span data-ttu-id="1ad4b-127">Exchange2013</span><span class="sxs-lookup"><span data-stu-id="1ad4b-127">Exchange2013</span></span>  <br/> |<span data-ttu-id="1ad4b-128">Exchange 2013 のスキーマファイルをターゲットにします。</span><span class="sxs-lookup"><span data-stu-id="1ad4b-128">Target the schema files for Exchange 2013.</span></span>  <br/> |
|<span data-ttu-id="1ad4b-129">Exchange2013_SP1</span><span class="sxs-lookup"><span data-stu-id="1ad4b-129">Exchange2013_SP1</span></span>  <br/> |<span data-ttu-id="1ad4b-130">Exchange 2013 Service Pack 1 (SP1) のスキーマファイルをターゲットにします。</span><span class="sxs-lookup"><span data-stu-id="1ad4b-130">Target the schema files for Exchange 2013 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1ad4b-131">子要素</span><span class="sxs-lookup"><span data-stu-id="1ad4b-131">Child elements</span></span>

<span data-ttu-id="1ad4b-132">なし。</span><span class="sxs-lookup"><span data-stu-id="1ad4b-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1ad4b-133">親要素</span><span class="sxs-lookup"><span data-stu-id="1ad4b-133">Parent elements</span></span>

<span data-ttu-id="1ad4b-134">**RequestServerVersion**要素は、SOAP ヘッダーにあります。</span><span class="sxs-lookup"><span data-stu-id="1ad4b-134">The **RequestServerVersion** element is located in the SOAP header.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1ad4b-135">注釈</span><span class="sxs-lookup"><span data-stu-id="1ad4b-135">Remarks</span></span>

<span data-ttu-id="1ad4b-136">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1ad4b-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ad4b-137">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1ad4b-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ad4b-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="1ad4b-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1ad4b-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1ad4b-139">Schema Name</span></span>  <br/> |<span data-ttu-id="1ad4b-140">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="1ad4b-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="1ad4b-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1ad4b-141">Validation File</span></span>  <br/> |<span data-ttu-id="1ad4b-142">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1ad4b-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1ad4b-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1ad4b-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="1ad4b-144">正しくない</span><span class="sxs-lookup"><span data-stu-id="1ad4b-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ad4b-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="1ad4b-145">See also</span></span>



- [<span data-ttu-id="1ad4b-146">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1ad4b-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="1ad4b-147">バージョン管理要求</span><span class="sxs-lookup"><span data-stu-id="1ad4b-147">Versioning Requests</span></span>](https://msdn.microsoft.com/library/76877b0a-d2e5-4c74-9295-7b445a41d46a%28Office.15%29.aspx)

