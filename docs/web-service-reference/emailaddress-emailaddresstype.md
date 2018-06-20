---
title: EmailAddress (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cdabfcb-7658-4c7d-bb03-1e776ed11e43
description: EmailAddress 要素は、サイトのメールボックス、または、関連付けられているため完全に解決済みの SMTP アドレスを指定します。
ms.openlocfilehash: c31a37fc0dbdcc2b501b82346a17a0a3b4775556
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760216"
---
# <a name="emailaddress-emailaddresstype"></a><span data-ttu-id="53deb-103">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="53deb-103">EmailAddress (EmailAddressType)</span></span>

<span data-ttu-id="53deb-104">**EmailAddress**要素は、サイトのメールボックス、または、関連付けられているため完全に解決済みの SMTP アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="53deb-104">The **EmailAddress** element specifies the fully resolved SMTP address for the site mailbox or the associated persona.</span></span> 
  
```xml
<EmailAddress>
    <Name></Name>
    <EmailAddress></EmailAddress>
    <RoutingType></RoutingType>
    <MailboxType></MailboxType>
    <ItemId></ItemId>
</EmailAddress>
```

 <span data-ttu-id="53deb-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="53deb-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="53deb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="53deb-106">Attributes and elements</span></span>

<span data-ttu-id="53deb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="53deb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="53deb-108">属性</span><span class="sxs-lookup"><span data-stu-id="53deb-108">Attributes</span></span>

<span data-ttu-id="53deb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="53deb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="53deb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="53deb-110">Child elements</span></span>

|<span data-ttu-id="53deb-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="53deb-111">**Element**</span></span>|<span data-ttu-id="53deb-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="53deb-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="53deb-113">名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="53deb-113">Name (string)</span></span>](name-string.md) <br/> |<span data-ttu-id="53deb-114">検索の絞り込み条件の名前またはキー、または、電子メール ユーザーの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="53deb-114">Specifies a search refiner name or key or the name of an email user.</span></span>  <br/> |
|[<span data-ttu-id="53deb-115">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="53deb-115">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="53deb-116">メールボックスのユーザーのプライマリ SMTP アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="53deb-116">Defines the primary SMTP address of a mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="53deb-117">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="53deb-117">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md) <br/> |<span data-ttu-id="53deb-118">電子メール アドレスのルーティングの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="53deb-118">Specifies the routing type of an email address.</span></span>  <br/> |
|[<span data-ttu-id="53deb-119">MailboxType</span><span class="sxs-lookup"><span data-stu-id="53deb-119">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="53deb-120">電子メール アドレスで表されるメールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="53deb-120">Represents the type of mailbox that is represented by the e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="53deb-121">ItemId</span><span class="sxs-lookup"><span data-stu-id="53deb-121">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="53deb-122">Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="53deb-122">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="53deb-123">親要素</span><span class="sxs-lookup"><span data-stu-id="53deb-123">Parent elements</span></span>

|<span data-ttu-id="53deb-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="53deb-124">**Element**</span></span>|<span data-ttu-id="53deb-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="53deb-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="53deb-126">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="53deb-126">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="53deb-127">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="53deb-127">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="53deb-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="53deb-128">Text value</span></span>

<span data-ttu-id="53deb-129">なし。</span><span class="sxs-lookup"><span data-stu-id="53deb-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="53deb-130">備考</span><span class="sxs-lookup"><span data-stu-id="53deb-130">Remarks</span></span>

<span data-ttu-id="53deb-131">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="53deb-131">This element is optional.</span></span>
  
<span data-ttu-id="53deb-132">**EmailAddress**要素は、オンラインの Exchange および Exchange 2013 を起動する Microsoft Exchange Server のバージョンを対象とするクライアントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="53deb-132">The **EmailAddress** element is applicable for clients that target Exchange Online and versions of Microsoft Exchange Server starting with Exchange 2013.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="53deb-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="53deb-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="53deb-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="53deb-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="53deb-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="53deb-135">Schema Name</span></span>  <br/> |<span data-ttu-id="53deb-136">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="53deb-136">Type schema</span></span>  <br/> |
|<span data-ttu-id="53deb-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="53deb-137">Validation File</span></span>  <br/> |<span data-ttu-id="53deb-138">types.xsd</span><span class="sxs-lookup"><span data-stu-id="53deb-138">types.xsd</span></span>  <br/> |
|<span data-ttu-id="53deb-139">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="53deb-139">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="53deb-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="53deb-140">See also</span></span>

- [<span data-ttu-id="53deb-141">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="53deb-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

