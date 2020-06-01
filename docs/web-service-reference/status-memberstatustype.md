---
title: Status (MemberStatusType)
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
description: Status 要素は、サーバー上の配布リストのメンバーの状態に関する情報を提供します。
ms.openlocfilehash: bfa0c349d6af51c1b2238c9749d2656541d31906
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465465"
---
# <a name="status-memberstatustype"></a><span data-ttu-id="5a032-103">Status (MemberStatusType)</span><span class="sxs-lookup"><span data-stu-id="5a032-103">Status (MemberStatusType)</span></span>

<span data-ttu-id="5a032-104">**Status**要素は、サーバー上の配布リストのメンバーの状態に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="5a032-104">The **Status** element provides information about the status of a distribution list member on the server.</span></span> 
  
```
<Status>Unrecognized or Normal or Demoted</Status>
```

 <span data-ttu-id="5a032-105">**MemberStatusType**</span><span class="sxs-lookup"><span data-stu-id="5a032-105">**MemberStatusType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5a032-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5a032-106">Attributes and elements</span></span>

<span data-ttu-id="5a032-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5a032-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5a032-108">属性</span><span class="sxs-lookup"><span data-stu-id="5a032-108">Attributes</span></span>

<span data-ttu-id="5a032-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5a032-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5a032-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5a032-110">Child elements</span></span>

<span data-ttu-id="5a032-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5a032-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5a032-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5a032-112">Parent elements</span></span>

|<span data-ttu-id="5a032-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5a032-113">**Element**</span></span>|<span data-ttu-id="5a032-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5a032-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5a032-115">メンバー</span><span class="sxs-lookup"><span data-stu-id="5a032-115">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5a032-116">配布リストのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="5a032-116">Represents a member of a distribution list.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5a032-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5a032-117">Text value</span></span>

<span data-ttu-id="5a032-118">次の表に、 **Status**要素に指定できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="5a032-118">The following table lists the possible values for the **Status** element.</span></span> 
  
<span data-ttu-id="5a032-119">**Status 要素の値**</span><span class="sxs-lookup"><span data-stu-id="5a032-119">**Status element values**</span></span>

|<span data-ttu-id="5a032-120">**値**</span><span class="sxs-lookup"><span data-stu-id="5a032-120">**Value**</span></span>|<span data-ttu-id="5a032-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="5a032-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5a032-122">認識できない</span><span class="sxs-lookup"><span data-stu-id="5a032-122">Unrecognized</span></span>  <br/> |<span data-ttu-id="5a032-123">メンバー情報が無効であるか、認識されません。</span><span class="sxs-lookup"><span data-stu-id="5a032-123">Member information is invalid or unrecognized.</span></span>  <br/> |
|<span data-ttu-id="5a032-124">標準</span><span class="sxs-lookup"><span data-stu-id="5a032-124">Normal</span></span>  <br/> |<span data-ttu-id="5a032-125">配布リスト内のメンバー情報は、参照されているオブジェクトと同期しています。</span><span class="sxs-lookup"><span data-stu-id="5a032-125">Member information in a distribution list is in sync with the referenced object.</span></span>  <br/> |
|<span data-ttu-id="5a032-126">差し戻し</span><span class="sxs-lookup"><span data-stu-id="5a032-126">Demoted</span></span>  <br/> |<span data-ttu-id="5a032-127">参照されるオブジェクトは使用できません。</span><span class="sxs-lookup"><span data-stu-id="5a032-127">Referenced object is not available.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5a032-128">注釈</span><span class="sxs-lookup"><span data-stu-id="5a032-128">Remarks</span></span>

<span data-ttu-id="5a032-129">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5a032-129">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5a032-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5a032-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5a032-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="5a032-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5a032-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5a032-132">Schema Name</span></span>  <br/> |<span data-ttu-id="5a032-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="5a032-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="5a032-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5a032-134">Validation File</span></span>  <br/> |<span data-ttu-id="5a032-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="5a032-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5a032-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5a032-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="5a032-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="5a032-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5a032-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="5a032-138">See also</span></span>



- [<span data-ttu-id="5a032-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5a032-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

