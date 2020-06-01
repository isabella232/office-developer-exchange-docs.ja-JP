---
title: Transition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Transition
api_type:
- schema
ms.assetid: 23ce171a-a9c9-47ed-a366-822777048eea
description: Transition 要素は、タイムゾーンの切り替えを表します。
ms.openlocfilehash: 05495eb4a493feedc88532cc4bc8b949493481f5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467495"
---
# <a name="transition"></a><span data-ttu-id="1d0f1-103">Transition</span><span class="sxs-lookup"><span data-stu-id="1d0f1-103">Transition</span></span>

<span data-ttu-id="1d0f1-104">**Transition**要素は、タイムゾーンの切り替えを表します。</span><span class="sxs-lookup"><span data-stu-id="1d0f1-104">The **Transition** element represents a time zone transition.</span></span> 
  
```xml
<Transition>
   <To/>
</Transition>
```

 <span data-ttu-id="1d0f1-105">**遷移 Tiontype**</span><span class="sxs-lookup"><span data-stu-id="1d0f1-105">**TransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1d0f1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1d0f1-106">Attributes and elements</span></span>

<span data-ttu-id="1d0f1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1d0f1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d0f1-108">属性</span><span class="sxs-lookup"><span data-stu-id="1d0f1-108">Attributes</span></span>

<span data-ttu-id="1d0f1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1d0f1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1d0f1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1d0f1-110">Child elements</span></span>

|<span data-ttu-id="1d0f1-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="1d0f1-111">**Element**</span></span>|<span data-ttu-id="1d0f1-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1d0f1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d0f1-113">To</span><span class="sxs-lookup"><span data-stu-id="1d0f1-113">To</span></span>](to.md) <br/> |<span data-ttu-id="1d0f1-114">タイムゾーンの遷移のターゲットである[期間](period.md)[または時間を指定](transitionsgroup.md)します。</span><span class="sxs-lookup"><span data-stu-id="1d0f1-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1d0f1-115">親要素</span><span class="sxs-lookup"><span data-stu-id="1d0f1-115">Parent elements</span></span>

|<span data-ttu-id="1d0f1-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="1d0f1-116">**Element**</span></span>|<span data-ttu-id="1d0f1-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="1d0f1-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d0f1-118">切り替わる</span><span class="sxs-lookup"><span data-stu-id="1d0f1-118">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="1d0f1-119">タイムゾーンの遷移のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="1d0f1-119">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1d0f1-120">注釈</span><span class="sxs-lookup"><span data-stu-id="1d0f1-120">Remarks</span></span>

<span data-ttu-id="1d0f1-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1d0f1-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1d0f1-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1d0f1-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d0f1-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="1d0f1-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1d0f1-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1d0f1-124">Schema Name</span></span>  <br/> |<span data-ttu-id="1d0f1-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="1d0f1-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="1d0f1-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1d0f1-126">Validation File</span></span>  <br/> |<span data-ttu-id="1d0f1-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1d0f1-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1d0f1-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1d0f1-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="1d0f1-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="1d0f1-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1d0f1-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="1d0f1-130">See also</span></span>



- [<span data-ttu-id="1d0f1-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1d0f1-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

