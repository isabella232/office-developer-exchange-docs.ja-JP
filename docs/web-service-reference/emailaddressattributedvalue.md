---
title: EmailAddressAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ebdf224d-3796-4179-aa0a-87942e7585ff
description: EmailAddressAttributedValue 要素は、電子メール アドレスの配列と、関連付けられている帰属のインスタンスを指定します。
ms.openlocfilehash: 3bcbb5c0a2bc9a2dc24516b5fc62e6e3363a360b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760233"
---
# <a name="emailaddressattributedvalue"></a><span data-ttu-id="ea96a-103">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="ea96a-103">EmailAddressAttributedValue</span></span>

<span data-ttu-id="ea96a-104">**EmailAddressAttributedValue**要素は、電子メール アドレスの配列と、関連付けられている帰属のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="ea96a-104">The **EmailAddressAttributedValue** element specifies an instance of an array of email addresses and their associated attributions.</span></span> 
  
```XML
<EmailAddressAttributedValue>
    <Value></Value>
    <Attributions></Attributions>
<EmailAddressAttributedValue>
```

 <span data-ttu-id="ea96a-105">**EmailAddressAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="ea96a-105">**EmailAddressAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea96a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="ea96a-106">Attributes and elements</span></span>

<span data-ttu-id="ea96a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ea96a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea96a-108">属性</span><span class="sxs-lookup"><span data-stu-id="ea96a-108">Attributes</span></span>

<span data-ttu-id="ea96a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ea96a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ea96a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ea96a-110">Child elements</span></span>

|<span data-ttu-id="ea96a-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="ea96a-111">**Element**</span></span>|<span data-ttu-id="ea96a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ea96a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea96a-113">値 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="ea96a-113">Value (EmailAddressType)</span></span>](value-emailaddresstype.md) <br/> |<span data-ttu-id="ea96a-114">帰属配列に関連付け、 **EmailAddress**の値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ea96a-114">Specifies the value of an **EmailAddress** associated with an attributions array.</span></span>  <br/> |
|[<span data-ttu-id="ea96a-115">帰属 (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="ea96a-115">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md) <br/> |<span data-ttu-id="ea96a-116">帰属、関連付けられている**値**の要素の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="ea96a-116">Specifies an array of attributions for its associated **Value** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ea96a-117">親要素</span><span class="sxs-lookup"><span data-stu-id="ea96a-117">Parent elements</span></span>

|<span data-ttu-id="ea96a-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="ea96a-118">**Element**</span></span>|<span data-ttu-id="ea96a-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="ea96a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea96a-120">Emails1</span><span class="sxs-lookup"><span data-stu-id="ea96a-120">Emails1</span></span>](emails1.md) <br/> |<span data-ttu-id="ea96a-121">電子メールの値の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="ea96a-121">Specifies an array of email values and the identifiers of their source attributions for the associated persona.</span></span>  <br/> |
|[<span data-ttu-id="ea96a-122">Emails2</span><span class="sxs-lookup"><span data-stu-id="ea96a-122">Emails2</span></span>](emails2.md) <br/> |<span data-ttu-id="ea96a-123">電子メールの値の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="ea96a-123">Specifies an array of email values and the identifiers of their source attributions for the associated persona.</span></span>  <br/> |
|[<span data-ttu-id="ea96a-124">Emails3</span><span class="sxs-lookup"><span data-stu-id="ea96a-124">Emails3</span></span>](emails3.md) <br/> |<span data-ttu-id="ea96a-125">電子メールの値の配列と関連付けられているペルソナにそのソースの帰属の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="ea96a-125">Specifies an array of email values and the identifiers of their source attributions for the associated persona.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ea96a-126">備考</span><span class="sxs-lookup"><span data-stu-id="ea96a-126">Remarks</span></span>

<span data-ttu-id="ea96a-127">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ea96a-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="ea96a-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ea96a-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea96a-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="ea96a-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea96a-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="ea96a-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ea96a-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ea96a-131">Schema Name</span></span>  <br/> |<span data-ttu-id="ea96a-132">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="ea96a-132">Type schema</span></span>  <br/> |
|<span data-ttu-id="ea96a-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ea96a-133">Validation File</span></span>  <br/> |<span data-ttu-id="ea96a-134">types.xsd</span><span class="sxs-lookup"><span data-stu-id="ea96a-134">types.xsd</span></span>  <br/> |
|<span data-ttu-id="ea96a-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="ea96a-135">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="ea96a-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="ea96a-136">See also</span></span>



- [<span data-ttu-id="ea96a-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="ea96a-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

