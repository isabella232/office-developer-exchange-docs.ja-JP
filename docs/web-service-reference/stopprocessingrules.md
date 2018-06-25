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
description: StopProcessingRules 要素は、後のルールが評価されるかどうかを示します。
ms.openlocfilehash: 48799975f8c928bf291fcdcdb83f2ff8768af8b9
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833593"
---
# <a name="stopprocessingrules"></a><span data-ttu-id="59689-103">StopProcessingRules</span><span class="sxs-lookup"><span data-stu-id="59689-103">StopProcessingRules</span></span>

<span data-ttu-id="59689-104">**StopProcessingRules**要素は、後のルールが評価されるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="59689-104">The **StopProcessingRules** element indicates whether subsequent rules are to be evaluated.</span></span> 
  
```XML
<StopProcessingRules>true | false</StopProcessingRules>
```

 <span data-ttu-id="59689-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="59689-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59689-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="59689-106">Attributes and elements</span></span>

<span data-ttu-id="59689-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="59689-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59689-108">属性</span><span class="sxs-lookup"><span data-stu-id="59689-108">Attributes</span></span>

<span data-ttu-id="59689-109">なし。</span><span class="sxs-lookup"><span data-stu-id="59689-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59689-110">子要素</span><span class="sxs-lookup"><span data-stu-id="59689-110">Child elements</span></span>

<span data-ttu-id="59689-111">なし。</span><span class="sxs-lookup"><span data-stu-id="59689-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="59689-112">親要素</span><span class="sxs-lookup"><span data-stu-id="59689-112">Parent elements</span></span>

|<span data-ttu-id="59689-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="59689-113">**Element**</span></span>|<span data-ttu-id="59689-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="59689-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59689-115">アクション</span><span class="sxs-lookup"><span data-stu-id="59689-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="59689-116">条件が満たされるときに、メッセージに対して実行される使用可能なアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="59689-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="59689-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="59689-117">Text value</span></span>

<span data-ttu-id="59689-118">**True**の場合、テキスト値は、後のルールを処理しないことを示します。</span><span class="sxs-lookup"><span data-stu-id="59689-118">A text value of **true** indicates that subsequent rules should not be processed.</span></span> <span data-ttu-id="59689-119">**False**の値は、後のルールが評価されるように継続する必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="59689-119">A value of **false** indicates that subsequent rules should continue to be evaluated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="59689-120">備考</span><span class="sxs-lookup"><span data-stu-id="59689-120">Remarks</span></span>

<span data-ttu-id="59689-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="59689-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59689-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="59689-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59689-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="59689-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="59689-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="59689-124">Schema Name</span></span>  <br/> |<span data-ttu-id="59689-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="59689-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="59689-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="59689-126">Validation File</span></span>  <br/> |<span data-ttu-id="59689-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="59689-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="59689-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="59689-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="59689-129">True</span><span class="sxs-lookup"><span data-stu-id="59689-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59689-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="59689-130">See also</span></span>



- [<span data-ttu-id="59689-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="59689-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

