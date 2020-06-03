---
title: EmailAddresses (ArrayOfEmailAddressEntitiesType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2fc4a8e8-5377-4059-8fb4-3fdabfd30fe3
description: EmailAddresses 要素は、電子メールアドレスエンティティの配列を指定します。
ms.openlocfilehash: bd478b369f3b359edc6007db9231af50c36877e8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463427"
---
# <a name="emailaddresses-arrayofemailaddressentitiestype"></a><span data-ttu-id="76337-103">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span><span class="sxs-lookup"><span data-stu-id="76337-103">EmailAddresses (ArrayOfEmailAddressEntitiesType)</span></span>

<span data-ttu-id="76337-104">**Emailaddresses**要素は、電子メールアドレスエンティティの配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="76337-104">The **EmailAddresses** element specifies an array of email address entities.</span></span> 
  
```XML
<EmailAddresses>
    <EmailAddressEntity></EmailAddressEntity>
</EmailAddresses>
```

 <span data-ttu-id="76337-105">**ArrayOfEmailAddressEntitiesType**</span><span class="sxs-lookup"><span data-stu-id="76337-105">**ArrayOfEmailAddressEntitiesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="76337-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="76337-106">Attributes and elements</span></span>

<span data-ttu-id="76337-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="76337-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76337-108">属性</span><span class="sxs-lookup"><span data-stu-id="76337-108">Attributes</span></span>

<span data-ttu-id="76337-109">なし。</span><span class="sxs-lookup"><span data-stu-id="76337-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="76337-110">子要素</span><span class="sxs-lookup"><span data-stu-id="76337-110">Child elements</span></span>

|<span data-ttu-id="76337-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="76337-111">**Element**</span></span>|<span data-ttu-id="76337-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="76337-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76337-113">EmailAddressEntity</span><span class="sxs-lookup"><span data-stu-id="76337-113">EmailAddressEntity</span></span>](emailaddressentity.md) <br/> |<span data-ttu-id="76337-114">1つの電子メールアドレスエンティティを指定します。</span><span class="sxs-lookup"><span data-stu-id="76337-114">Specifies a single email address entity.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="76337-115">親要素</span><span class="sxs-lookup"><span data-stu-id="76337-115">Parent elements</span></span>

|<span data-ttu-id="76337-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="76337-116">**Element**</span></span>|<span data-ttu-id="76337-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="76337-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76337-118">EntityExtractionResult</span><span class="sxs-lookup"><span data-stu-id="76337-118">EntityExtractionResult</span></span>](entityextractionresult.md) <br/> |<span data-ttu-id="76337-119">アイテムの**Entityextractionresult**プロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="76337-119">Specifies the **EntityExtractionResult** property of an item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="76337-120">注釈</span><span class="sxs-lookup"><span data-stu-id="76337-120">Remarks</span></span>

<span data-ttu-id="76337-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="76337-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="76337-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="76337-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76337-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="76337-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76337-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="76337-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="76337-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="76337-125">Schema Name</span></span>  <br/> |<span data-ttu-id="76337-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="76337-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="76337-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="76337-127">Validation File</span></span>  <br/> |<span data-ttu-id="76337-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="76337-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="76337-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="76337-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="76337-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="76337-130">See also</span></span>



- [<span data-ttu-id="76337-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="76337-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

