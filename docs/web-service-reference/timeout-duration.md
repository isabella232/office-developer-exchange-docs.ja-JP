---
title: タイムアウト (期間)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb15f9a7-8ea5-4765-9877-762c3f98bf50
description: Timeout 要素は、サーバーによってプルサブスクリプションがタイムアウトになるまでの時間の長さを指定します。
ms.openlocfilehash: b5b0e77d794080cd8e0da1e14acf4cb059b80b08
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460282"
---
# <a name="timeout-duration"></a><span data-ttu-id="8b29e-103">タイムアウト (期間)</span><span class="sxs-lookup"><span data-stu-id="8b29e-103">Timeout (duration)</span></span>

<span data-ttu-id="8b29e-104">**Timeout**要素は、サーバーによってプルサブスクリプションがタイムアウトになるまでの時間の長さを指定します。</span><span class="sxs-lookup"><span data-stu-id="8b29e-104">The **Timeout** element specifies the length of time before a pull subscription is timed out by the server.</span></span> 
  
```XML
<Timeout></Timeout>
```

 <span data-ttu-id="8b29e-105">**SubscriptionTimeoutType**</span><span class="sxs-lookup"><span data-stu-id="8b29e-105">**SubscriptionTimeoutType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8b29e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8b29e-106">Attributes and elements</span></span>

<span data-ttu-id="8b29e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8b29e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8b29e-108">属性</span><span class="sxs-lookup"><span data-stu-id="8b29e-108">Attributes</span></span>

<span data-ttu-id="8b29e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8b29e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8b29e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8b29e-110">Child elements</span></span>

<span data-ttu-id="8b29e-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8b29e-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8b29e-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8b29e-112">Parent elements</span></span>

[<span data-ttu-id="8b29e-113">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="8b29e-113">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
  
## <a name="text-value"></a><span data-ttu-id="8b29e-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8b29e-114">Text value</span></span>

<span data-ttu-id="8b29e-115">**Timeout**要素のテキスト値は、サーバーによってプルサブスクリプションがタイムアウトになるまでの時間 (分単位) です。</span><span class="sxs-lookup"><span data-stu-id="8b29e-115">The text value of the **Timeout** element is the length of time, in minutes, before a pull subscription is timed out by the server.</span></span> <span data-ttu-id="8b29e-116">最小値は1です。最大値は1440です。</span><span class="sxs-lookup"><span data-stu-id="8b29e-116">The minimum value is 1; the maximum value is 1440.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="8b29e-117">注釈</span><span class="sxs-lookup"><span data-stu-id="8b29e-117">Remarks</span></span>

<span data-ttu-id="8b29e-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8b29e-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8b29e-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8b29e-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8b29e-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8b29e-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8b29e-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="8b29e-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8b29e-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8b29e-122">Schema name</span></span>  <br/> |<span data-ttu-id="8b29e-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8b29e-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="8b29e-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8b29e-124">Validation file</span></span>  <br/> |<span data-ttu-id="8b29e-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8b29e-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8b29e-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8b29e-126">Can be empty</span></span>  <br/> ||
   

