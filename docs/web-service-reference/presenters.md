---
title: プレゼン
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: プレゼンター要素は、オンライン会議のプレゼンターを指定します。
ms.openlocfilehash: 0236457020dfc4684569e84d3d54e357af00d102
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529911"
---
# <a name="presenters"></a><span data-ttu-id="dd451-103">プレゼン</span><span class="sxs-lookup"><span data-stu-id="dd451-103">Presenters</span></span>

<span data-ttu-id="dd451-104">**プレゼンター**要素は、オンライン会議のプレゼンターを指定します。</span><span class="sxs-lookup"><span data-stu-id="dd451-104">The **Presenters** element specifies the presenters for an online meeting.</span></span> 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 <span data-ttu-id="dd451-105">**PresentersType**</span><span class="sxs-lookup"><span data-stu-id="dd451-105">**PresentersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd451-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="dd451-106">Attributes and elements</span></span>

<span data-ttu-id="dd451-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dd451-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd451-108">属性</span><span class="sxs-lookup"><span data-stu-id="dd451-108">Attributes</span></span>

<span data-ttu-id="dd451-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dd451-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd451-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dd451-110">Child elements</span></span>

<span data-ttu-id="dd451-111">なし。</span><span class="sxs-lookup"><span data-stu-id="dd451-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dd451-112">親要素</span><span class="sxs-lookup"><span data-stu-id="dd451-112">Parent elements</span></span>

[<span data-ttu-id="dd451-113">OnlineMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="dd451-113">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md)
  
## <a name="text-value"></a><span data-ttu-id="dd451-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="dd451-114">Text value</span></span>

<span data-ttu-id="dd451-115">**プレゼンター**要素のテキスト値は、オンライン会議の発表者になることができるユーザーの種類です。</span><span class="sxs-lookup"><span data-stu-id="dd451-115">The text value of **Presenters** element is the type of users that can be a presenter for an online meeting.</span></span> <span data-ttu-id="dd451-116">次の表では、**プレゼンター**要素のテキスト値について説明します。</span><span class="sxs-lookup"><span data-stu-id="dd451-116">The text values for the **Presenters** element are described in the following table.</span></span> 
  
<span data-ttu-id="dd451-117">**プレゼンター要素のテキスト値**</span><span class="sxs-lookup"><span data-stu-id="dd451-117">**Presenters element text values**</span></span>

|<span data-ttu-id="dd451-118">**値**</span><span class="sxs-lookup"><span data-stu-id="dd451-118">**Value**</span></span>|<span data-ttu-id="dd451-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="dd451-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="dd451-120">無効</span><span class="sxs-lookup"><span data-stu-id="dd451-120">Disabled</span></span>  <br/> |<span data-ttu-id="dd451-121">プレゼンターは無効になっています。</span><span class="sxs-lookup"><span data-stu-id="dd451-121">Presenters are disabled.</span></span>  <br/> |
|<span data-ttu-id="dd451-122">内部</span><span class="sxs-lookup"><span data-stu-id="dd451-122">Internal</span></span>  <br/> |<span data-ttu-id="dd451-123">内部参加者のみがプレゼンターになることができます。</span><span class="sxs-lookup"><span data-stu-id="dd451-123">Only internal participants can be presenters.</span></span>  <br/> |
|<span data-ttu-id="dd451-124">すべてのユーザー</span><span class="sxs-lookup"><span data-stu-id="dd451-124">Everyone</span></span>  <br/> |<span data-ttu-id="dd451-125">参加者はすべて発表者になることができます。</span><span class="sxs-lookup"><span data-stu-id="dd451-125">Any participant can be a presenter.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="dd451-126">注釈</span><span class="sxs-lookup"><span data-stu-id="dd451-126">Remarks</span></span>

<span data-ttu-id="dd451-127">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="dd451-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="dd451-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="dd451-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd451-129">要素の情報</span><span class="sxs-lookup"><span data-stu-id="dd451-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd451-130">Namespace</span><span class="sxs-lookup"><span data-stu-id="dd451-130">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dd451-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dd451-131">Schema name</span></span>  <br/> |<span data-ttu-id="dd451-132">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="dd451-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="dd451-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dd451-133">Validation file</span></span>  <br/> |<span data-ttu-id="dd451-134">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="dd451-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dd451-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="dd451-135">Can be empty</span></span>  <br/> ||
   

