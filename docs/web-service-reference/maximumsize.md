---
title: MaximumSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fb7c3ab3-ef97-44c7-83e0-93cfe8c48e84
description: 作成要素は、メッセージ内に含まれる条件や例外条件を適用する順序の最大サイズを表します。
ms.openlocfilehash: 37e3d377b105534fe34b54e262bd47bc450706da
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832387"
---
# <a name="maximumsize"></a><span data-ttu-id="f0ef0-103">MaximumSize</span><span class="sxs-lookup"><span data-stu-id="f0ef0-103">MaximumSize</span></span>

<span data-ttu-id="f0ef0-104">**作成**要素は、メッセージ内に含まれる条件や例外条件を適用する順序の最大サイズを表します。</span><span class="sxs-lookup"><span data-stu-id="f0ef0-104">The **MaximumSize** element represents the maximum size that a message must be in order for the condition or exception to apply.</span></span> 
  
```XML
<Maximum/>
```

 <span data-ttu-id="f0ef0-105">**int**</span><span class="sxs-lookup"><span data-stu-id="f0ef0-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0ef0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f0ef0-106">Attributes and elements</span></span>

<span data-ttu-id="f0ef0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f0ef0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0ef0-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0ef0-108">Attributes</span></span>

<span data-ttu-id="f0ef0-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f0ef0-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f0ef0-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f0ef0-110">Child elements</span></span>

<span data-ttu-id="f0ef0-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f0ef0-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f0ef0-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f0ef0-112">Parent elements</span></span>

|<span data-ttu-id="f0ef0-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f0ef0-113">**Element**</span></span>|<span data-ttu-id="f0ef0-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f0ef0-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0ef0-115">WithinSizeRange</span><span class="sxs-lookup"><span data-stu-id="f0ef0-115">WithinSizeRange</span></span>](withinsizerange.md) <br/> |<span data-ttu-id="f0ef0-116">適用する場合の条件または例外の順序で受信メッセージをする必要のある最小値と最大サイズを指定します。</span><span class="sxs-lookup"><span data-stu-id="f0ef0-116">Specifies the minimum and maximum sizes that incoming messages must be in order for the condition or exception to apply.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f0ef0-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f0ef0-117">Text value</span></span>

<span data-ttu-id="f0ef0-118">テキスト値は、バイト単位でのメッセージの最大サイズを識別する整数です。</span><span class="sxs-lookup"><span data-stu-id="f0ef0-118">The text value is an integer that identifies the maximum size of the message in bytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f0ef0-119">備考</span><span class="sxs-lookup"><span data-stu-id="f0ef0-119">Remarks</span></span>

<span data-ttu-id="f0ef0-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f0ef0-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0ef0-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="f0ef0-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0ef0-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="f0ef0-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f0ef0-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f0ef0-123">Schema Name</span></span>  <br/> |<span data-ttu-id="f0ef0-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="f0ef0-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f0ef0-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f0ef0-125">Validation File</span></span>  <br/> |<span data-ttu-id="f0ef0-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f0ef0-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f0ef0-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f0ef0-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="f0ef0-128">True</span><span class="sxs-lookup"><span data-stu-id="f0ef0-128">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0ef0-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="f0ef0-129">See also</span></span>



[<span data-ttu-id="f0ef0-130">MinimumSize</span><span class="sxs-lookup"><span data-stu-id="f0ef0-130">MinimumSize</span></span>](minimumsize.md)


- [<span data-ttu-id="f0ef0-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f0ef0-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

