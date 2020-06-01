---
title: Member
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
description: Member 要素は、配布リストのメンバーを表します。
ms.openlocfilehash: e84223b7c41846ca2f174293bff46a8825777a0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457306"
---
# <a name="member"></a><span data-ttu-id="38258-103">Member</span><span class="sxs-lookup"><span data-stu-id="38258-103">Member</span></span>

<span data-ttu-id="38258-104">**Member**要素は、配布リストのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="38258-104">The **Member** element represents a member of a distribution list.</span></span> 
  
```xml
<Member Key="">
   <Mailbox/>
   <Status/>
</Member>
```

<span data-ttu-id="38258-105">**MemberType**</span><span class="sxs-lookup"><span data-stu-id="38258-105">**MemberType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="38258-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="38258-106">Attributes and elements</span></span>

<span data-ttu-id="38258-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="38258-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="38258-108">属性</span><span class="sxs-lookup"><span data-stu-id="38258-108">Attributes</span></span>

|<span data-ttu-id="38258-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="38258-109">**Attribute**</span></span>|<span data-ttu-id="38258-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="38258-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="38258-111">キー</span><span class="sxs-lookup"><span data-stu-id="38258-111">Key</span></span>  <br/> |<span data-ttu-id="38258-112">配布リストのメンバーの一意の識別子を提供します。</span><span class="sxs-lookup"><span data-stu-id="38258-112">Provides a unique identifier for the distribution list member.</span></span> <span data-ttu-id="38258-113">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="38258-113">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="38258-114">子要素</span><span class="sxs-lookup"><span data-stu-id="38258-114">Child elements</span></span>

|<span data-ttu-id="38258-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="38258-115">**Element**</span></span>|<span data-ttu-id="38258-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="38258-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38258-117">メールボックス</span><span class="sxs-lookup"><span data-stu-id="38258-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="38258-118">配布リストのメンバーの電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="38258-118">Represents the e-mail address of the distribution list member.</span></span> <span data-ttu-id="38258-119">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="38258-119">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="38258-120">Status (MemberStatusType)</span><span class="sxs-lookup"><span data-stu-id="38258-120">Status (MemberStatusType)</span></span>](status-memberstatustype.md) <br/> |<span data-ttu-id="38258-121">配布リストのメンバーの状態に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="38258-121">Provides information about the status of a distribution list member.</span></span> <span data-ttu-id="38258-122">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="38258-122">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="38258-123">親要素</span><span class="sxs-lookup"><span data-stu-id="38258-123">Parent elements</span></span>

|<span data-ttu-id="38258-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="38258-124">**Element**</span></span>|<span data-ttu-id="38258-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="38258-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="38258-126">Members (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="38258-126">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="38258-127">配布リストのメンバーの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="38258-127">Contains a list of distribution list members.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="38258-128">注釈</span><span class="sxs-lookup"><span data-stu-id="38258-128">Remarks</span></span>

<span data-ttu-id="38258-129">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="38258-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="38258-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="38258-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="38258-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="38258-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="38258-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="38258-132">Schema Name</span></span>  <br/> |<span data-ttu-id="38258-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="38258-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="38258-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="38258-134">Validation File</span></span>  <br/> |<span data-ttu-id="38258-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="38258-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="38258-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="38258-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="38258-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="38258-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="38258-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="38258-138">See also</span></span>

- [<span data-ttu-id="38258-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="38258-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

