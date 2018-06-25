---
title: スコープ (NonEmptyStringType)
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
description: スコープ要素は、メッセージ追跡レポートの範囲を指定します。
ms.openlocfilehash: 534ed23916a60b246c7cb5be4a59d086980a7c37
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833280"
---
# <a name="scope-nonemptystringtype"></a><span data-ttu-id="5dcc7-103">スコープ (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="5dcc7-103">Scope (NonEmptyStringType)</span></span>

<span data-ttu-id="5dcc7-104">**スコープ**要素は、メッセージ追跡レポートの範囲を指定します。</span><span class="sxs-lookup"><span data-stu-id="5dcc7-104">The **Scope** element specifies the scope of the message tracking report.</span></span> 
  
```XML
<Scope>Organization | Forest | Site</Scope>
```

 <span data-ttu-id="5dcc7-105">**NonEmptyStringType**</span><span class="sxs-lookup"><span data-stu-id="5dcc7-105">**NonEmptyStringType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5dcc7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5dcc7-106">Attributes and elements</span></span>

<span data-ttu-id="5dcc7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5dcc7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5dcc7-108">属性</span><span class="sxs-lookup"><span data-stu-id="5dcc7-108">Attributes</span></span>

<span data-ttu-id="5dcc7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5dcc7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5dcc7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5dcc7-110">Child elements</span></span>

<span data-ttu-id="5dcc7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5dcc7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5dcc7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5dcc7-112">Parent elements</span></span>

<span data-ttu-id="5dcc7-113">[FindMessageTrackingReport](findmessagetrackingreport.md) | [GetMessageTrackingReport](getmessagetrackingreport.md)</span><span class="sxs-lookup"><span data-stu-id="5dcc7-113">[FindMessageTrackingReport](findmessagetrackingreport.md) | [GetMessageTrackingReport](getmessagetrackingreport.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="5dcc7-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5dcc7-114">Text value</span></span>

<span data-ttu-id="5dcc7-115">**スコープ**要素の有効な値を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="5dcc7-115">The following table lists the possible values for the **Scope** element.</span></span> 
  
|<span data-ttu-id="5dcc7-116">**値**</span><span class="sxs-lookup"><span data-stu-id="5dcc7-116">**Value**</span></span>|<span data-ttu-id="5dcc7-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="5dcc7-117">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5dcc7-118">組織</span><span class="sxs-lookup"><span data-stu-id="5dcc7-118">Organization</span></span>  <br/> |<span data-ttu-id="5dcc7-119">組織全体にわたってメッセージ追跡用のスコープにまたがっています。</span><span class="sxs-lookup"><span data-stu-id="5dcc7-119">The message tracking scopes spans across an organization.</span></span>  <br/> |
|<span data-ttu-id="5dcc7-120">フォレスト</span><span class="sxs-lookup"><span data-stu-id="5dcc7-120">Forest</span></span>  <br/> |<span data-ttu-id="5dcc7-121">フォレストにまたがるメッセージのスコープを追跡できます。</span><span class="sxs-lookup"><span data-stu-id="5dcc7-121">The message tracking scopes spans across a forest.</span></span>  <br/> |
|<span data-ttu-id="5dcc7-122">サイト</span><span class="sxs-lookup"><span data-stu-id="5dcc7-122">Site</span></span>  <br/> |<span data-ttu-id="5dcc7-123">サイトにまたがるメッセージのスコープを追跡できます。</span><span class="sxs-lookup"><span data-stu-id="5dcc7-123">The message tracking scopes spans across a site.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5dcc7-124">備考</span><span class="sxs-lookup"><span data-stu-id="5dcc7-124">Remarks</span></span>

<span data-ttu-id="5dcc7-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5dcc7-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5dcc7-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="5dcc7-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5dcc7-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="5dcc7-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5dcc7-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5dcc7-128">Schema Name</span></span>  <br/> |<span data-ttu-id="5dcc7-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="5dcc7-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5dcc7-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5dcc7-130">Validation File</span></span>  <br/> |<span data-ttu-id="5dcc7-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5dcc7-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5dcc7-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5dcc7-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="5dcc7-133">False</span><span class="sxs-lookup"><span data-stu-id="5dcc7-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5dcc7-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="5dcc7-134">See also</span></span>



- [<span data-ttu-id="5dcc7-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5dcc7-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

