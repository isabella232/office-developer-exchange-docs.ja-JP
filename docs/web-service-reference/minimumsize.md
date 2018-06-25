---
title: MinimumSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 841d229c-140c-48bd-b3a7-21478fcea2fb
description: MinimumSize 要素は、メッセージが適用する条件または例外の順にする必要がある最小サイズを表します。
ms.openlocfilehash: 4f80bac3b9226019ec3d726cd2d6430e02cac423
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832480"
---
# <a name="minimumsize"></a><span data-ttu-id="5d0cf-103">MinimumSize</span><span class="sxs-lookup"><span data-stu-id="5d0cf-103">MinimumSize</span></span>

<span data-ttu-id="5d0cf-104">**MinimumSize**要素は、メッセージが適用する条件または例外の順にする必要がある最小サイズを表します。</span><span class="sxs-lookup"><span data-stu-id="5d0cf-104">The **MinimumSize** element represents the minimum size that a message must be in order for the condition or exception to apply.</span></span> 
  
```XML
<MinimumSize/>
```

 <span data-ttu-id="5d0cf-105">**int**</span><span class="sxs-lookup"><span data-stu-id="5d0cf-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5d0cf-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5d0cf-106">Attributes and elements</span></span>

<span data-ttu-id="5d0cf-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5d0cf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5d0cf-108">属性</span><span class="sxs-lookup"><span data-stu-id="5d0cf-108">Attributes</span></span>

<span data-ttu-id="5d0cf-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5d0cf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5d0cf-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5d0cf-110">Child elements</span></span>

<span data-ttu-id="5d0cf-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5d0cf-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5d0cf-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5d0cf-112">Parent elements</span></span>

|<span data-ttu-id="5d0cf-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5d0cf-113">**Element**</span></span>|<span data-ttu-id="5d0cf-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5d0cf-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5d0cf-115">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="5d0cf-115">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="5d0cf-116">適用する場合の条件または例外の順序で受信メッセージをする必要のある最小値と最大サイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="5d0cf-116">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5d0cf-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5d0cf-117">Text value</span></span>

<span data-ttu-id="5d0cf-118">テキスト値は、バイト単位でメッセージの最小サイズを識別する整数です。</span><span class="sxs-lookup"><span data-stu-id="5d0cf-118">The text value is an integer that identifies the minimum size of the message in bytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="5d0cf-119">備考</span><span class="sxs-lookup"><span data-stu-id="5d0cf-119">Remarks</span></span>

<span data-ttu-id="5d0cf-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5d0cf-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5d0cf-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="5d0cf-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5d0cf-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="5d0cf-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5d0cf-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5d0cf-123">Schema Name</span></span>  <br/> |<span data-ttu-id="5d0cf-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="5d0cf-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5d0cf-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5d0cf-125">Validation File</span></span>  <br/> |<span data-ttu-id="5d0cf-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5d0cf-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5d0cf-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5d0cf-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="5d0cf-128">True</span><span class="sxs-lookup"><span data-stu-id="5d0cf-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5d0cf-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="5d0cf-129">See also</span></span>



[<span data-ttu-id="5d0cf-130">作成</span><span class="sxs-lookup"><span data-stu-id="5d0cf-130">MaximumSize</span></span>](maximumsize.md)


- [<span data-ttu-id="5d0cf-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5d0cf-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

