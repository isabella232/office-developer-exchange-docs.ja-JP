---
title: EnhancedLocation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4fdfb74f-f33c-46ae-a7c7-451a5b0c6a59
description: EnhancedLocation 要素は、場所の名前、住所、メモなどの位置情報を指定します。
ms.openlocfilehash: 90397cfc622fed40c561d30c13d6617eb979a68a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760303"
---
# <a name="enhancedlocation"></a><span data-ttu-id="4e4c4-103">EnhancedLocation</span><span class="sxs-lookup"><span data-stu-id="4e4c4-103">EnhancedLocation</span></span>

<span data-ttu-id="4e4c4-104">**EnhancedLocation**要素は、場所の名前、住所、メモなどの位置情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e4c4-104">The **EnhancedLocation** element specifies location information such as the name, address, and optional notes about a location.</span></span> 
  
```XML
<EnhancedLocation>
    <DisplayName/>
    <Annotation/>
    <PostalAddress/>
</EnhancedLocation>
```

 <span data-ttu-id="4e4c4-105">**EnhancedLocationType**</span><span class="sxs-lookup"><span data-stu-id="4e4c4-105">**EnhancedLocationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4e4c4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4e4c4-106">Attributes and elements</span></span>

<span data-ttu-id="4e4c4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4e4c4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4e4c4-108">属性</span><span class="sxs-lookup"><span data-stu-id="4e4c4-108">Attributes</span></span>

<span data-ttu-id="4e4c4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4e4c4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4e4c4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4e4c4-110">Child elements</span></span>

|<span data-ttu-id="4e4c4-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="4e4c4-111">**Element**</span></span>|<span data-ttu-id="4e4c4-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4e4c4-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e4c4-113">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="4e4c4-113">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="4e4c4-114">フォルダー、連絡先、配布リスト、ユーザーの代理人、場所、またはルールの表示名を定義します。</span><span class="sxs-lookup"><span data-stu-id="4e4c4-114">Defines the display name of a folder, contact, distribution list, delegate user, location, or rule.</span></span>  <br/> |
|[<span data-ttu-id="4e4c4-115">注釈</span><span class="sxs-lookup"><span data-stu-id="4e4c4-115">Annotation</span></span>](annotation.md) <br/> |<span data-ttu-id="4e4c4-116">ユーザーによって追加されたメモが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4e4c4-116">Contains optional notes added by a user.</span></span>  <br/> |
|[<span data-ttu-id="4e4c4-117">住所 (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="4e4c4-117">PostalAddress (PersonaPostalAddressType)</span></span>](postaladdress-personapostaladdresstype.md) <br/> |<span data-ttu-id="4e4c4-118">ペルソナの郵便の宛先を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e4c4-118">Specifies the postal address for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4e4c4-119">親要素</span><span class="sxs-lookup"><span data-stu-id="4e4c4-119">Parent elements</span></span>

|<span data-ttu-id="4e4c4-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="4e4c4-120">**Element**</span></span>|<span data-ttu-id="4e4c4-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="4e4c4-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e4c4-122">カレンダー項目</span><span class="sxs-lookup"><span data-stu-id="4e4c4-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="4e4c4-123">Exchange 予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="4e4c4-123">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="4e4c4-124">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="4e4c4-124">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="4e4c4-125">Exchange ストア内の会議の取り消し通知を表します。</span><span class="sxs-lookup"><span data-stu-id="4e4c4-125">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="4e4c4-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="4e4c4-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="4e4c4-127">Exchange ストア内の会議の返信を表します。</span><span class="sxs-lookup"><span data-stu-id="4e4c4-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4e4c4-128">備考</span><span class="sxs-lookup"><span data-stu-id="4e4c4-128">Remarks</span></span>

<span data-ttu-id="4e4c4-129">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4e4c4-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4e4c4-130">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4e4c4-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4e4c4-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="4e4c4-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4e4c4-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="4e4c4-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4e4c4-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4e4c4-133">Schema Name</span></span>  <br/> |<span data-ttu-id="4e4c4-134">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="4e4c4-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="4e4c4-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4e4c4-135">Validation File</span></span>  <br/> |<span data-ttu-id="4e4c4-136">types.xsd</span><span class="sxs-lookup"><span data-stu-id="4e4c4-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4e4c4-137">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4e4c4-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4e4c4-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="4e4c4-138">See also</span></span>



- [<span data-ttu-id="4e4c4-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4e4c4-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

