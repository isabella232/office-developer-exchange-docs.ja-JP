---
title: EntityExtractionResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 643b99ab-ff90-4411-864c-1077623028d6
description: EntityExtractionResult 要素は、アイテムの EntityExtractionResult プロパティを指定します。
ms.openlocfilehash: f2f069717a5862adff3349090c35f95499d135f8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456956"
---
# <a name="entityextractionresult"></a><span data-ttu-id="817d2-103">EntityExtractionResult</span><span class="sxs-lookup"><span data-stu-id="817d2-103">EntityExtractionResult</span></span>

<span data-ttu-id="817d2-104">**Entityextractionresult**要素は、アイテムの**entityextractionresult**プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="817d2-104">The **EntityExtractionResult** element specifies the **EntityExtractionResult** property of an item.</span></span> 
  
```XML
<EntityExtractionResult>
    <Addresses/>
    <MeetingSuggestions/>
    <TaskSuggestions/>
    <EmailAddresses/>
    <Contacts/>
    <Urls/>
    <PhoneNumbers/>
</EntityExtractionResult>
```

 <span data-ttu-id="817d2-105">**EntityExtractionResultType**</span><span class="sxs-lookup"><span data-stu-id="817d2-105">**EntityExtractionResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="817d2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="817d2-106">Attributes and elements</span></span>

<span data-ttu-id="817d2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="817d2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="817d2-108">属性</span><span class="sxs-lookup"><span data-stu-id="817d2-108">Attributes</span></span>

<span data-ttu-id="817d2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="817d2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="817d2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="817d2-110">Child elements</span></span>

|<span data-ttu-id="817d2-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="817d2-111">**Element**</span></span>|<span data-ttu-id="817d2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="817d2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="817d2-113">住所 (ArrayOfAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="817d2-113">Addresses (ArrayOfAddressEntitiesType)</span></span>](addresses-arrayofaddressentitiestype.md) <br/> |<span data-ttu-id="817d2-114">**Addressentity**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="817d2-114">Specifies an array of **AddressEntity** elements.</span></span>  <br/> |
|[<span data-ttu-id="817d2-115">MeetingSuggestions</span><span class="sxs-lookup"><span data-stu-id="817d2-115">MeetingSuggestions</span></span>](meetingsuggestions.md) <br/> |<span data-ttu-id="817d2-116">**会議提案**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="817d2-116">Specifies an array of **MeetingSuggestion** elements.</span></span>  <br/> |
|[<span data-ttu-id="817d2-117">TaskSuggestions</span><span class="sxs-lookup"><span data-stu-id="817d2-117">TaskSuggestions</span></span>](tasksuggestions.md) <br/> |<span data-ttu-id="817d2-118">**Tasksuggestion**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="817d2-118">Specifies an array of **TaskSuggestion** elements.</span></span>  <br/> |
|[<span data-ttu-id="817d2-119">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="817d2-119">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span></span>](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |<span data-ttu-id="817d2-120">電子メールアドレスエンティティの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="817d2-120">Specifies an array of email address entities.</span></span>  <br/> |
|[<span data-ttu-id="817d2-121">連絡先 (ArrayOfContactsType)</span><span class="sxs-lookup"><span data-stu-id="817d2-121">Contacts (ArrayOfContactsType)</span></span>](contacts-arrayofcontactstype.md) <br/> |<span data-ttu-id="817d2-122">連絡先の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="817d2-122">Specifies an array of contacts.</span></span>  <br/> |
|[<span data-ttu-id="817d2-123">Url (ArrayOfUrlEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="817d2-123">Urls (ArrayOfUrlEntitiesType)</span></span>](urls-arrayofurlentitiestype.md) <br/> |<span data-ttu-id="817d2-124">Url の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="817d2-124">Specifies an array of URLs.</span></span>  <br/> |
|[<span data-ttu-id="817d2-125">PhoneNumbers (ArrayOfPhoneEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="817d2-125">PhoneNumbers (ArrayOfPhoneEntitiesType)</span></span>](phonenumbers-arrayofphoneentitiestype.md) <br/> |<span data-ttu-id="817d2-126">電話番号の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="817d2-126">Specifies an array of phone numbers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="817d2-127">親要素</span><span class="sxs-lookup"><span data-stu-id="817d2-127">Parent elements</span></span>

|<span data-ttu-id="817d2-128">**要素**</span><span class="sxs-lookup"><span data-stu-id="817d2-128">**Element**</span></span>|<span data-ttu-id="817d2-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="817d2-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="817d2-130">Item</span><span class="sxs-lookup"><span data-stu-id="817d2-130">Item</span></span>](item.md) <br/> |<span data-ttu-id="817d2-131">Exchange ストア内の汎用アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="817d2-131">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="817d2-132">注釈</span><span class="sxs-lookup"><span data-stu-id="817d2-132">Remarks</span></span>

<span data-ttu-id="817d2-133">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="817d2-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="817d2-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="817d2-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="817d2-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="817d2-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="817d2-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="817d2-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="817d2-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="817d2-137">Schema Name</span></span>  <br/> |<span data-ttu-id="817d2-138">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="817d2-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="817d2-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="817d2-139">Validation File</span></span>  <br/> |<span data-ttu-id="817d2-140">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="817d2-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="817d2-141">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="817d2-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="817d2-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="817d2-142">See also</span></span>



- [<span data-ttu-id="817d2-143">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="817d2-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

