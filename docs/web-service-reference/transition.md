---
title: 遷移
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
description: 遷移要素では、タイム ゾーンの移行を表します。
ms.openlocfilehash: 5dcd2f0dae7c3df2dcf660d6fe1a41b216c67b59
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839751"
---
# <a name="transition"></a><span data-ttu-id="d90e2-103">遷移</span><span class="sxs-lookup"><span data-stu-id="d90e2-103">Transition</span></span>

<span data-ttu-id="d90e2-104">**遷移**要素では、タイム ゾーンの移行を表します。</span><span class="sxs-lookup"><span data-stu-id="d90e2-104">The **Transition** element represents a time zone transition.</span></span> 
  
```xml
<Transition>
   <To/>
</Transition>
```

 <span data-ttu-id="d90e2-105">**TransitionType**</span><span class="sxs-lookup"><span data-stu-id="d90e2-105">**TransitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d90e2-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d90e2-106">Attributes and elements</span></span>

<span data-ttu-id="d90e2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d90e2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d90e2-108">属性</span><span class="sxs-lookup"><span data-stu-id="d90e2-108">Attributes</span></span>

<span data-ttu-id="d90e2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d90e2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d90e2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d90e2-110">Child elements</span></span>

|<span data-ttu-id="d90e2-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d90e2-111">**Element**</span></span>|<span data-ttu-id="d90e2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d90e2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d90e2-113">To</span><span class="sxs-lookup"><span data-stu-id="d90e2-113">To</span></span>](to.md) <br/> |<span data-ttu-id="d90e2-114">[TransitionsGroup](transitionsgroup.md)タイム ゾーンの移行の対象となる[期間](period.md)を指定します。</span><span class="sxs-lookup"><span data-stu-id="d90e2-114">Specifies the [Period](period.md) or [TransitionsGroup](transitionsgroup.md) that is the target of the time zone transition.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d90e2-115">親要素</span><span class="sxs-lookup"><span data-stu-id="d90e2-115">Parent elements</span></span>

|<span data-ttu-id="d90e2-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="d90e2-116">**Element**</span></span>|<span data-ttu-id="d90e2-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="d90e2-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d90e2-118">遷移</span><span class="sxs-lookup"><span data-stu-id="d90e2-118">Transitions</span></span>](transitions.md) <br/> |<span data-ttu-id="d90e2-119">タイム ゾーンの切り替え効果のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="d90e2-119">Represents a collection of time zone transitions.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d90e2-120">備考</span><span class="sxs-lookup"><span data-stu-id="d90e2-120">Remarks</span></span>

<span data-ttu-id="d90e2-121">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d90e2-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d90e2-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="d90e2-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d90e2-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="d90e2-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d90e2-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d90e2-124">Schema Name</span></span>  <br/> |<span data-ttu-id="d90e2-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d90e2-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="d90e2-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d90e2-126">Validation File</span></span>  <br/> |<span data-ttu-id="d90e2-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d90e2-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d90e2-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d90e2-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="d90e2-129">False</span><span class="sxs-lookup"><span data-stu-id="d90e2-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d90e2-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="d90e2-130">See also</span></span>



- [<span data-ttu-id="d90e2-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d90e2-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

