---
title: EnhancedLocation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4fdfb74f-f33c-46ae-a7c7-451a5b0c6a59
description: EnhancedLocation 要素は、場所に関する名前、住所、オプションのメモなどの場所情報を指定します。
ms.openlocfilehash: 06ec800b763ef61af51da03ca8a340f6ac4d2a8e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462958"
---
# <a name="enhancedlocation"></a><span data-ttu-id="7c4a8-103">EnhancedLocation</span><span class="sxs-lookup"><span data-stu-id="7c4a8-103">EnhancedLocation</span></span>

<span data-ttu-id="7c4a8-104">**EnhancedLocation**要素は、場所に関する名前、住所、オプションのメモなどの場所情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="7c4a8-104">The **EnhancedLocation** element specifies location information such as the name, address, and optional notes about a location.</span></span> 
  
```XML
<EnhancedLocation>
    <DisplayName/>
    <Annotation/>
    <PostalAddress/>
</EnhancedLocation>
```

 <span data-ttu-id="7c4a8-105">**EnhancedLocationType**</span><span class="sxs-lookup"><span data-stu-id="7c4a8-105">**EnhancedLocationType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c4a8-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7c4a8-106">Attributes and elements</span></span>

<span data-ttu-id="7c4a8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7c4a8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c4a8-108">属性</span><span class="sxs-lookup"><span data-stu-id="7c4a8-108">Attributes</span></span>

<span data-ttu-id="7c4a8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7c4a8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c4a8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7c4a8-110">Child elements</span></span>

|<span data-ttu-id="7c4a8-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="7c4a8-111">**Element**</span></span>|<span data-ttu-id="7c4a8-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7c4a8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c4a8-113">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="7c4a8-113">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="7c4a8-114">フォルダー、連絡先、配布リスト、代理人のユーザー、場所、またはルールの表示名を定義します。</span><span class="sxs-lookup"><span data-stu-id="7c4a8-114">Defines the display name of a folder, contact, distribution list, delegate user, location, or rule.</span></span>  <br/> |
|[<span data-ttu-id="7c4a8-115">アノテーションフィーチャー</span><span class="sxs-lookup"><span data-stu-id="7c4a8-115">Annotation</span></span>](annotation.md) <br/> |<span data-ttu-id="7c4a8-116">ユーザーによって追加されたオプションのメモが保存されています。</span><span class="sxs-lookup"><span data-stu-id="7c4a8-116">Contains optional notes added by a user.</span></span>  <br/> |
|[<span data-ttu-id="7c4a8-117">"Postaladdress (PersonaPostalAddressType)</span><span class="sxs-lookup"><span data-stu-id="7c4a8-117">PostalAddress (PersonaPostalAddressType)</span></span>](postaladdress-personapostaladdresstype.md) <br/> |<span data-ttu-id="7c4a8-118">ペルソナの住所を指定します。</span><span class="sxs-lookup"><span data-stu-id="7c4a8-118">Specifies the postal address for a persona.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c4a8-119">親要素</span><span class="sxs-lookup"><span data-stu-id="7c4a8-119">Parent elements</span></span>

|<span data-ttu-id="7c4a8-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="7c4a8-120">**Element**</span></span>|<span data-ttu-id="7c4a8-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="7c4a8-121">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c4a8-122">CalendarItem</span><span class="sxs-lookup"><span data-stu-id="7c4a8-122">CalendarItem</span></span>](calendaritem.md) <br/> |<span data-ttu-id="7c4a8-123">Exchange の予定表アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="7c4a8-123">Represents an Exchange calendar item.</span></span>  <br/> |
|[<span data-ttu-id="7c4a8-124">MeetingCancellation</span><span class="sxs-lookup"><span data-stu-id="7c4a8-124">MeetingCancellation</span></span>](meetingcancellation.md) <br/> |<span data-ttu-id="7c4a8-125">Exchange ストア内の会議の取り消しを表します。</span><span class="sxs-lookup"><span data-stu-id="7c4a8-125">Represents a meeting cancellation in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7c4a8-126">MeetingResponse</span><span class="sxs-lookup"><span data-stu-id="7c4a8-126">MeetingResponse</span></span>](meetingresponse.md) <br/> |<span data-ttu-id="7c4a8-127">Exchange ストア内の会議の応答を表します。</span><span class="sxs-lookup"><span data-stu-id="7c4a8-127">Represents a meeting response in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7c4a8-128">注釈</span><span class="sxs-lookup"><span data-stu-id="7c4a8-128">Remarks</span></span>

<span data-ttu-id="7c4a8-129">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7c4a8-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7c4a8-130">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7c4a8-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c4a8-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7c4a8-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c4a8-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="7c4a8-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c4a8-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7c4a8-133">Schema Name</span></span>  <br/> |<span data-ttu-id="7c4a8-134">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="7c4a8-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="7c4a8-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7c4a8-135">Validation File</span></span>  <br/> |<span data-ttu-id="7c4a8-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7c4a8-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c4a8-137">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7c4a8-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="7c4a8-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="7c4a8-138">See also</span></span>



- [<span data-ttu-id="7c4a8-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7c4a8-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

