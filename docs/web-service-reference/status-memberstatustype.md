---
title: 状態 (MemberStatusType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Status
api_type:
- schema
ms.assetid: 4f8a860b-0a48-4a0d-9a7a-69a0304aa747
description: 状態の要素は、サーバー上の配布リストのメンバーの状態に関する情報を提供します。
ms.openlocfilehash: ef062433c80f0cca413c33012e1164b17e226faf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833580"
---
# <a name="status-memberstatustype"></a><span data-ttu-id="af16d-103">状態 (MemberStatusType)</span><span class="sxs-lookup"><span data-stu-id="af16d-103">Status (MemberStatusType)</span></span>

<span data-ttu-id="af16d-104">**状態**の要素は、サーバー上の配布リストのメンバーの状態に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="af16d-104">The **Status** element provides information about the status of a distribution list member on the server.</span></span> 
  
```
<Status>Unrecognized or Normal or Demoted</Status>
```

 <span data-ttu-id="af16d-105">**MemberStatusType**</span><span class="sxs-lookup"><span data-stu-id="af16d-105">**MemberStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af16d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="af16d-106">Attributes and elements</span></span>

<span data-ttu-id="af16d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="af16d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af16d-108">属性</span><span class="sxs-lookup"><span data-stu-id="af16d-108">Attributes</span></span>

<span data-ttu-id="af16d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="af16d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af16d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="af16d-110">Child elements</span></span>

<span data-ttu-id="af16d-111">なし。</span><span class="sxs-lookup"><span data-stu-id="af16d-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="af16d-112">親要素</span><span class="sxs-lookup"><span data-stu-id="af16d-112">Parent elements</span></span>

|<span data-ttu-id="af16d-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="af16d-113">**Element**</span></span>|<span data-ttu-id="af16d-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="af16d-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af16d-115">メンバー</span><span class="sxs-lookup"><span data-stu-id="af16d-115">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="af16d-116">配布リストのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="af16d-116">Represents a member of a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="af16d-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="af16d-117">Text value</span></span>

<span data-ttu-id="af16d-118">**状態**の要素の値を次の表に一覧します。</span><span class="sxs-lookup"><span data-stu-id="af16d-118">The following table lists the possible values for the **Status** element.</span></span> 
  
<span data-ttu-id="af16d-119">**要素のステータス値**</span><span class="sxs-lookup"><span data-stu-id="af16d-119">**Status element values**</span></span>

|<span data-ttu-id="af16d-120">**値**</span><span class="sxs-lookup"><span data-stu-id="af16d-120">**Value**</span></span>|<span data-ttu-id="af16d-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="af16d-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="af16d-122">認識されません。</span><span class="sxs-lookup"><span data-stu-id="af16d-122">Unrecognized</span></span>  <br/> |<span data-ttu-id="af16d-123">メンバー情報は、無効なまたは認識されません。</span><span class="sxs-lookup"><span data-stu-id="af16d-123">Member information is invalid or unrecognized.</span></span>  <br/> |
|<span data-ttu-id="af16d-124">Normal</span><span class="sxs-lookup"><span data-stu-id="af16d-124">Normal</span></span>  <br/> |<span data-ttu-id="af16d-125">配布リストのメンバー情報は、参照されるオブジェクトとの同期します。</span><span class="sxs-lookup"><span data-stu-id="af16d-125">Member information in a distribution list is in sync with the referenced object.</span></span>  <br/> |
|<span data-ttu-id="af16d-126">降格</span><span class="sxs-lookup"><span data-stu-id="af16d-126">Demoted</span></span>  <br/> |<span data-ttu-id="af16d-127">参照先のオブジェクトでは使用できません。</span><span class="sxs-lookup"><span data-stu-id="af16d-127">Referenced object is not available.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="af16d-128">備考</span><span class="sxs-lookup"><span data-stu-id="af16d-128">Remarks</span></span>

<span data-ttu-id="af16d-129">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="af16d-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af16d-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="af16d-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af16d-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="af16d-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="af16d-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="af16d-132">Schema Name</span></span>  <br/> |<span data-ttu-id="af16d-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="af16d-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="af16d-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="af16d-134">Validation File</span></span>  <br/> |<span data-ttu-id="af16d-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="af16d-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="af16d-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="af16d-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="af16d-137">False</span><span class="sxs-lookup"><span data-stu-id="af16d-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af16d-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="af16d-138">See also</span></span>



- [<span data-ttu-id="af16d-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="af16d-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

