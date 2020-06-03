---
title: 連絡先 (ArrayOfContactsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a2c1e833-5f8c-438d-bad7-bb5dcc29ca9e
description: 連絡先要素は、連絡先の配列を指定します。
ms.openlocfilehash: eeb202f41fcf5ec7aad12a8a2b8e6dd539b3dba4
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529442"
---
# <a name="contacts-arrayofcontactstype"></a><span data-ttu-id="2a7c5-103">連絡先 (ArrayOfContactsType)</span><span class="sxs-lookup"><span data-stu-id="2a7c5-103">Contacts (ArrayOfContactsType)</span></span>

<span data-ttu-id="2a7c5-104">**連絡先**要素は、連絡先の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="2a7c5-104">The **Contacts** element specifies an array of contacts.</span></span> 
  
```XML
<Contacts>
    <Contact></Contact>
</Contacts>
```

 <span data-ttu-id="2a7c5-105">**ArrayOfContactsType**</span><span class="sxs-lookup"><span data-stu-id="2a7c5-105">**ArrayOfContactsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2a7c5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2a7c5-106">Attributes and elements</span></span>

<span data-ttu-id="2a7c5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2a7c5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a7c5-108">属性</span><span class="sxs-lookup"><span data-stu-id="2a7c5-108">Attributes</span></span>

<span data-ttu-id="2a7c5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2a7c5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2a7c5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2a7c5-110">Child elements</span></span>

|<span data-ttu-id="2a7c5-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="2a7c5-111">**Element**</span></span>|<span data-ttu-id="2a7c5-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2a7c5-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a7c5-113">Contact (ContactType)</span><span class="sxs-lookup"><span data-stu-id="2a7c5-113">Contact (ContactType)</span></span>](contact-contacttype.md) <br/> |<span data-ttu-id="2a7c5-114">統合連絡先ストアの連絡先を指定します。</span><span class="sxs-lookup"><span data-stu-id="2a7c5-114">Specifies a contact in the Unified Contact Store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2a7c5-115">親要素</span><span class="sxs-lookup"><span data-stu-id="2a7c5-115">Parent elements</span></span>

|<span data-ttu-id="2a7c5-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="2a7c5-116">**Element**</span></span>|<span data-ttu-id="2a7c5-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="2a7c5-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a7c5-118">EntityExtractionResult</span><span class="sxs-lookup"><span data-stu-id="2a7c5-118">EntityExtractionResult</span></span>](entityextractionresult.md) <br/> |<span data-ttu-id="2a7c5-119">アイテムの**Entityextractionresult**プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="2a7c5-119">Specifies the **EntityExtractionResult** property of an item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2a7c5-120">注釈</span><span class="sxs-lookup"><span data-stu-id="2a7c5-120">Remarks</span></span>

<span data-ttu-id="2a7c5-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2a7c5-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2a7c5-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2a7c5-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2a7c5-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2a7c5-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2a7c5-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="2a7c5-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2a7c5-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2a7c5-125">Schema Name</span></span>  <br/> |<span data-ttu-id="2a7c5-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="2a7c5-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="2a7c5-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2a7c5-127">Validation File</span></span>  <br/> |<span data-ttu-id="2a7c5-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="2a7c5-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="2a7c5-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2a7c5-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="2a7c5-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="2a7c5-130">See also</span></span>



- [<span data-ttu-id="2a7c5-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2a7c5-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

