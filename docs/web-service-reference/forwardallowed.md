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
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760586"
---
# <a name="forwardallowed"></a><span data-ttu-id="546bd-103">ForwardAllowed</span><span class="sxs-lookup"><span data-stu-id="546bd-103">ForwardAllowed</span></span>

<span data-ttu-id="546bd-104">**ForwardAllowed**要素は、電子メールの転送が有効になっているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="546bd-104">The **ForwardAllowed** element specifies whether forwarding emails is enabled.</span></span> 
  
```XML
<ForwardAllowed>true | false</ForwardAllowed>
```

 <span data-ttu-id="546bd-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="546bd-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="546bd-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="546bd-106">Attributes and elements</span></span>

<span data-ttu-id="546bd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="546bd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="546bd-108">属性</span><span class="sxs-lookup"><span data-stu-id="546bd-108">Attributes</span></span>

<span data-ttu-id="546bd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="546bd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="546bd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="546bd-110">Child elements</span></span>

<span data-ttu-id="546bd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="546bd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="546bd-112">親要素</span><span class="sxs-lookup"><span data-stu-id="546bd-112">Parent elements</span></span>

|<span data-ttu-id="546bd-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="546bd-113">**Element**</span></span>|<span data-ttu-id="546bd-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="546bd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="546bd-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="546bd-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="546bd-116">権限管理のライセンスについての情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="546bd-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="546bd-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="546bd-117">Text value</span></span>

<span data-ttu-id="546bd-118">の**場合は true** 、 **ForwardAllowed**要素のテキスト値は、e メールを転送を許可することを示します。</span><span class="sxs-lookup"><span data-stu-id="546bd-118">A text value of **true** for the **ForwardAllowed** element indicates that forwarding emails is allowed.</span></span> <span data-ttu-id="546bd-119">**False**の値は、転送が許可されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="546bd-119">A value of **false** indicates that forwarding is not allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="546bd-120">備考</span><span class="sxs-lookup"><span data-stu-id="546bd-120">Remarks</span></span>

<span data-ttu-id="546bd-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="546bd-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="546bd-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="546bd-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="546bd-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="546bd-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="546bd-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="546bd-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="546bd-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="546bd-125">Schema Name</span></span>  <br/> |<span data-ttu-id="546bd-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="546bd-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="546bd-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="546bd-127">Validation File</span></span>  <br/> |<span data-ttu-id="546bd-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="546bd-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="546bd-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="546bd-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="546bd-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="546bd-130">See also</span></span>



- [<span data-ttu-id="546bd-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="546bd-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

