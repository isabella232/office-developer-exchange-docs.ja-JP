---
title: EmailAddressAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ebdf224d-3796-4179-aa0a-87942e7585ff
description: EmailAddressAttributedValue 要素は、電子メールアドレスの配列のインスタンスと、それに関連付けられている attributions を指定します。
ms.openlocfilehash: 09fdd5921cef3d70a6da4b6d4d38f08834c5d482
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530692"
---
# <a name="emailaddressattributedvalue"></a><span data-ttu-id="e3381-103">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="e3381-103">EmailAddressAttributedValue</span></span>

<span data-ttu-id="e3381-104">**EmailAddressAttributedValue**要素は、電子メールアドレスの配列のインスタンスと、それに関連付けられている attributions を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3381-104">The **EmailAddressAttributedValue** element specifies an instance of an array of email addresses and their associated attributions.</span></span> 
  
```XML
<EmailAddressAttributedValue>
    <Value></Value>
    <Attributions></Attributions>
<EmailAddressAttributedValue>
```

 <span data-ttu-id="e3381-105">**EmailAddressAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="e3381-105">**EmailAddressAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3381-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e3381-106">Attributes and elements</span></span>

<span data-ttu-id="e3381-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e3381-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3381-108">属性</span><span class="sxs-lookup"><span data-stu-id="e3381-108">Attributes</span></span>

<span data-ttu-id="e3381-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e3381-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e3381-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e3381-110">Child elements</span></span>

|<span data-ttu-id="e3381-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="e3381-111">**Element**</span></span>|<span data-ttu-id="e3381-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e3381-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3381-113">値 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="e3381-113">Value (EmailAddressType)</span></span>](value-emailaddresstype.md) <br/> |<span data-ttu-id="e3381-114">Attributions 配列に関連付けられている**EmailAddress**の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3381-114">Specifies the value of an **EmailAddress** associated with an attributions array.</span></span>  <br/> |
|[<span data-ttu-id="e3381-115">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="e3381-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="e3381-116">関連する**Value**要素の attributions の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3381-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e3381-117">親要素</span><span class="sxs-lookup"><span data-stu-id="e3381-117">Parent elements</span></span>

|<span data-ttu-id="e3381-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="e3381-118">**Element**</span></span>|<span data-ttu-id="e3381-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="e3381-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3381-120">Emails1</span><span class="sxs-lookup"><span data-stu-id="e3381-120">Emails1</span></span>](emails1.md) <br/> |<span data-ttu-id="e3381-121">電子メール値の配列と、関連付けられているペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3381-121">Specifies an array of email values and the identifiers of their source attributions for the associated persona.</span></span>  <br/> |
|[<span data-ttu-id="e3381-122">Emails2</span><span class="sxs-lookup"><span data-stu-id="e3381-122">Emails2</span></span>](emails2.md) <br/> |<span data-ttu-id="e3381-123">電子メール値の配列と、関連付けられているペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3381-123">Specifies an array of email values and the identifiers of their source attributions for the associated persona.</span></span>  <br/> |
|[<span data-ttu-id="e3381-124">Emails3</span><span class="sxs-lookup"><span data-stu-id="e3381-124">Emails3</span></span>](emails3.md) <br/> |<span data-ttu-id="e3381-125">電子メール値の配列と、関連付けられているペルソナのソース attributions の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3381-125">Specifies an array of email values and the identifiers of their source attributions for the associated persona.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e3381-126">注釈</span><span class="sxs-lookup"><span data-stu-id="e3381-126">Remarks</span></span>

<span data-ttu-id="e3381-127">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e3381-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e3381-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e3381-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3381-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e3381-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3381-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="e3381-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e3381-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e3381-131">Schema Name</span></span>  <br/> |<span data-ttu-id="e3381-132">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="e3381-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="e3381-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e3381-133">Validation File</span></span>  <br/> |<span data-ttu-id="e3381-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e3381-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e3381-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e3381-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e3381-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="e3381-136">See also</span></span>



- [<span data-ttu-id="e3381-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e3381-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

