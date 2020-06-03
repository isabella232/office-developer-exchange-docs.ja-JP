---
title: AddressEntity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ead22eab-f1e7-48b4-a165-db0e49fe86a8
description: AddressEntity 要素は、1つのアドレスエンティティを指定します。
ms.openlocfilehash: c597557fe02a9c0ff7ed3c9862e1662cfbae596a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466907"
---
# <a name="addressentity"></a><span data-ttu-id="134ec-103">AddressEntity</span><span class="sxs-lookup"><span data-stu-id="134ec-103">AddressEntity</span></span>

<span data-ttu-id="134ec-104">**Addressentity**要素は、1つのアドレスエンティティを指定します。</span><span class="sxs-lookup"><span data-stu-id="134ec-104">The **AddressEntity** element specifies a single address entity.</span></span> 
  
```XML
<AddressEntity>
    <Address></Address>
    <Position></Position>
</AddressEntity>
```

 <span data-ttu-id="134ec-105">**AddressEntityType**</span><span class="sxs-lookup"><span data-stu-id="134ec-105">**AddressEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="134ec-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="134ec-106">Attributes and elements</span></span>

<span data-ttu-id="134ec-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="134ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="134ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="134ec-108">Attributes</span></span>

<span data-ttu-id="134ec-109">なし。</span><span class="sxs-lookup"><span data-stu-id="134ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="134ec-110">子要素</span><span class="sxs-lookup"><span data-stu-id="134ec-110">Child elements</span></span>

|<span data-ttu-id="134ec-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="134ec-111">**Element**</span></span>|<span data-ttu-id="134ec-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="134ec-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="134ec-113">Address (string)</span><span class="sxs-lookup"><span data-stu-id="134ec-113">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="134ec-114">住所を指定します。</span><span class="sxs-lookup"><span data-stu-id="134ec-114">Specifies an address.</span></span>  <br/> |
|[<span data-ttu-id="134ec-115">Position</span><span class="sxs-lookup"><span data-stu-id="134ec-115">Position</span></span>](position.md) <br/> |<span data-ttu-id="134ec-116">電子メールメッセージ内の位置を指定します。</span><span class="sxs-lookup"><span data-stu-id="134ec-116">Specifies the position in an email message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="134ec-117">親要素</span><span class="sxs-lookup"><span data-stu-id="134ec-117">Parent elements</span></span>

|<span data-ttu-id="134ec-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="134ec-118">**Element**</span></span>|<span data-ttu-id="134ec-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="134ec-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="134ec-120">住所 (ArrayOfAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="134ec-120">Addresses (ArrayOfAddressEntitiesType)</span></span>](addresses-arrayofaddressentitiestype.md) <br/> |<span data-ttu-id="134ec-121">**Addressentity**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="134ec-121">Specifies an array of **AddressEntity** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="134ec-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="134ec-122">Text value</span></span>

<span data-ttu-id="134ec-123">なし。</span><span class="sxs-lookup"><span data-stu-id="134ec-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="134ec-124">注釈</span><span class="sxs-lookup"><span data-stu-id="134ec-124">Remarks</span></span>

<span data-ttu-id="134ec-125">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="134ec-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="134ec-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="134ec-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="134ec-127">要素の情報</span><span class="sxs-lookup"><span data-stu-id="134ec-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="134ec-128">Namespace</span><span class="sxs-lookup"><span data-stu-id="134ec-128">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="134ec-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="134ec-129">Schema Name</span></span>  <br/> |<span data-ttu-id="134ec-130">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="134ec-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="134ec-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="134ec-131">Validation File</span></span>  <br/> |<span data-ttu-id="134ec-132">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="134ec-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="134ec-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="134ec-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="134ec-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="134ec-134">See also</span></span>

- [<span data-ttu-id="134ec-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="134ec-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

