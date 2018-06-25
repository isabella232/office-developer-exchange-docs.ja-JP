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
description: RequestServerVersion 要素には、要求の対象とするスキーマのバージョンを識別するバージョン情報が含まれています。
ms.openlocfilehash: 0092d90a5fc479363f6d774b793c7148ad29f21c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833143"
---
# <a name="requestserverversion"></a><span data-ttu-id="d81c6-103">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="d81c6-103">RequestServerVersion</span></span>

<span data-ttu-id="d81c6-104">**RequestServerVersion**要素には、要求の対象とするスキーマのバージョンを識別するバージョン情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d81c6-104">The **RequestServerVersion** element contains the versioning information that identifies the schema version to target for a request.</span></span> 
  
```XML
<RequestServerVersion Version=""/>
```

 <span data-ttu-id="d81c6-105">**ExchangeVersionType**</span><span class="sxs-lookup"><span data-stu-id="d81c6-105">**ExchangeVersionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d81c6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d81c6-106">Attributes and elements</span></span>

<span data-ttu-id="d81c6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d81c6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d81c6-108">属性</span><span class="sxs-lookup"><span data-stu-id="d81c6-108">Attributes</span></span>

|<span data-ttu-id="d81c6-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="d81c6-109">**Attribute**</span></span>|<span data-ttu-id="d81c6-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="d81c6-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d81c6-111">バージョン</span><span class="sxs-lookup"><span data-stu-id="d81c6-111">Version</span></span>  <br/> |<span data-ttu-id="d81c6-112">要求の対象とするバージョンをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="d81c6-112">Describes the version to target for the request.</span></span> <span data-ttu-id="d81c6-113">対象サーバーのバージョンのバージョンの Exchange が Exchange Server 2010 で始まる場合、この属性が必要です。</span><span class="sxs-lookup"><span data-stu-id="d81c6-113">This attribute is required when the target server version is a version of Exchange starting with Exchange Server 2010.</span></span>  <br/> |
   
#### <a name="version-attribute-values"></a><span data-ttu-id="d81c6-114">バージョン属性の値</span><span class="sxs-lookup"><span data-stu-id="d81c6-114">Version attribute values</span></span>

