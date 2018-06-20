---
title: EntityExtractionResult
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 643b99ab-ff90-4411-864c-1077623028d6
description: EntityExtractionResult 要素は、項目の EntityExtractionResult プロパティを指定します。
ms.openlocfilehash: ef99629beb95f1e1123569fa99e3f495c1b56e95
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760313"
---
# <a name="entityextractionresult"></a><span data-ttu-id="d0b4f-103">EntityExtractionResult</span><span class="sxs-lookup"><span data-stu-id="d0b4f-103">EntityExtractionResult</span></span>

<span data-ttu-id="d0b4f-104">**EntityExtractionResult**要素は、項目の**EntityExtractionResult**プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="d0b4f-104">The **EntityExtractionResult** element specifies the **EntityExtractionResult** property of an item.</span></span> 
  
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

 <span data-ttu-id="d0b4f-105">**EntityExtractionResultType**</span><span class="sxs-lookup"><span data-stu-id="d0b4f-105">**EntityExtractionResultType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d0b4f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d0b4f-106">Attributes and elements</span></span>

<span data-ttu-id="d0b4f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d0b4f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d0b4f-108">属性</span><span class="sxs-lookup"><span data-stu-id="d0b4f-108">Attributes</span></span>

<span data-ttu-id="d0b4f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d0b4f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d0b4f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d0b4f-110">Child elements</span></span>

|<span data-ttu-id="d0b4f-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d0b4f-111">**Element**</span></span>|<span data-ttu-id="d0b4f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d0b4f-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0b4f-113">アドレス (ArrayOfAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="d0b4f-113">Addresses (ArrayOfAddressEntitiesType)</span></span>](addresses-arrayofaddressentitiestype.md) <br/> |<span data-ttu-id="d0b4f-114">**AddressEntity**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="d0b4f-114">Specifies an array of **AddressEntity** elements.</span></span>  <br/> |
|[<span data-ttu-id="d0b4f-115">MeetingSuggestions</span><span class="sxs-lookup"><span data-stu-id="d0b4f-115">MeetingSuggestions</span></span>](meetingsuggestions.md) <br/> |<span data-ttu-id="d0b4f-116">**MeetingSuggestion**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="d0b4f-116">Specifies an array of **MeetingSuggestion** elements.</span></span>  <br/> |
|[<span data-ttu-id="d0b4f-117">TaskSuggestions</span><span class="sxs-lookup"><span data-stu-id="d0b4f-117">TaskSuggestions</span></span>](tasksuggestions.md) <br/> |<span data-ttu-id="d0b4f-118">**TaskSuggestion**要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="d0b4f-118">Specifies an array of **TaskSuggestion** elements.</span></span>  <br/> |
|[<span data-ttu-id="d0b4f-119">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="d0b4f-119">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span></span>](emailaddresses-arrayofemailaddressentitiestype.md) <br/> |<span data-ttu-id="d0b4f-120">E メール アドレスのエンティティの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="d0b4f-120">Specifies an array of email address entities.</span></span>  <br/> |
|[<span data-ttu-id="d0b4f-121">連絡先 (ArrayOfContactsType)</span><span class="sxs-lookup"><span data-stu-id="d0b4f-121">Contacts (ArrayOfContactsType)</span></span>](contacts-arrayofcontactstype.md) <br/> |<span data-ttu-id="d0b4f-122">メンバーの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="d0b4f-122">Specifies an array of contacts.</span></span>  <br/> |
|[<span data-ttu-id="d0b4f-123">Url (ArrayOfUrlEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="d0b4f-123">Urls (ArrayOfUrlEntitiesType)</span></span>](urls-arrayofurlentitiestype.md) <br/> |<span data-ttu-id="d0b4f-124">Url の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="d0b4f-124">Specifies an array of URLs.</span></span>  <br/> |
|[<span data-ttu-id="d0b4f-125">PhoneNumbers (ArrayOfPhoneEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="d0b4f-125">PhoneNumbers (ArrayOfPhoneEntitiesType)</span></span>](phonenumbers-arrayofphoneentitiestype.md) <br/> |<span data-ttu-id="d0b4f-126">電話番号の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="d0b4f-126">Specifies an array of phone numbers.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d0b4f-127">親要素</span><span class="sxs-lookup"><span data-stu-id="d0b4f-127">Parent elements</span></span>

|<span data-ttu-id="d0b4f-128">**要素**</span><span class="sxs-lookup"><span data-stu-id="d0b4f-128">**Element**</span></span>|<span data-ttu-id="d0b4f-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="d0b4f-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d0b4f-130">Item</span><span class="sxs-lookup"><span data-stu-id="d0b4f-130">Item</span></span>](item.md) <br/> |<span data-ttu-id="d0b4f-131">Exchange ストア内の一般的な項目を表します。</span><span class="sxs-lookup"><span data-stu-id="d0b4f-131">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d0b4f-132">備考</span><span class="sxs-lookup"><span data-stu-id="d0b4f-132">Remarks</span></span>

<span data-ttu-id="d0b4f-133">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d0b4f-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d0b4f-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d0b4f-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d0b4f-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="d0b4f-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d0b4f-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="d0b4f-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d0b4f-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d0b4f-137">Schema Name</span></span>  <br/> |<span data-ttu-id="d0b4f-138">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="d0b4f-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="d0b4f-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d0b4f-139">Validation File</span></span>  <br/> |<span data-ttu-id="d0b4f-140">types.xsd</span><span class="sxs-lookup"><span data-stu-id="d0b4f-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d0b4f-141">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d0b4f-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d0b4f-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="d0b4f-142">See also</span></span>



- [<span data-ttu-id="d0b4f-143">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d0b4f-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

