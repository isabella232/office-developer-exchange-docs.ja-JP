---
title: メンバー
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Member
api_type:
- schema
ms.assetid: af9c5ff8-02a4-41fc-876d-14ac05f1ee77
description: メンバーの要素は、配布リストのメンバーを表します。
ms.openlocfilehash: c38e2ed24e78b5199d4d65cce27a00a8e6704037
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/21/2018
ms.locfileid: "19832434"
---
# <a name="member"></a><span data-ttu-id="d2fa4-103">メンバー</span><span class="sxs-lookup"><span data-stu-id="d2fa4-103">Member</span></span>

<span data-ttu-id="d2fa4-104">**メンバー**の要素は、配布リストのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="d2fa4-104">The **Member** element represents a member of a distribution list.</span></span> 
  
```xml
<Member Key="">
   <Mailbox/>
   <Status/>
</Member>
```

<span data-ttu-id="d2fa4-105">**MemberType**</span><span class="sxs-lookup"><span data-stu-id="d2fa4-105">**MemberType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d2fa4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d2fa4-106">Attributes and elements</span></span>

<span data-ttu-id="d2fa4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d2fa4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2fa4-108">属性</span><span class="sxs-lookup"><span data-stu-id="d2fa4-108">Attributes</span></span>

|<span data-ttu-id="d2fa4-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="d2fa4-109">**Attribute**</span></span>|<span data-ttu-id="d2fa4-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2fa4-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d2fa4-111">キー</span><span class="sxs-lookup"><span data-stu-id="d2fa4-111">Key</span></span>  <br/> |<span data-ttu-id="d2fa4-112">配布リストのメンバーの一意の識別子を提供します。</span><span class="sxs-lookup"><span data-stu-id="d2fa4-112">Provides a unique identifier for the distribution list member.</span></span> <span data-ttu-id="d2fa4-113">この属性は、省略可能です。</span><span class="sxs-lookup"><span data-stu-id="d2fa4-113">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d2fa4-114">子要素</span><span class="sxs-lookup"><span data-stu-id="d2fa4-114">Child elements</span></span>

|<span data-ttu-id="d2fa4-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="d2fa4-115">**Element**</span></span>|<span data-ttu-id="d2fa4-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2fa4-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2fa4-117">メールボックス</span><span class="sxs-lookup"><span data-stu-id="d2fa4-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="d2fa4-118">配布リストのメンバーの電子メール アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="d2fa4-118">Represents the e-mail address of the distribution list member.</span></span> <span data-ttu-id="d2fa4-119">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="d2fa4-119">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="d2fa4-120">状態 (MemberStatusType)</span><span class="sxs-lookup"><span data-stu-id="d2fa4-120">Status (MemberStatusType)</span></span>](status-memberstatustype.md) <br/> |<span data-ttu-id="d2fa4-121">配布リストのメンバーの状態に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="d2fa4-121">Provides information about the status of a distribution list member.</span></span> <span data-ttu-id="d2fa4-122">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="d2fa4-122">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d2fa4-123">親要素</span><span class="sxs-lookup"><span data-stu-id="d2fa4-123">Parent elements</span></span>

|<span data-ttu-id="d2fa4-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="d2fa4-124">**Element**</span></span>|<span data-ttu-id="d2fa4-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2fa4-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2fa4-126">メンバー (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="d2fa4-126">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="d2fa4-127">配布リストのメンバーの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d2fa4-127">Contains a list of distribution list members.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d2fa4-128">備考</span><span class="sxs-lookup"><span data-stu-id="d2fa4-128">Remarks</span></span>

<span data-ttu-id="d2fa4-129">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d2fa4-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2fa4-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="d2fa4-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2fa4-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="d2fa4-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d2fa4-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d2fa4-132">Schema Name</span></span>  <br/> |<span data-ttu-id="d2fa4-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d2fa4-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="d2fa4-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d2fa4-134">Validation File</span></span>  <br/> |<span data-ttu-id="d2fa4-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d2fa4-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d2fa4-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d2fa4-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="d2fa4-137">False</span><span class="sxs-lookup"><span data-stu-id="d2fa4-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2fa4-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="d2fa4-138">See also</span></span>

- [<span data-ttu-id="d2fa4-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d2fa4-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

