---
title: マーク (重要)
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
description: MarkImportance な要素は、メッセージにスタンプされる重要度を指定します。
ms.openlocfilehash: 051307c0943a22e0c46439410806d168603d8a69
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530882"
---
# <a name="markimportance"></a><span data-ttu-id="7e54b-103">マーク (重要)</span><span class="sxs-lookup"><span data-stu-id="7e54b-103">MarkImportance</span></span>

<span data-ttu-id="7e54b-104">**Markimportance**な要素は、メッセージにスタンプされる重要度を指定します。</span><span class="sxs-lookup"><span data-stu-id="7e54b-104">The **MarkImportance** element specifies the importance that is to be stamped on messages.</span></span> 
  
```XML
<MarkImportance/>
```

 <span data-ttu-id="7e54b-105">**ImportanceChoicesType**</span><span class="sxs-lookup"><span data-stu-id="7e54b-105">**ImportanceChoicesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e54b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7e54b-106">Attributes and elements</span></span>

<span data-ttu-id="7e54b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7e54b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e54b-108">属性</span><span class="sxs-lookup"><span data-stu-id="7e54b-108">Attributes</span></span>

<span data-ttu-id="7e54b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7e54b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e54b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7e54b-110">Child elements</span></span>

<span data-ttu-id="7e54b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7e54b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7e54b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7e54b-112">Parent elements</span></span>

|<span data-ttu-id="7e54b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="7e54b-113">**Element**</span></span>|<span data-ttu-id="7e54b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e54b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e54b-115">Actions</span><span class="sxs-lookup"><span data-stu-id="7e54b-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="7e54b-116">条件が満たされたときに、メッセージに対して実行できるアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="7e54b-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7e54b-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7e54b-117">Text value</span></span>

<span data-ttu-id="7e54b-118">この要素のテキスト値は、次のいずれかの文字列値に制限されています。</span><span class="sxs-lookup"><span data-stu-id="7e54b-118">The text value for this element is restricted to one of the following string values:</span></span>
  
- <span data-ttu-id="7e54b-119">低</span><span class="sxs-lookup"><span data-stu-id="7e54b-119">Low</span></span>
    
- <span data-ttu-id="7e54b-120">標準</span><span class="sxs-lookup"><span data-stu-id="7e54b-120">Normal</span></span>
    
- <span data-ttu-id="7e54b-121">高</span><span class="sxs-lookup"><span data-stu-id="7e54b-121">High</span></span>
    
## <a name="remarks"></a><span data-ttu-id="7e54b-122">注釈</span><span class="sxs-lookup"><span data-stu-id="7e54b-122">Remarks</span></span>

<span data-ttu-id="7e54b-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7e54b-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e54b-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7e54b-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e54b-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="7e54b-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7e54b-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7e54b-126">Schema Name</span></span>  <br/> |<span data-ttu-id="7e54b-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="7e54b-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7e54b-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7e54b-128">Validation File</span></span>  <br/> |<span data-ttu-id="7e54b-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7e54b-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7e54b-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7e54b-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e54b-131">正しい</span><span class="sxs-lookup"><span data-stu-id="7e54b-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e54b-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="7e54b-132">See also</span></span>



- [<span data-ttu-id="7e54b-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7e54b-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

