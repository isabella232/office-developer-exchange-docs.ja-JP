---
title: ArrayOfUserResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 3e5cf65c-8d0b-4fd9-8207-56c07f914acd
description: ArrayOfUserResponse 要素には、UserResponse (SOAP) の要素の配列が含まれています。
ms.openlocfilehash: 7fab572c5e783a09c37e07492ddcd55d5ba34c84
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759440"
---
# <a name="arrayofuserresponse-soap"></a><span data-ttu-id="fef8b-103">ArrayOfUserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fef8b-103">ArrayOfUserResponse (SOAP)</span></span>

<span data-ttu-id="fef8b-104">**ArrayOfUserResponse**要素には、 [UserResponse (SOAP)](userresponse-soap.md)の要素の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fef8b-104">The **ArrayOfUserResponse** element contains an array of [UserResponse (SOAP)](userresponse-soap.md) elements.</span></span> 
  
```XML
<ArrayOfUserResponse>
   <UserResponse/>
</ArrayOfUserResponse>
```

 <span data-ttu-id="fef8b-105">**ArrayOfUserResponse**</span><span class="sxs-lookup"><span data-stu-id="fef8b-105">**ArrayOfUserResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fef8b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fef8b-106">Attributes and elements</span></span>

<span data-ttu-id="fef8b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fef8b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fef8b-108">属性</span><span class="sxs-lookup"><span data-stu-id="fef8b-108">Attributes</span></span>

<span data-ttu-id="fef8b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fef8b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fef8b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fef8b-110">Child elements</span></span>

|<span data-ttu-id="fef8b-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="fef8b-111">**Element**</span></span>|<span data-ttu-id="fef8b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="fef8b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fef8b-113">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fef8b-113">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="fef8b-114">指定したユーザーの要求された設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="fef8b-114">Contains the requested settings for the specified user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fef8b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="fef8b-115">Parent elements</span></span>

<span data-ttu-id="fef8b-116">なし。</span><span class="sxs-lookup"><span data-stu-id="fef8b-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="fef8b-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fef8b-117">Text value</span></span>

<span data-ttu-id="fef8b-118">なし。</span><span class="sxs-lookup"><span data-stu-id="fef8b-118">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fef8b-119">要素情報</span><span class="sxs-lookup"><span data-stu-id="fef8b-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fef8b-120">名前空間</span><span class="sxs-lookup"><span data-stu-id="fef8b-120">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="fef8b-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fef8b-121">Schema Name</span></span>  <br/> |<span data-ttu-id="fef8b-122">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="fef8b-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="fef8b-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fef8b-123">Validation File</span></span>  <br/> |<span data-ttu-id="fef8b-124">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fef8b-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fef8b-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="fef8b-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="fef8b-126">True</span><span class="sxs-lookup"><span data-stu-id="fef8b-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fef8b-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="fef8b-127">See also</span></span>

- [<span data-ttu-id="fef8b-128">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="fef8b-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

