---
title: バージョン (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 47c9216e-6bfe-48c8-a27a-26f70db8e8d5
description: バージョン要素は、サーバー製品のバージョンの説明を表します。
ms.openlocfilehash: b8284880646cb82e6af6715523467021f080b8e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839993"
---
# <a name="version-soap"></a><span data-ttu-id="8d4a9-103">バージョン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8d4a9-103">Version (SOAP)</span></span>

<span data-ttu-id="8d4a9-104">**バージョン**要素は、サーバー製品のバージョンの説明を表します。</span><span class="sxs-lookup"><span data-stu-id="8d4a9-104">The **Version** element represents a description of the server product version.</span></span> 
  
```XML
<Version/>
```

 <span data-ttu-id="8d4a9-105">**string**</span><span class="sxs-lookup"><span data-stu-id="8d4a9-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8d4a9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8d4a9-106">Attributes and elements</span></span>

<span data-ttu-id="8d4a9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8d4a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d4a9-108">属性</span><span class="sxs-lookup"><span data-stu-id="8d4a9-108">Attributes</span></span>

<span data-ttu-id="8d4a9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8d4a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d4a9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8d4a9-110">Child elements</span></span>

<span data-ttu-id="8d4a9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8d4a9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8d4a9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8d4a9-112">Parent elements</span></span>

|<span data-ttu-id="8d4a9-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8d4a9-113">**Element**</span></span>|<span data-ttu-id="8d4a9-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8d4a9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d4a9-115">ServerVersionInfo (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8d4a9-115">ServerVersionInfo (SOAP)</span></span>](serverversioninfo-soap.md) <br/> |<span data-ttu-id="8d4a9-116">要求を処理したサーバーのバージョンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8d4a9-116">Contains the version of the server that processed the request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8d4a9-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8d4a9-117">Text value</span></span>

<span data-ttu-id="8d4a9-118">**バージョン**の要素の値は、サーバー製品のバージョンの説明です。</span><span class="sxs-lookup"><span data-stu-id="8d4a9-118">The value of the **Version** element is a description of the server product version.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8d4a9-119">備考</span><span class="sxs-lookup"><span data-stu-id="8d4a9-119">Remarks</span></span>

<span data-ttu-id="8d4a9-120">**バージョン**要素は、応答の SOAP ヘッダーに含まれます。</span><span class="sxs-lookup"><span data-stu-id="8d4a9-120">The **Version** element is contained in the SOAP header of a response.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="8d4a9-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="8d4a9-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d4a9-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="8d4a9-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="8d4a9-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8d4a9-123">Schema Name</span></span>  <br/> |<span data-ttu-id="8d4a9-124">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="8d4a9-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="8d4a9-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8d4a9-125">Validation File</span></span>  <br/> |<span data-ttu-id="8d4a9-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8d4a9-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8d4a9-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8d4a9-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="8d4a9-128">True</span><span class="sxs-lookup"><span data-stu-id="8d4a9-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8d4a9-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="8d4a9-129">See also</span></span>



[<span data-ttu-id="8d4a9-130">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8d4a9-130">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="8d4a9-131">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8d4a9-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="8d4a9-132">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="8d4a9-132">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

