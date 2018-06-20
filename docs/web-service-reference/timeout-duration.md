---
title: タイムアウト (時間)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bb15f9a7-8ea5-4765-9877-762c3f98bf50
description: タイムアウト要素は、プル サブスクリプションの前に時間の長さは、サーバーでタイムアウトを指定します。
ms.openlocfilehash: 23b210dcdd87f2388aecec246068f12ec6c69a78
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839674"
---
# <a name="timeout-duration"></a><span data-ttu-id="2b4d7-103">タイムアウト (時間)</span><span class="sxs-lookup"><span data-stu-id="2b4d7-103">Timeout (duration)</span></span>

<span data-ttu-id="2b4d7-104">**タイムアウト**要素は、プル サブスクリプションの前に時間の長さは、サーバーでタイムアウトを指定します。</span><span class="sxs-lookup"><span data-stu-id="2b4d7-104">The **Timeout** element specifies the length of time before a pull subscription is timed out by the server.</span></span> 
  
```XML
<Timeout></Timeout>
```

 <span data-ttu-id="2b4d7-105">**SubscriptionTimeoutType**</span><span class="sxs-lookup"><span data-stu-id="2b4d7-105">**SubscriptionTimeoutType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b4d7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2b4d7-106">Attributes and elements</span></span>

<span data-ttu-id="2b4d7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2b4d7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b4d7-108">属性</span><span class="sxs-lookup"><span data-stu-id="2b4d7-108">Attributes</span></span>

<span data-ttu-id="2b4d7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2b4d7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b4d7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2b4d7-110">Child elements</span></span>

<span data-ttu-id="2b4d7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2b4d7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2b4d7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2b4d7-112">Parent elements</span></span>

[<span data-ttu-id="2b4d7-113">PullSubscriptionRequest</span><span class="sxs-lookup"><span data-stu-id="2b4d7-113">PullSubscriptionRequest</span></span>](pullsubscriptionrequest.md)
  
## <a name="text-value"></a><span data-ttu-id="2b4d7-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2b4d7-114">Text value</span></span>

<span data-ttu-id="2b4d7-115">**タイムアウト**要素のテキスト値は、プル サブスクリプションは、サーバーがタイムアウトする前に、分単位の時間の長さです。</span><span class="sxs-lookup"><span data-stu-id="2b4d7-115">The text value of the **Timeout** element is the length of time, in minutes, before a pull subscription is timed out by the server.</span></span> <span data-ttu-id="2b4d7-116">最小値は 1 です。最大値は、1440 です。</span><span class="sxs-lookup"><span data-stu-id="2b4d7-116">The minimum value is 1; the maximum value is 1440.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2b4d7-117">備考</span><span class="sxs-lookup"><span data-stu-id="2b4d7-117">Remarks</span></span>

<span data-ttu-id="2b4d7-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2b4d7-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="2b4d7-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2b4d7-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b4d7-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="2b4d7-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b4d7-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="2b4d7-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2b4d7-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2b4d7-122">Schema name</span></span>  <br/> |<span data-ttu-id="2b4d7-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="2b4d7-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="2b4d7-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2b4d7-124">Validation file</span></span>  <br/> |<span data-ttu-id="2b4d7-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2b4d7-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2b4d7-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2b4d7-126">Can be empty</span></span>  <br/> ||
   

