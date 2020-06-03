---
title: ReferenceAttachment
ms.date: 7/7/2016
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: b9bde862-6b75-4a81-8033-00a47be4dc2f
description: ReferenceAttachment 要素は、XXX を指定します。
ms.openlocfilehash: a5e4445b24395f1530e072f8aa9b5a9eed02f671
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468741"
---
# <a name="referenceattachment"></a><span data-ttu-id="c965c-103">ReferenceAttachment</span><span class="sxs-lookup"><span data-stu-id="c965c-103">ReferenceAttachment</span></span>

<span data-ttu-id="c965c-104">**Referenceattachment**要素は、XXX を指定します。</span><span class="sxs-lookup"><span data-stu-id="c965c-104">The **ReferenceAttachment** element specifies XXX.</span></span> 
  
```XML
<RecurringMasterItemIdRanges Id="" ChangeKey="">
   <Ranges/>
</RecurringMasterItemIdRanges>
```

 <span data-ttu-id="c965c-105">**ReferenceAttachmen**</span><span class="sxs-lookup"><span data-stu-id="c965c-105">**ReferenceAttachmen**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c965c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c965c-106">Attributes and elements</span></span>

<span data-ttu-id="c965c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c965c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c965c-108">属性</span><span class="sxs-lookup"><span data-stu-id="c965c-108">Attributes</span></span>

|<span data-ttu-id="c965c-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="c965c-109">**Attribute**</span></span>|<span data-ttu-id="c965c-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="c965c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c965c-111">**Id**</span><span class="sxs-lookup"><span data-stu-id="c965c-111">**Id**</span></span> <br/> |<span data-ttu-id="c965c-112">**Id**属性のテキスト値は、定期的なマスターアイテムの一意識別子です。</span><span class="sxs-lookup"><span data-stu-id="c965c-112">The text value of the **Id** attribute is a recurring master item's unique identifier.</span></span> <span data-ttu-id="c965c-113">これは、**文字列型 (string** ) の値です。</span><span class="sxs-lookup"><span data-stu-id="c965c-113">This is a **string** value.</span></span>  <br/> |
|<span data-ttu-id="c965c-114">**ChangeKey**</span><span class="sxs-lookup"><span data-stu-id="c965c-114">**ChangeKey**</span></span> <br/> |<span data-ttu-id="c965c-115">**Changekey**属性のテキスト値は、定期的なマスターアイテムの変更キーです。</span><span class="sxs-lookup"><span data-stu-id="c965c-115">The text value of the **ChangeKey** attribute is the recurring master item's change key.</span></span> <span data-ttu-id="c965c-116">これは、**文字列型 (string** ) の値です。</span><span class="sxs-lookup"><span data-stu-id="c965c-116">This is a **string** value.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c965c-117">子要素</span><span class="sxs-lookup"><span data-stu-id="c965c-117">Child elements</span></span>

<span data-ttu-id="c965c-118">範囲</span><span class="sxs-lookup"><span data-stu-id="c965c-118">Ranges</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c965c-119">親要素</span><span class="sxs-lookup"><span data-stu-id="c965c-119">Parent elements</span></span>

<span data-ttu-id="c965c-120">ItemIds |GlobalItemIds |DraftItemIds |ContactIds |Groupid</span><span class="sxs-lookup"><span data-stu-id="c965c-120">ItemIds | GlobalItemIds | DraftItemIds| ContactIds | GroupIds</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c965c-121">注釈</span><span class="sxs-lookup"><span data-stu-id="c965c-121">Remarks</span></span>

<span data-ttu-id="c965c-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c965c-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c965c-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c965c-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c965c-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c965c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c965c-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="c965c-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c965c-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c965c-126">Schema name</span></span>  <br/> |<span data-ttu-id="c965c-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c965c-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="c965c-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c965c-128">Validation file</span></span>  <br/> |<span data-ttu-id="c965c-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c965c-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c965c-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c965c-130">Can be empty</span></span>  <br/> ||
   

