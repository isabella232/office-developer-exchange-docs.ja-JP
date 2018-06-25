---
title: MarkImportance
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MarkImportance
api_type:
- schema
ms.assetid: 32b8b08f-65e9-4764-b40a-63245551f4a3
description: MarkImportance 要素は、メッセージにスタンプするのには重要度を指定します。
ms.openlocfilehash: 32b1fa63ef47327e7d3af717ed9f452e43b16380
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832356"
---
# <a name="markimportance"></a><span data-ttu-id="4472e-103">MarkImportance</span><span class="sxs-lookup"><span data-stu-id="4472e-103">MarkImportance</span></span>

<span data-ttu-id="4472e-104">**MarkImportance**要素は、メッセージにスタンプするのには重要度を指定します。</span><span class="sxs-lookup"><span data-stu-id="4472e-104">The **MarkImportance** element specifies the importance that is to be stamped on messages.</span></span> 
  
```XML
<MarkImportance/>
```

 <span data-ttu-id="4472e-105">**ImportanceChoicesType**</span><span class="sxs-lookup"><span data-stu-id="4472e-105">**ImportanceChoicesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4472e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4472e-106">Attributes and elements</span></span>

<span data-ttu-id="4472e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4472e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4472e-108">属性</span><span class="sxs-lookup"><span data-stu-id="4472e-108">Attributes</span></span>

<span data-ttu-id="4472e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4472e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4472e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4472e-110">Child elements</span></span>

<span data-ttu-id="4472e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4472e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4472e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4472e-112">Parent elements</span></span>

|<span data-ttu-id="4472e-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4472e-113">**Element**</span></span>|<span data-ttu-id="4472e-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4472e-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4472e-115">アクション</span><span class="sxs-lookup"><span data-stu-id="4472e-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="4472e-116">条件が満たされるときに、メッセージに対して実行される使用可能なアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="4472e-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4472e-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4472e-117">Text value</span></span>

<span data-ttu-id="4472e-118">この要素のテキスト値は、次の文字列値の 1 つに制限されています。</span><span class="sxs-lookup"><span data-stu-id="4472e-118">The text value for this element is restricted to one of the following string values:</span></span>
  
- <span data-ttu-id="4472e-119">低</span><span class="sxs-lookup"><span data-stu-id="4472e-119">Low</span></span>
    
- <span data-ttu-id="4472e-120">Normal</span><span class="sxs-lookup"><span data-stu-id="4472e-120">Normal</span></span>
    
- <span data-ttu-id="4472e-121">高</span><span class="sxs-lookup"><span data-stu-id="4472e-121">High</span></span>
    
## <a name="remarks"></a><span data-ttu-id="4472e-122">備考</span><span class="sxs-lookup"><span data-stu-id="4472e-122">Remarks</span></span>

<span data-ttu-id="4472e-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4472e-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4472e-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="4472e-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4472e-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="4472e-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4472e-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4472e-126">Schema Name</span></span>  <br/> |<span data-ttu-id="4472e-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="4472e-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4472e-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4472e-128">Validation File</span></span>  <br/> |<span data-ttu-id="4472e-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4472e-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4472e-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4472e-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="4472e-131">True</span><span class="sxs-lookup"><span data-stu-id="4472e-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4472e-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="4472e-132">See also</span></span>



- [<span data-ttu-id="4472e-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4472e-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

