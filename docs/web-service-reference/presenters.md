---
title: 発表者
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 01057872-4f1a-4246-86ba-73d10ef854a0
description: プレゼンター要素は、オンライン会議の発表者を指定します。
ms.openlocfilehash: f62b458759e0d8199c98827602d6c3fe16aebeea
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832875"
---
# <a name="presenters"></a><span data-ttu-id="8eabc-103">発表者</span><span class="sxs-lookup"><span data-stu-id="8eabc-103">Presenters</span></span>

<span data-ttu-id="8eabc-104">**プレゼンター**要素は、オンライン会議の発表者を指定します。</span><span class="sxs-lookup"><span data-stu-id="8eabc-104">The **Presenters** element specifies the presenters for an online meeting.</span></span> 
  
```XML
<Presenters> Disabled | Internal | Everyone </Presenters>
```

 <span data-ttu-id="8eabc-105">**PresentersType**</span><span class="sxs-lookup"><span data-stu-id="8eabc-105">**PresentersType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8eabc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8eabc-106">Attributes and elements</span></span>

<span data-ttu-id="8eabc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8eabc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8eabc-108">属性</span><span class="sxs-lookup"><span data-stu-id="8eabc-108">Attributes</span></span>

<span data-ttu-id="8eabc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8eabc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8eabc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8eabc-110">Child elements</span></span>

<span data-ttu-id="8eabc-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8eabc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8eabc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8eabc-112">Parent elements</span></span>

[<span data-ttu-id="8eabc-113">OnlineMeetingSettings</span><span class="sxs-lookup"><span data-stu-id="8eabc-113">OnlineMeetingSettings</span></span>](onlinemeetingsettings.md)
  
## <a name="text-value"></a><span data-ttu-id="8eabc-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8eabc-114">Text value</span></span>

<span data-ttu-id="8eabc-115">**発表者**の要素のテキスト値は、オンライン会議の発表者ことができるユーザーの種類です。</span><span class="sxs-lookup"><span data-stu-id="8eabc-115">The text value of **Presenters** element is the type of users that can be a presenter for an online meeting.</span></span> <span data-ttu-id="8eabc-116">**発表者**の要素のテキスト値は、次の表で説明します。</span><span class="sxs-lookup"><span data-stu-id="8eabc-116">The text values for the **Presenters** element are described in the following table.</span></span> 
  
<span data-ttu-id="8eabc-117">**要素のテキスト値を発表**</span><span class="sxs-lookup"><span data-stu-id="8eabc-117">**Presenters element text values**</span></span>

|<span data-ttu-id="8eabc-118">**値**</span><span class="sxs-lookup"><span data-stu-id="8eabc-118">**Value**</span></span>|<span data-ttu-id="8eabc-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="8eabc-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8eabc-120">無効</span><span class="sxs-lookup"><span data-stu-id="8eabc-120">Disabled</span></span>  <br/> |<span data-ttu-id="8eabc-121">発表者が無効になります。</span><span class="sxs-lookup"><span data-stu-id="8eabc-121">Presenters are disabled.</span></span>  <br/> |
|<span data-ttu-id="8eabc-122">内部</span><span class="sxs-lookup"><span data-stu-id="8eabc-122">Internal</span></span>  <br/> |<span data-ttu-id="8eabc-123">内部のみの参加者は、発表者を指定できます。</span><span class="sxs-lookup"><span data-stu-id="8eabc-123">Only internal participants can be presenters.</span></span>  <br/> |
|<span data-ttu-id="8eabc-124">全員</span><span class="sxs-lookup"><span data-stu-id="8eabc-124">Everyone</span></span>  <br/> |<span data-ttu-id="8eabc-125">任意の参加者、発表者ができます。</span><span class="sxs-lookup"><span data-stu-id="8eabc-125">Any participant can be a presenter.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8eabc-126">備考</span><span class="sxs-lookup"><span data-stu-id="8eabc-126">Remarks</span></span>

<span data-ttu-id="8eabc-127">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8eabc-127">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8eabc-128">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8eabc-128">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8eabc-129">要素情報</span><span class="sxs-lookup"><span data-stu-id="8eabc-129">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8eabc-130">名前空間</span><span class="sxs-lookup"><span data-stu-id="8eabc-130">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8eabc-131">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8eabc-131">Schema name</span></span>  <br/> |<span data-ttu-id="8eabc-132">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8eabc-132">Types schema</span></span>  <br/> |
|<span data-ttu-id="8eabc-133">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8eabc-133">Validation file</span></span>  <br/> |<span data-ttu-id="8eabc-134">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8eabc-134">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8eabc-135">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8eabc-135">Can be empty</span></span>  <br/> ||
   

