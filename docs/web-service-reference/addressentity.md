---
title: AddressEntity
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ead22eab-f1e7-48b4-a165-db0e49fe86a8
description: AddressEntity 要素は、1 つのアドレス エンティティを指定します。
ms.openlocfilehash: 6a46a64c9824efdd8df6a08fe1a159e7e42b3731
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759308"
---
# <a name="addressentity"></a><span data-ttu-id="3a3e7-103">AddressEntity</span><span class="sxs-lookup"><span data-stu-id="3a3e7-103">AddressEntity</span></span>

<span data-ttu-id="3a3e7-104">**AddressEntity**要素は、1 つのアドレス エンティティを指定します。</span><span class="sxs-lookup"><span data-stu-id="3a3e7-104">The **AddressEntity** element specifies a single address entity.</span></span> 
  
```XML
<AddressEntity>
    <Address></Address>
    <Position></Position>
</AddressEntity>
```

 <span data-ttu-id="3a3e7-105">**AddressEntityType**</span><span class="sxs-lookup"><span data-stu-id="3a3e7-105">**AddressEntityType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3a3e7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3a3e7-106">Attributes and elements</span></span>

<span data-ttu-id="3a3e7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3a3e7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3a3e7-108">属性</span><span class="sxs-lookup"><span data-stu-id="3a3e7-108">Attributes</span></span>

<span data-ttu-id="3a3e7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3a3e7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3a3e7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3a3e7-110">Child elements</span></span>

|<span data-ttu-id="3a3e7-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="3a3e7-111">**Element**</span></span>|<span data-ttu-id="3a3e7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3a3e7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a3e7-113">アドレス (文字列)</span><span class="sxs-lookup"><span data-stu-id="3a3e7-113">Address (string)</span></span>](address-string.md) <br/> |<span data-ttu-id="3a3e7-114">アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="3a3e7-114">Specifies an address.</span></span>  <br/> |
|[<span data-ttu-id="3a3e7-115">Position</span><span class="sxs-lookup"><span data-stu-id="3a3e7-115">Position</span></span>](position.md) <br/> |<span data-ttu-id="3a3e7-116">電子メール メッセージ内の位置を指定します。</span><span class="sxs-lookup"><span data-stu-id="3a3e7-116">Specifies the position in an email message.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3a3e7-117">親要素</span><span class="sxs-lookup"><span data-stu-id="3a3e7-117">Parent elements</span></span>

|<span data-ttu-id="3a3e7-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="3a3e7-118">**Element**</span></span>|<span data-ttu-id="3a3e7-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="3a3e7-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3a3e7-120">アドレス (ArrayOfAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="3a3e7-120">Addresses (ArrayOfAddressEntitiesType)</span></span>](addresses-arrayofaddressentitiestype.md) <br/> |<span data-ttu-id="3a3e7-121">**AddressEntity**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="3a3e7-121">Specifies an array of **AddressEntity** elements.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3a3e7-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3a3e7-122">Text value</span></span>

<span data-ttu-id="3a3e7-123">なし。</span><span class="sxs-lookup"><span data-stu-id="3a3e7-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3a3e7-124">備考</span><span class="sxs-lookup"><span data-stu-id="3a3e7-124">Remarks</span></span>

<span data-ttu-id="3a3e7-125">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3a3e7-125">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3a3e7-126">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3a3e7-126">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3a3e7-127">要素情報</span><span class="sxs-lookup"><span data-stu-id="3a3e7-127">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3a3e7-128">名前空間</span><span class="sxs-lookup"><span data-stu-id="3a3e7-128">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3a3e7-129">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3a3e7-129">Schema Name</span></span>  <br/> |<span data-ttu-id="3a3e7-130">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="3a3e7-130">Type schema</span></span>  <br/> |
|<span data-ttu-id="3a3e7-131">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3a3e7-131">Validation File</span></span>  <br/> |<span data-ttu-id="3a3e7-132">types.xsd</span><span class="sxs-lookup"><span data-stu-id="3a3e7-132">types.xsd</span></span>  <br/> |
|<span data-ttu-id="3a3e7-133">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3a3e7-133">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3a3e7-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="3a3e7-134">See also</span></span>

- [<span data-ttu-id="3a3e7-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3a3e7-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

