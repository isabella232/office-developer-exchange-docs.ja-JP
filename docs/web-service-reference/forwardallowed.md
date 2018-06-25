---
title: ForwardAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bc32e0f4-61e9-4c9f-9a03-90a07eb51c53
description: ForwardAllowed 要素は、電子メールの転送が有効になっているかどうかを指定します。
ms.openlocfilehash: 4baa170a531cc9021102ff2255afc113f40e2348
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760586"
---
# <a name="forwardallowed"></a><span data-ttu-id="2ff9c-103">ForwardAllowed</span><span class="sxs-lookup"><span data-stu-id="2ff9c-103">ForwardAllowed</span></span>

<span data-ttu-id="2ff9c-104">**ForwardAllowed**要素は、電子メールの転送が有効になっているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="2ff9c-104">The **ForwardAllowed** element specifies whether forwarding emails is enabled.</span></span> 
  
```XML
<ForwardAllowed>true | false</ForwardAllowed>
```

 <span data-ttu-id="2ff9c-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="2ff9c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2ff9c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2ff9c-106">Attributes and elements</span></span>

<span data-ttu-id="2ff9c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2ff9c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2ff9c-108">属性</span><span class="sxs-lookup"><span data-stu-id="2ff9c-108">Attributes</span></span>

<span data-ttu-id="2ff9c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2ff9c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2ff9c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2ff9c-110">Child elements</span></span>

<span data-ttu-id="2ff9c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2ff9c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2ff9c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2ff9c-112">Parent elements</span></span>

|<span data-ttu-id="2ff9c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="2ff9c-113">**Element**</span></span>|<span data-ttu-id="2ff9c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="2ff9c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2ff9c-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="2ff9c-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="2ff9c-116">権限管理のライセンスについての情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="2ff9c-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2ff9c-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2ff9c-117">Text value</span></span>

<span data-ttu-id="2ff9c-118">の**場合は true** 、 **ForwardAllowed**要素のテキスト値は、e メールを転送を許可することを示します。</span><span class="sxs-lookup"><span data-stu-id="2ff9c-118">A text value of **true** for the **ForwardAllowed** element indicates that forwarding emails is allowed.</span></span> <span data-ttu-id="2ff9c-119">**False**の値は、転送が許可されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="2ff9c-119">A value of **false** indicates that forwarding is not allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2ff9c-120">備考</span><span class="sxs-lookup"><span data-stu-id="2ff9c-120">Remarks</span></span>

<span data-ttu-id="2ff9c-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2ff9c-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2ff9c-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2ff9c-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2ff9c-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="2ff9c-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2ff9c-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="2ff9c-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2ff9c-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2ff9c-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2ff9c-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="2ff9c-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="2ff9c-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2ff9c-127">Validation File</span></span>  <br/> |<span data-ttu-id="2ff9c-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="2ff9c-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2ff9c-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2ff9c-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2ff9c-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="2ff9c-130">See also</span></span>



- [<span data-ttu-id="2ff9c-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2ff9c-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

