---
title: 住所 (ArrayOfAddressEntitiesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0c1f3fd3-1b78-46ee-8dd4-b2aff51e767e
description: Addresses 要素は、AddressEntity 要素の配列を指定します。
ms.openlocfilehash: 48cf8c0fda6a8ef894ef8d3a4c154f7255b218bf
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463630"
---
# <a name="addresses-arrayofaddressentitiestype"></a><span data-ttu-id="b74ce-103">住所 (ArrayOfAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="b74ce-103">Addresses (ArrayOfAddressEntitiesType)</span></span>

<span data-ttu-id="b74ce-104">**Addresses**要素は、 **addressentity**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="b74ce-104">The **Addresses** element specifies an array of **AddressEntity** elements.</span></span> 
  
```XML
<Addresses>
   <AddressEntity/>
</Addresses>
```

 <span data-ttu-id="b74ce-105">**ArrayOfAddressEntitiesType**</span><span class="sxs-lookup"><span data-stu-id="b74ce-105">**ArrayOfAddressEntitiesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b74ce-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b74ce-106">Attributes and elements</span></span>

<span data-ttu-id="b74ce-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b74ce-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b74ce-108">属性</span><span class="sxs-lookup"><span data-stu-id="b74ce-108">Attributes</span></span>

<span data-ttu-id="b74ce-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b74ce-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b74ce-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b74ce-110">Child elements</span></span>

|<span data-ttu-id="b74ce-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="b74ce-111">**Element**</span></span>|<span data-ttu-id="b74ce-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="b74ce-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b74ce-113">AddressEntity</span><span class="sxs-lookup"><span data-stu-id="b74ce-113">AddressEntity</span></span>](addressentity.md) <br/> |<span data-ttu-id="b74ce-114">単一のアドレスエンティティを指定します。</span><span class="sxs-lookup"><span data-stu-id="b74ce-114">Specifies a single address entity.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b74ce-115">親要素</span><span class="sxs-lookup"><span data-stu-id="b74ce-115">Parent elements</span></span>

|<span data-ttu-id="b74ce-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="b74ce-116">**Element**</span></span>|<span data-ttu-id="b74ce-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="b74ce-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b74ce-118">EntityExtractionResult</span><span class="sxs-lookup"><span data-stu-id="b74ce-118">EntityExtractionResult</span></span>](entityextractionresult.md) <br/> |<span data-ttu-id="b74ce-119">アイテムの**Entityextractionresult**プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="b74ce-119">Specifies the **EntityExtractionResult** property of an item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b74ce-120">注釈</span><span class="sxs-lookup"><span data-stu-id="b74ce-120">Remarks</span></span>

<span data-ttu-id="b74ce-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b74ce-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b74ce-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b74ce-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b74ce-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b74ce-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b74ce-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="b74ce-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b74ce-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b74ce-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b74ce-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="b74ce-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="b74ce-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b74ce-127">Validation File</span></span>  <br/> |<span data-ttu-id="b74ce-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b74ce-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b74ce-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b74ce-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b74ce-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="b74ce-130">See also</span></span>

- [<span data-ttu-id="b74ce-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b74ce-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