|<span data-ttu-id="d81c6-115">**値**</span><span class="sxs-lookup"><span data-stu-id="d81c6-115">**Value**</span></span>|<span data-ttu-id="d81c6-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="d81c6-116">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d81c6-117">Exchange2007</span><span class="sxs-lookup"><span data-stu-id="d81c6-117">Exchange2007</span></span>  <br/> |<span data-ttu-id="d81c6-118">初期リリース版の Exchange 2007 用のスキーマ ファイルを対象とします。</span><span class="sxs-lookup"><span data-stu-id="d81c6-118">Target the schema files for the initial release version of Exchange 2007.</span></span>  <br/> |
|<span data-ttu-id="d81c6-119">Exchange2007_SP1</span><span class="sxs-lookup"><span data-stu-id="d81c6-119">Exchange2007_SP1</span></span>  <br/> |<span data-ttu-id="d81c6-120">Exchange 2007 Service Pack 1 (SP1)、Exchange 2007 Service Pack 2 (SP2)、および Exchange 2007 Service Pack 3 (SP3) 用のスキーマ ファイルを対象とします。</span><span class="sxs-lookup"><span data-stu-id="d81c6-120">Target the schema files for Exchange 2007 Service Pack 1 (SP1), Exchange 2007 Service Pack 2 (SP2), and Exchange 2007 Service Pack 3 (SP3).</span></span>  <br/> |
|<span data-ttu-id="d81c6-121">Exchange2010</span><span class="sxs-lookup"><span data-stu-id="d81c6-121">Exchange2010</span></span>  <br/> |<span data-ttu-id="d81c6-122">Exchange 2010 用のスキーマ ファイルを対象とします。</span><span class="sxs-lookup"><span data-stu-id="d81c6-122">Target the schema files for Exchange 2010.</span></span>  <br/> |
|<span data-ttu-id="d81c6-123">Exchange2010_SP1</span><span class="sxs-lookup"><span data-stu-id="d81c6-123">Exchange2010_SP1</span></span>  <br/> |<span data-ttu-id="d81c6-124">Exchange 2010 Service Pack 1 (SP1) 用のスキーマ ファイルを対象とします。</span><span class="sxs-lookup"><span data-stu-id="d81c6-124">Target the schema files for Exchange 2010 Service Pack 1 (SP1).</span></span>  <br/> |
|<span data-ttu-id="d81c6-125">Exchange2010_SP2</span><span class="sxs-lookup"><span data-stu-id="d81c6-125">Exchange2010_SP2</span></span>  <br/> |<span data-ttu-id="d81c6-126">Exchange 2010 Service Pack 2 (SP2) および Exchange 2010 Service Pack 3 (SP3) 用のスキーマ ファイルを対象とします。</span><span class="sxs-lookup"><span data-stu-id="d81c6-126">Target the schema files for Exchange 2010 Service Pack 2 (SP2) and Exchange 2010 Service Pack 3 (SP3).</span></span>  <br/> |
|<span data-ttu-id="d81c6-127">Exchange2013</span><span class="sxs-lookup"><span data-stu-id="d81c6-127">Exchange2013</span></span>  <br/> |<span data-ttu-id="d81c6-128">Exchange 2013 のスキーマ ファイルを対象とします。</span><span class="sxs-lookup"><span data-stu-id="d81c6-128">Target the schema files for Exchange 2013.</span></span>  <br/> |
|<span data-ttu-id="d81c6-129">Exchange2013_SP1</span><span class="sxs-lookup"><span data-stu-id="d81c6-129">Exchange2013_SP1</span></span>  <br/> |<span data-ttu-id="d81c6-130">Exchange 2013 の Service Pack 1 (SP1) 用のスキーマ ファイルを対象とします。</span><span class="sxs-lookup"><span data-stu-id="d81c6-130">Target the schema files for Exchange 2013 Service Pack 1 (SP1).</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d81c6-131">子要素</span><span class="sxs-lookup"><span data-stu-id="d81c6-131">Child elements</span></span>

<span data-ttu-id="d81c6-132">なし。</span><span class="sxs-lookup"><span data-stu-id="d81c6-132">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d81c6-133">親要素</span><span class="sxs-lookup"><span data-stu-id="d81c6-133">Parent elements</span></span>

<span data-ttu-id="d81c6-134">**RequestServerVersion**要素は、SOAP ヘッダーに配置されます。</span><span class="sxs-lookup"><span data-stu-id="d81c6-134">The **RequestServerVersion** element is located in the SOAP header.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d81c6-135">備考</span><span class="sxs-lookup"><span data-stu-id="d81c6-135">Remarks</span></span>

<span data-ttu-id="d81c6-136">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d81c6-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d81c6-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="d81c6-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d81c6-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="d81c6-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d81c6-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d81c6-139">Schema Name</span></span>  <br/> |<span data-ttu-id="d81c6-140">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d81c6-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="d81c6-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d81c6-141">Validation File</span></span>  <br/> |<span data-ttu-id="d81c6-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d81c6-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d81c6-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d81c6-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="d81c6-144">False</span><span class="sxs-lookup"><span data-stu-id="d81c6-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d81c6-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="d81c6-145">See also</span></span>



- [<span data-ttu-id="d81c6-146">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d81c6-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="d81c6-147">バージョン管理の要求</span><span class="sxs-lookup"><span data-stu-id="d81c6-147">Versioning Requests</span></span>](http://msdn.microsoft.com/library/76877b0a-d2e5-4c74-9295-7b445a41d46a%28Office.15%29.aspx)

