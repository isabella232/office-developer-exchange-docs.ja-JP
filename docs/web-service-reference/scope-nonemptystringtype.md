---
title: 範囲 (非 Emptystringtype)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Scope
api_type:
- schema
ms.assetid: 7efb6fd9-1615-469e-96f6-0f7846ad9b44
description: Scope 要素は、メッセージ追跡レポートの範囲を指定します。
ms.openlocfilehash: f86f6198e84e094e61ee569f6d005549316bbb9b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466942"
---
# <a name="scope-nonemptystringtype"></a><span data-ttu-id="e0dbd-103">範囲 (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="e0dbd-103">Scope (NonEmptyStringType)</span></span>

<span data-ttu-id="e0dbd-104">**Scope**要素は、メッセージ追跡レポートの範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="e0dbd-104">The **Scope** element specifies the scope of the message tracking report.</span></span> 
  
```XML
<Scope>Organization | Forest | Site</Scope>
```

 <span data-ttu-id="e0dbd-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="e0dbd-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e0dbd-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e0dbd-106">Attributes and elements</span></span>

<span data-ttu-id="e0dbd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e0dbd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e0dbd-108">属性</span><span class="sxs-lookup"><span data-stu-id="e0dbd-108">Attributes</span></span>

<span data-ttu-id="e0dbd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e0dbd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e0dbd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e0dbd-110">Child elements</span></span>

<span data-ttu-id="e0dbd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e0dbd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e0dbd-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e0dbd-112">Parent elements</span></span>

<span data-ttu-id="e0dbd-113">[Findmessagetrackingreport](findmessagetrackingreport.md)  | [Getmessagetrackingreport](getmessagetrackingreport.md)</span><span class="sxs-lookup"><span data-stu-id="e0dbd-113">[FindMessageTrackingReport](findmessagetrackingreport.md) | [GetMessageTrackingReport](getmessagetrackingreport.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="e0dbd-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e0dbd-114">Text value</span></span>

<span data-ttu-id="e0dbd-115">次の表に、 **Scope**要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="e0dbd-115">The following table lists the possible values for the **Scope** element.</span></span> 
  
|<span data-ttu-id="e0dbd-116">**値**</span><span class="sxs-lookup"><span data-stu-id="e0dbd-116">**Value**</span></span>|<span data-ttu-id="e0dbd-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="e0dbd-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e0dbd-118">組織</span><span class="sxs-lookup"><span data-stu-id="e0dbd-118">Organization</span></span>  <br/> |<span data-ttu-id="e0dbd-119">メッセージ追跡スコープは組織全体に及びます。</span><span class="sxs-lookup"><span data-stu-id="e0dbd-119">The message tracking scopes spans across an organization.</span></span>  <br/> |
|<span data-ttu-id="e0dbd-120">Forest</span><span class="sxs-lookup"><span data-stu-id="e0dbd-120">Forest</span></span>  <br/> |<span data-ttu-id="e0dbd-121">メッセージ追跡スコープはフォレスト全体に及びます。</span><span class="sxs-lookup"><span data-stu-id="e0dbd-121">The message tracking scopes spans across a forest.</span></span>  <br/> |
|<span data-ttu-id="e0dbd-122">サイト</span><span class="sxs-lookup"><span data-stu-id="e0dbd-122">Site</span></span>  <br/> |<span data-ttu-id="e0dbd-123">メッセージ追跡スコープはサイト全体にわたっています。</span><span class="sxs-lookup"><span data-stu-id="e0dbd-123">The message tracking scopes spans across a site.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e0dbd-124">注釈</span><span class="sxs-lookup"><span data-stu-id="e0dbd-124">Remarks</span></span>

<span data-ttu-id="e0dbd-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e0dbd-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e0dbd-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e0dbd-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e0dbd-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="e0dbd-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e0dbd-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e0dbd-128">Schema Name</span></span>  <br/> |<span data-ttu-id="e0dbd-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="e0dbd-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e0dbd-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e0dbd-130">Validation File</span></span>  <br/> |<span data-ttu-id="e0dbd-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="e0dbd-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e0dbd-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e0dbd-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="e0dbd-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="e0dbd-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e0dbd-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="e0dbd-134">See also</span></span>



- [<span data-ttu-id="e0dbd-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e0dbd-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

