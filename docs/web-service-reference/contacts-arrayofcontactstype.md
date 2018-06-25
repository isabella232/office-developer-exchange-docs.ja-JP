---
title: 連絡先 (ArrayOfContactsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a2c1e833-5f8c-438d-bad7-bb5dcc29ca9e
description: 連絡先の要素は、連絡先の配列を指定します。
ms.openlocfilehash: 01aab90d28c5d9706a45a2e42be1e60221394e80
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759676"
---
# <a name="contacts-arrayofcontactstype"></a><span data-ttu-id="3def1-103">連絡先 (ArrayOfContactsType)</span><span class="sxs-lookup"><span data-stu-id="3def1-103">Contacts (ArrayOfContactsType)</span></span>

<span data-ttu-id="3def1-104">**連絡先**の要素は、連絡先の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="3def1-104">The **Contacts** element specifies an array of contacts.</span></span> 
  
```XML
<Contacts>
    <Contact></Contact>
</Contacts>
```

 <span data-ttu-id="3def1-105">**ArrayOfContactsType**</span><span class="sxs-lookup"><span data-stu-id="3def1-105">**ArrayOfContactsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3def1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3def1-106">Attributes and elements</span></span>

<span data-ttu-id="3def1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3def1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3def1-108">属性</span><span class="sxs-lookup"><span data-stu-id="3def1-108">Attributes</span></span>

<span data-ttu-id="3def1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3def1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3def1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3def1-110">Child elements</span></span>

|<span data-ttu-id="3def1-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="3def1-111">**Element**</span></span>|<span data-ttu-id="3def1-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3def1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3def1-113">連絡先 (ContactType)</span><span class="sxs-lookup"><span data-stu-id="3def1-113">Contact (ContactType)</span></span>](contact-contacttype.md) <br/> |<span data-ttu-id="3def1-114">統合連絡先ストアには、取引先担当者を指定します。</span><span class="sxs-lookup"><span data-stu-id="3def1-114">Specifies a contact in the Unified Contact Store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3def1-115">親要素</span><span class="sxs-lookup"><span data-stu-id="3def1-115">Parent elements</span></span>

|<span data-ttu-id="3def1-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="3def1-116">**Element**</span></span>|<span data-ttu-id="3def1-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="3def1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3def1-118">EntityExtractionResult</span><span class="sxs-lookup"><span data-stu-id="3def1-118">EntityExtractionResult</span></span>](entityextractionresult.md) <br/> |<span data-ttu-id="3def1-119">項目の**EntityExtractionResult**プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="3def1-119">Specifies the **EntityExtractionResult** property of an item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3def1-120">備考</span><span class="sxs-lookup"><span data-stu-id="3def1-120">Remarks</span></span>

<span data-ttu-id="3def1-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3def1-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3def1-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3def1-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3def1-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="3def1-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3def1-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="3def1-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3def1-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3def1-125">Schema Name</span></span>  <br/> |<span data-ttu-id="3def1-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="3def1-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="3def1-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3def1-127">Validation File</span></span>  <br/> |<span data-ttu-id="3def1-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="3def1-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="3def1-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3def1-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3def1-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="3def1-130">See also</span></span>



- [<span data-ttu-id="3def1-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3def1-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

