---
title: アドレス (ArrayOfAddressEntitiesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0c1f3fd3-1b78-46ee-8dd4-b2aff51e767e
description: アドレス要素は、AddressEntity 要素の配列を指定します。
ms.openlocfilehash: b6fbcc54a016e698bccbe075fd340c0c784f121a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759298"
---
# <a name="addresses-arrayofaddressentitiestype"></a><span data-ttu-id="cf240-103">アドレス (ArrayOfAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="cf240-103">Addresses (ArrayOfAddressEntitiesType)</span></span>

<span data-ttu-id="cf240-104">**アドレス**要素は、 **AddressEntity**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="cf240-104">The **Addresses** element specifies an array of **AddressEntity** elements.</span></span> 
  
```XML
<Addresses>
   <AddressEntity/>
</Addresses>
```

 <span data-ttu-id="cf240-105">**ArrayOfAddressEntitiesType**</span><span class="sxs-lookup"><span data-stu-id="cf240-105">**ArrayOfAddressEntitiesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf240-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cf240-106">Attributes and elements</span></span>

<span data-ttu-id="cf240-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cf240-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf240-108">属性</span><span class="sxs-lookup"><span data-stu-id="cf240-108">Attributes</span></span>

<span data-ttu-id="cf240-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cf240-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf240-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cf240-110">Child elements</span></span>

|<span data-ttu-id="cf240-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="cf240-111">**Element**</span></span>|<span data-ttu-id="cf240-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="cf240-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf240-113">AddressEntity</span><span class="sxs-lookup"><span data-stu-id="cf240-113">AddressEntity</span></span>](addressentity.md) <br/> |<span data-ttu-id="cf240-114">アドレスの 1 つのエンティティを指定します。</span><span class="sxs-lookup"><span data-stu-id="cf240-114">Specifies a single address entity.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cf240-115">親要素</span><span class="sxs-lookup"><span data-stu-id="cf240-115">Parent elements</span></span>

|<span data-ttu-id="cf240-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="cf240-116">**Element**</span></span>|<span data-ttu-id="cf240-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="cf240-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf240-118">EntityExtractionResult</span><span class="sxs-lookup"><span data-stu-id="cf240-118">EntityExtractionResult</span></span>](entityextractionresult.md) <br/> |<span data-ttu-id="cf240-119">項目の**EntityExtractionResult**プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="cf240-119">Specifies the **EntityExtractionResult** property of an item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cf240-120">備考</span><span class="sxs-lookup"><span data-stu-id="cf240-120">Remarks</span></span>

<span data-ttu-id="cf240-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="cf240-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cf240-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cf240-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf240-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="cf240-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf240-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="cf240-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cf240-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cf240-125">Schema Name</span></span>  <br/> |<span data-ttu-id="cf240-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="cf240-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="cf240-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cf240-127">Validation File</span></span>  <br/> |<span data-ttu-id="cf240-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="cf240-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="cf240-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cf240-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="cf240-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="cf240-130">See also</span></span>

- [<span data-ttu-id="cf240-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="cf240-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

