---
title: メンバー (MemberListType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Members
api_type:
- schema
ms.assetid: cbd38049-2ef7-40bf-9bec-0469af0f58ec
description: メンバーの要素は、配布リストのメンバーの一覧を提供します。
ms.openlocfilehash: 8cf9ed7a64a908614ce7be30a9bef631739fcebf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832439"
---
# <a name="members-memberlisttype"></a><span data-ttu-id="3fca7-103">メンバー (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="3fca7-103">Members (MemberListType)</span></span>

<span data-ttu-id="3fca7-104">**メンバー**の要素は、配布リストのメンバーの一覧を提供します。</span><span class="sxs-lookup"><span data-stu-id="3fca7-104">The **Members** element provides the list of members for a distribution list.</span></span> 
  
```xml
<Members>
   <Member/>
</Members>
```

<span data-ttu-id="3fca7-105">**MemberListType**</span><span class="sxs-lookup"><span data-stu-id="3fca7-105">**MemberListType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="3fca7-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3fca7-106">Attributes and elements</span></span>

<span data-ttu-id="3fca7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3fca7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3fca7-108">属性</span><span class="sxs-lookup"><span data-stu-id="3fca7-108">Attributes</span></span>

<span data-ttu-id="3fca7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3fca7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3fca7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3fca7-110">Child elements</span></span>

|<span data-ttu-id="3fca7-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="3fca7-111">**Element**</span></span>|<span data-ttu-id="3fca7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3fca7-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3fca7-113">メンバー</span><span class="sxs-lookup"><span data-stu-id="3fca7-113">Member</span></span>](member-ex15websvcsotherref.md) <br/> |<span data-ttu-id="3fca7-114">完全に解決された電子メール アドレス、およびサーバー上でそのアドレスの状態の識別子を提供します。</span><span class="sxs-lookup"><span data-stu-id="3fca7-114">Provides an identifier for a fully resolved e-mail address, and the status of that address on the server.</span></span> <span data-ttu-id="3fca7-115">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="3fca7-115">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3fca7-116">親要素</span><span class="sxs-lookup"><span data-stu-id="3fca7-116">Parent elements</span></span>

|<span data-ttu-id="3fca7-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="3fca7-117">**Element**</span></span>|<span data-ttu-id="3fca7-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="3fca7-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3fca7-119">DistributionList</span><span class="sxs-lookup"><span data-stu-id="3fca7-119">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="3fca7-120">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="3fca7-120">Represents a distribution list.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3fca7-121">備考</span><span class="sxs-lookup"><span data-stu-id="3fca7-121">Remarks</span></span>

<span data-ttu-id="3fca7-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3fca7-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3fca7-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="3fca7-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3fca7-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="3fca7-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3fca7-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3fca7-125">Schema Name</span></span>  <br/> |<span data-ttu-id="3fca7-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="3fca7-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="3fca7-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3fca7-127">Validation File</span></span>  <br/> |<span data-ttu-id="3fca7-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3fca7-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3fca7-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3fca7-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="3fca7-130">False</span><span class="sxs-lookup"><span data-stu-id="3fca7-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3fca7-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="3fca7-131">See also</span></span>

- [<span data-ttu-id="3fca7-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3fca7-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

