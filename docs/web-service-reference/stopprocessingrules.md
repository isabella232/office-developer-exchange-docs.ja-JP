---
title: StopProcessingRules
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StopProcessingRules
api_type:
- schema
ms.assetid: 5b89a2cb-ab26-444d-b3dd-2b3858872d63
description: StopProcessingRules 要素は、後続のルールを評価する必要があるかどうかを示します。
ms.openlocfilehash: 9f068fd6290a39bbab6e3c1e29066c4fefefc64b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467901"
---
# <a name="stopprocessingrules"></a><span data-ttu-id="41e45-103">StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="41e45-103">StopProcessingRules</span></span>

<span data-ttu-id="41e45-104">**StopProcessingRules**要素は、後続のルールを評価する必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="41e45-104">The **StopProcessingRules** element indicates whether subsequent rules are to be evaluated.</span></span> 
  
```XML
<StopProcessingRules>true | false</StopProcessingRules>
```

 <span data-ttu-id="41e45-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="41e45-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="41e45-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="41e45-106">Attributes and elements</span></span>

<span data-ttu-id="41e45-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="41e45-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="41e45-108">属性</span><span class="sxs-lookup"><span data-stu-id="41e45-108">Attributes</span></span>

<span data-ttu-id="41e45-109">なし。</span><span class="sxs-lookup"><span data-stu-id="41e45-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="41e45-110">子要素</span><span class="sxs-lookup"><span data-stu-id="41e45-110">Child elements</span></span>

<span data-ttu-id="41e45-111">なし。</span><span class="sxs-lookup"><span data-stu-id="41e45-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="41e45-112">親要素</span><span class="sxs-lookup"><span data-stu-id="41e45-112">Parent elements</span></span>

|<span data-ttu-id="41e45-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="41e45-113">**Element**</span></span>|<span data-ttu-id="41e45-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="41e45-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="41e45-115">Actions</span><span class="sxs-lookup"><span data-stu-id="41e45-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="41e45-116">条件が満たされたときに、メッセージに対して実行できるアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="41e45-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="41e45-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="41e45-117">Text value</span></span>

<span data-ttu-id="41e45-118">テキスト値が**true の場合**、後続のルールは処理されないことを示します。</span><span class="sxs-lookup"><span data-stu-id="41e45-118">A text value of **true** indicates that subsequent rules should not be processed.</span></span> <span data-ttu-id="41e45-119">値が**false**の場合、後続のルールは引き続き評価される必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="41e45-119">A value of **false** indicates that subsequent rules should continue to be evaluated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="41e45-120">注釈</span><span class="sxs-lookup"><span data-stu-id="41e45-120">Remarks</span></span>

<span data-ttu-id="41e45-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="41e45-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="41e45-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="41e45-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="41e45-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="41e45-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="41e45-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="41e45-124">Schema Name</span></span>  <br/> |<span data-ttu-id="41e45-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="41e45-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="41e45-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="41e45-126">Validation File</span></span>  <br/> |<span data-ttu-id="41e45-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="41e45-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="41e45-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="41e45-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="41e45-129">正しい</span><span class="sxs-lookup"><span data-stu-id="41e45-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="41e45-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="41e45-130">See also</span></span>



- [<span data-ttu-id="41e45-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="41e45-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

