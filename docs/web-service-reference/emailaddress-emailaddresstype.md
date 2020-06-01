---
title: EmailAddress (EmailAddressType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cdabfcb-7658-4c7d-bb03-1e776ed11e43
description: EmailAddress 要素は、サイトメールボックスまたは関連するペルソナの完全に解決された SMTP アドレスを指定します。
ms.openlocfilehash: 8b04b75e91cc16be7f88c9a0ac08c5e36855056e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463462"
---
# <a name="emailaddress-emailaddresstype"></a><span data-ttu-id="f280c-103">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="f280c-103">EmailAddress (EmailAddressType)</span></span>

<span data-ttu-id="f280c-104">**EmailAddress**要素は、サイトメールボックスまたは関連するペルソナの完全に解決された SMTP アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="f280c-104">The **EmailAddress** element specifies the fully resolved SMTP address for the site mailbox or the associated persona.</span></span> 
  
```xml
<EmailAddress>
    <Name></Name>
    <EmailAddress></EmailAddress>
    <RoutingType></RoutingType>
    <MailboxType></MailboxType>
    <ItemId></ItemId>
</EmailAddress>
```

 <span data-ttu-id="f280c-105">**EmailAddressType**</span><span class="sxs-lookup"><span data-stu-id="f280c-105">**EmailAddressType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f280c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f280c-106">Attributes and elements</span></span>

<span data-ttu-id="f280c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f280c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f280c-108">属性</span><span class="sxs-lookup"><span data-stu-id="f280c-108">Attributes</span></span>

<span data-ttu-id="f280c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f280c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f280c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f280c-110">Child elements</span></span>

|<span data-ttu-id="f280c-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="f280c-111">**Element**</span></span>|<span data-ttu-id="f280c-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f280c-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f280c-113">Name (string)</span><span class="sxs-lookup"><span data-stu-id="f280c-113">Name (string)</span></span>](name-string.md) <br/> |<span data-ttu-id="f280c-114">検索絞り込み条件の名前またはキーまたはメールユーザーの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="f280c-114">Specifies a search refiner name or key or the name of an email user.</span></span>  <br/> |
|[<span data-ttu-id="f280c-115">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="f280c-115">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md) <br/> |<span data-ttu-id="f280c-116">メールボックスユーザーのプライマリ SMTP アドレスを定義します。</span><span class="sxs-lookup"><span data-stu-id="f280c-116">Defines the primary SMTP address of a mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="f280c-117">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="f280c-117">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md) <br/> |<span data-ttu-id="f280c-118">電子メールアドレスのルーティングの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="f280c-118">Specifies the routing type of an email address.</span></span>  <br/> |
|[<span data-ttu-id="f280c-119">MailboxType</span><span class="sxs-lookup"><span data-stu-id="f280c-119">MailboxType</span></span>](mailboxtype.md) <br/> |<span data-ttu-id="f280c-120">電子メールアドレスによって表されるメールボックスの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="f280c-120">Represents the type of mailbox that is represented by the e-mail address.</span></span>  <br/> |
|[<span data-ttu-id="f280c-121">ItemId</span><span class="sxs-lookup"><span data-stu-id="f280c-121">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="f280c-122">Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="f280c-122">Contains the unique identifier and change key of an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f280c-123">親要素</span><span class="sxs-lookup"><span data-stu-id="f280c-123">Parent elements</span></span>

|<span data-ttu-id="f280c-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="f280c-124">**Element**</span></span>|<span data-ttu-id="f280c-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="f280c-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f280c-126">ユーザー</span><span class="sxs-lookup"><span data-stu-id="f280c-126">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="f280c-127">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="f280c-127">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f280c-128">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f280c-128">Text value</span></span>

<span data-ttu-id="f280c-129">なし。</span><span class="sxs-lookup"><span data-stu-id="f280c-129">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f280c-130">注釈</span><span class="sxs-lookup"><span data-stu-id="f280c-130">Remarks</span></span>

<span data-ttu-id="f280c-131">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="f280c-131">This element is optional.</span></span>
  
<span data-ttu-id="f280c-132">**EmailAddress**要素は、exchange Online および exchange 2013 以降のバージョンの Microsoft exchange Server を対象とするクライアントに適用されます。</span><span class="sxs-lookup"><span data-stu-id="f280c-132">The **EmailAddress** element is applicable for clients that target Exchange Online and versions of Microsoft Exchange Server starting with Exchange 2013.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="f280c-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f280c-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f280c-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="f280c-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f280c-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f280c-135">Schema Name</span></span>  <br/> |<span data-ttu-id="f280c-136">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="f280c-136">Type schema</span></span>  <br/> |
|<span data-ttu-id="f280c-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f280c-137">Validation File</span></span>  <br/> |<span data-ttu-id="f280c-138">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f280c-138">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f280c-139">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f280c-139">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f280c-140">関連項目</span><span class="sxs-lookup"><span data-stu-id="f280c-140">See also</span></span>

- [<span data-ttu-id="f280c-141">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f280c-141">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

