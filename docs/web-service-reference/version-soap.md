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
description: Version 要素は、サーバー製品バージョンの説明を表します。
ms.openlocfilehash: d7e6983c837b2818b7d11e1777015ec583968242
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44531029"
---
# <a name="version-soap"></a><span data-ttu-id="aa3dd-103">バージョン (SOAP)</span><span class="sxs-lookup"><span data-stu-id="aa3dd-103">Version (SOAP)</span></span>

<span data-ttu-id="aa3dd-104">**Version**要素は、サーバー製品バージョンの説明を表します。</span><span class="sxs-lookup"><span data-stu-id="aa3dd-104">The **Version** element represents a description of the server product version.</span></span> 
  
```XML
<Version/>
```

 <span data-ttu-id="aa3dd-105">**string**</span><span class="sxs-lookup"><span data-stu-id="aa3dd-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="aa3dd-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="aa3dd-106">Attributes and elements</span></span>

<span data-ttu-id="aa3dd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="aa3dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="aa3dd-108">属性</span><span class="sxs-lookup"><span data-stu-id="aa3dd-108">Attributes</span></span>

<span data-ttu-id="aa3dd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="aa3dd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="aa3dd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="aa3dd-110">Child elements</span></span>

<span data-ttu-id="aa3dd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="aa3dd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="aa3dd-112">親要素</span><span class="sxs-lookup"><span data-stu-id="aa3dd-112">Parent elements</span></span>

|<span data-ttu-id="aa3dd-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="aa3dd-113">**Element**</span></span>|<span data-ttu-id="aa3dd-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="aa3dd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="aa3dd-115">ServerVersionInfo (SOAP)</span><span class="sxs-lookup"><span data-stu-id="aa3dd-115">ServerVersionInfo (SOAP)</span></span>](serverversioninfo-soap.md) <br/> |<span data-ttu-id="aa3dd-116">要求を処理したサーバーのバージョンが保存されています。</span><span class="sxs-lookup"><span data-stu-id="aa3dd-116">Contains the version of the server that processed the request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="aa3dd-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="aa3dd-117">Text value</span></span>

<span data-ttu-id="aa3dd-118">**Version**要素の値は、サーバー製品のバージョンの説明です。</span><span class="sxs-lookup"><span data-stu-id="aa3dd-118">The value of the **Version** element is a description of the server product version.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="aa3dd-119">注釈</span><span class="sxs-lookup"><span data-stu-id="aa3dd-119">Remarks</span></span>

<span data-ttu-id="aa3dd-120">**Version**要素は、応答の SOAP ヘッダーに含まれています。</span><span class="sxs-lookup"><span data-stu-id="aa3dd-120">The **Version** element is contained in the SOAP header of a response.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="aa3dd-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="aa3dd-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="aa3dd-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="aa3dd-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="aa3dd-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="aa3dd-123">Schema Name</span></span>  <br/> |<span data-ttu-id="aa3dd-124">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="aa3dd-124">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="aa3dd-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="aa3dd-125">Validation File</span></span>  <br/> |<span data-ttu-id="aa3dd-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="aa3dd-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="aa3dd-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="aa3dd-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="aa3dd-128">正しい</span><span class="sxs-lookup"><span data-stu-id="aa3dd-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="aa3dd-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="aa3dd-129">See also</span></span>



[<span data-ttu-id="aa3dd-130">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="aa3dd-130">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="aa3dd-131">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="aa3dd-131">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)
  
[<span data-ttu-id="aa3dd-132">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="aa3dd-132">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

