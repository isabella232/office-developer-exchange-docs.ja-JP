---
title: MajorBuildNumber (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 7335b1c1-0b47-4452-a8cb-d19cddcfc281
description: MajorBuildNumber 要素は、サーバーの主要なビルド番号を表します。
ms.openlocfilehash: 2d6520b65f75c9fa14d236c99e96523baa3ddfb5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832329"
---
# <a name="majorbuildnumber-soap"></a><span data-ttu-id="cdbd1-103">MajorBuildNumber (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cdbd1-103">MajorBuildNumber (SOAP)</span></span>

<span data-ttu-id="cdbd1-104">**MajorBuildNumber**要素は、サーバーの主要なビルド番号を表します。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-104">The **MajorBuildNumber** element represents major build number for the server.</span></span> 
  
```XML
<MajorBuildNumber/>
```

 <span data-ttu-id="cdbd1-105">**xs:int**</span><span class="sxs-lookup"><span data-stu-id="cdbd1-105">**xs:int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cdbd1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cdbd1-106">Attributes and elements</span></span>

<span data-ttu-id="cdbd1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cdbd1-108">属性</span><span class="sxs-lookup"><span data-stu-id="cdbd1-108">Attributes</span></span>

<span data-ttu-id="cdbd1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cdbd1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cdbd1-110">Child elements</span></span>

<span data-ttu-id="cdbd1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cdbd1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="cdbd1-112">Parent elements</span></span>

|<span data-ttu-id="cdbd1-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="cdbd1-113">**Element**</span></span>|<span data-ttu-id="cdbd1-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="cdbd1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cdbd1-115">ServerVersionInfo (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cdbd1-115">ServerVersionInfo (SOAP)</span></span>](serverversioninfo-soap.md) <br/> |<span data-ttu-id="cdbd1-116">要求を処理したサーバーのバージョンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-116">Contains the version of the server that processed the request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cdbd1-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cdbd1-117">Text value</span></span>

<span data-ttu-id="cdbd1-118">MajorBuildNumber 要素のテキスト値は、メジャー番号を表す整数値が要求を処理するサーバーの数を構築します。</span><span class="sxs-lookup"><span data-stu-id="cdbd1-118">The text value of the MajorBuildNumber element is an integer that represents the major build number of the server that processed the request.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cdbd1-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="cdbd1-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cdbd1-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="cdbd1-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="cdbd1-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cdbd1-121">Schema Name</span></span>  <br/> |<span data-ttu-id="cdbd1-122">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="cdbd1-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="cdbd1-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cdbd1-123">Validation File</span></span>  <br/> |<span data-ttu-id="cdbd1-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cdbd1-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cdbd1-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cdbd1-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="cdbd1-126">True</span><span class="sxs-lookup"><span data-stu-id="cdbd1-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cdbd1-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="cdbd1-127">See also</span></span>



[<span data-ttu-id="cdbd1-128">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cdbd1-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="cdbd1-129">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cdbd1-129">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="cdbd1-130">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="cdbd1-130">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

