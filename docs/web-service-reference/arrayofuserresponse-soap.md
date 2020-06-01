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
description: ArrayOfUserResponse 要素には、UserResponse (SOAP) 要素の配列が含まれています。
ms.openlocfilehash: fb14b6cd714a0561e9c8e17bd1779d955ba16dfc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466011"
---
# <a name="arrayofuserresponse-soap"></a><span data-ttu-id="bc1d0-103">ArrayOfUserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bc1d0-103">ArrayOfUserResponse (SOAP)</span></span>

<span data-ttu-id="bc1d0-104">**Arrayofuserresponse**要素には、 [USERRESPONSE (SOAP)](userresponse-soap.md)要素の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bc1d0-104">The **ArrayOfUserResponse** element contains an array of [UserResponse (SOAP)](userresponse-soap.md) elements.</span></span> 
  
```XML
<ArrayOfUserResponse>
   <UserResponse/>
</ArrayOfUserResponse>
```

 <span data-ttu-id="bc1d0-105">**ArrayOfUserResponse**</span><span class="sxs-lookup"><span data-stu-id="bc1d0-105">**ArrayOfUserResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="bc1d0-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="bc1d0-106">Attributes and elements</span></span>

<span data-ttu-id="bc1d0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bc1d0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bc1d0-108">属性</span><span class="sxs-lookup"><span data-stu-id="bc1d0-108">Attributes</span></span>

<span data-ttu-id="bc1d0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="bc1d0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="bc1d0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="bc1d0-110">Child elements</span></span>

|<span data-ttu-id="bc1d0-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="bc1d0-111">**Element**</span></span>|<span data-ttu-id="bc1d0-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="bc1d0-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bc1d0-113">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bc1d0-113">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="bc1d0-114">指定したユーザーの要求された設定を含みます。</span><span class="sxs-lookup"><span data-stu-id="bc1d0-114">Contains the requested settings for the specified user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bc1d0-115">親要素</span><span class="sxs-lookup"><span data-stu-id="bc1d0-115">Parent elements</span></span>

<span data-ttu-id="bc1d0-116">なし。</span><span class="sxs-lookup"><span data-stu-id="bc1d0-116">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="bc1d0-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bc1d0-117">Text value</span></span>

<span data-ttu-id="bc1d0-118">なし。</span><span class="sxs-lookup"><span data-stu-id="bc1d0-118">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bc1d0-119">要素の情報</span><span class="sxs-lookup"><span data-stu-id="bc1d0-119">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bc1d0-120">Namespace</span><span class="sxs-lookup"><span data-stu-id="bc1d0-120">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="bc1d0-121">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bc1d0-121">Schema Name</span></span>  <br/> |<span data-ttu-id="bc1d0-122">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="bc1d0-122">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="bc1d0-123">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bc1d0-123">Validation File</span></span>  <br/> |<span data-ttu-id="bc1d0-124">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="bc1d0-124">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bc1d0-125">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bc1d0-125">Can be Empty</span></span>  <br/> |<span data-ttu-id="bc1d0-126">正しい</span><span class="sxs-lookup"><span data-stu-id="bc1d0-126">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bc1d0-127">関連項目</span><span class="sxs-lookup"><span data-stu-id="bc1d0-127">See also</span></span>

- [<span data-ttu-id="bc1d0-128">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="bc1d0-128">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

