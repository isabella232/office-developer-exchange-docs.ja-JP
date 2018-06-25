---
title: EmailAddresses (ArrayOfEmailAddressEntitiesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2fc4a8e8-5377-4059-8fb4-3fdabfd30fe3
description: EmailAddresses 要素は、電子メール アドレスのエンティティの配列を指定します。
ms.openlocfilehash: 8d96d49ef2420f269197e47577efb956daa64e53
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760231"
---
# <a name="emailaddresses-arrayofemailaddressentitiestype"></a><span data-ttu-id="4ba83-103">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="4ba83-103">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span></span>

<span data-ttu-id="4ba83-104">**EmailAddresses**要素は、電子メール アドレスのエンティティの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="4ba83-104">The **EmailAddresses** element specifies an array of email address entities.</span></span> 
  
```XML
<EmailAddresses>
    <EmailAddressEntity></EmailAddressEntity>
</EmailAddresses>
```

 <span data-ttu-id="4ba83-105">**ArrayOfEmailAddressEntitiesType**</span><span class="sxs-lookup"><span data-stu-id="4ba83-105">**ArrayOfEmailAddressEntitiesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4ba83-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4ba83-106">Attributes and elements</span></span>

<span data-ttu-id="4ba83-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4ba83-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4ba83-108">属性</span><span class="sxs-lookup"><span data-stu-id="4ba83-108">Attributes</span></span>

<span data-ttu-id="4ba83-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4ba83-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4ba83-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4ba83-110">Child elements</span></span>

|<span data-ttu-id="4ba83-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="4ba83-111">**Element**</span></span>|<span data-ttu-id="4ba83-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4ba83-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ba83-113">EmailAddressEntity</span><span class="sxs-lookup"><span data-stu-id="4ba83-113">EmailAddressEntity</span></span>](emailaddressentity.md) <br/> |<span data-ttu-id="4ba83-114">1 つの e メール アドレスのエンティティを指定します。</span><span class="sxs-lookup"><span data-stu-id="4ba83-114">Specifies a single email address entity.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4ba83-115">親要素</span><span class="sxs-lookup"><span data-stu-id="4ba83-115">Parent elements</span></span>

|<span data-ttu-id="4ba83-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="4ba83-116">**Element**</span></span>|<span data-ttu-id="4ba83-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="4ba83-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4ba83-118">EntityExtractionResult</span><span class="sxs-lookup"><span data-stu-id="4ba83-118">EntityExtractionResult</span></span>](entityextractionresult.md) <br/> |<span data-ttu-id="4ba83-119">項目の**EntityExtractionResult**プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="4ba83-119">Specifies the **EntityExtractionResult** property of an item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="4ba83-120">備考</span><span class="sxs-lookup"><span data-stu-id="4ba83-120">Remarks</span></span>

<span data-ttu-id="4ba83-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4ba83-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4ba83-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4ba83-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4ba83-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="4ba83-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4ba83-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="4ba83-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4ba83-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4ba83-125">Schema Name</span></span>  <br/> |<span data-ttu-id="4ba83-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="4ba83-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="4ba83-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4ba83-127">Validation File</span></span>  <br/> |<span data-ttu-id="4ba83-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="4ba83-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4ba83-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4ba83-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4ba83-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="4ba83-130">See also</span></span>



- [<span data-ttu-id="4ba83-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4ba83-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

