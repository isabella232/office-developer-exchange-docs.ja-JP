---
title: MinimumSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 841d229c-140c-48bd-b3a7-21478fcea2fb
description: MinimumSize 要素は、条件または例外を適用するためにメッセージが必要とされる最小サイズを表します。
ms.openlocfilehash: b43a8b5916747c4e3e4ca9b66cf8b9d73f5f8942
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464204"
---
# <a name="minimumsize"></a><span data-ttu-id="7e215-103">MinimumSize</span><span class="sxs-lookup"><span data-stu-id="7e215-103">MinimumSize</span></span>

<span data-ttu-id="7e215-104">**Minimumsize**要素は、条件または例外を適用するためにメッセージが必要とされる最小サイズを表します。</span><span class="sxs-lookup"><span data-stu-id="7e215-104">The **MinimumSize** element represents the minimum size that a message must be in order for the condition or exception to apply.</span></span> 
  
```XML
<MinimumSize/>
```

 <span data-ttu-id="7e215-105">**int**</span><span class="sxs-lookup"><span data-stu-id="7e215-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e215-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7e215-106">Attributes and elements</span></span>

<span data-ttu-id="7e215-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7e215-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e215-108">属性</span><span class="sxs-lookup"><span data-stu-id="7e215-108">Attributes</span></span>

<span data-ttu-id="7e215-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7e215-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e215-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7e215-110">Child elements</span></span>

<span data-ttu-id="7e215-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7e215-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7e215-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7e215-112">Parent elements</span></span>

|<span data-ttu-id="7e215-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="7e215-113">**Element**</span></span>|<span data-ttu-id="7e215-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e215-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e215-115">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="7e215-115">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="7e215-116">条件または例外を適用するために、受信メッセージが必要とする最小サイズと最大サイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="7e215-116">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7e215-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7e215-117">Text value</span></span>

<span data-ttu-id="7e215-118">テキスト値は、メッセージの最小サイズをバイト単位で示す整数です。</span><span class="sxs-lookup"><span data-stu-id="7e215-118">The text value is an integer that identifies the minimum size of the message in bytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7e215-119">注釈</span><span class="sxs-lookup"><span data-stu-id="7e215-119">Remarks</span></span>

<span data-ttu-id="7e215-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7e215-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e215-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7e215-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e215-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="7e215-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7e215-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7e215-123">Schema Name</span></span>  <br/> |<span data-ttu-id="7e215-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="7e215-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7e215-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7e215-125">Validation File</span></span>  <br/> |<span data-ttu-id="7e215-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7e215-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7e215-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7e215-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e215-128">正しい</span><span class="sxs-lookup"><span data-stu-id="7e215-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e215-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="7e215-129">See also</span></span>



[<span data-ttu-id="7e215-130">MaximumSize</span><span class="sxs-lookup"><span data-stu-id="7e215-130">MaximumSize</span></span>](maximumsize.md)


- [<span data-ttu-id="7e215-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7e215-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

