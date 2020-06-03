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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457306"
---
# <a name="member"></a><span data-ttu-id="9f983-103">Member</span><span class="sxs-lookup"><span data-stu-id="9f983-103">Member</span></span>

<span data-ttu-id="9f983-104">**Member**要素は、配布リストのメンバーを表します。</span><span class="sxs-lookup"><span data-stu-id="9f983-104">The **Member** element represents a member of a distribution list.</span></span> 
  
```xml
<Member Key="">
   <Mailbox/>
   <Status/>
</Member>
```

<span data-ttu-id="9f983-105">**MemberType**</span><span class="sxs-lookup"><span data-stu-id="9f983-105">**MemberType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="9f983-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9f983-106">Attributes and elements</span></span>

<span data-ttu-id="9f983-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9f983-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9f983-108">属性</span><span class="sxs-lookup"><span data-stu-id="9f983-108">Attributes</span></span>

|<span data-ttu-id="9f983-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="9f983-109">**Attribute**</span></span>|<span data-ttu-id="9f983-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="9f983-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9f983-111">キー</span><span class="sxs-lookup"><span data-stu-id="9f983-111">Key</span></span>  <br/> |<span data-ttu-id="9f983-112">配布リストのメンバーの一意の識別子を提供します。</span><span class="sxs-lookup"><span data-stu-id="9f983-112">Provides a unique identifier for the distribution list member.</span></span> <span data-ttu-id="9f983-113">この属性は省略可能です。</span><span class="sxs-lookup"><span data-stu-id="9f983-113">This attribute is optional.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9f983-114">子要素</span><span class="sxs-lookup"><span data-stu-id="9f983-114">Child elements</span></span>

|<span data-ttu-id="9f983-115">**Element**</span><span class="sxs-lookup"><span data-stu-id="9f983-115">**Element**</span></span>|<span data-ttu-id="9f983-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="9f983-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f983-117">メールボックス</span><span class="sxs-lookup"><span data-stu-id="9f983-117">Mailbox</span></span>](mailbox.md) <br/> |<span data-ttu-id="9f983-118">配布リストのメンバーの電子メールアドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="9f983-118">Represents the e-mail address of the distribution list member.</span></span> <span data-ttu-id="9f983-119">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="9f983-119">This element is optional.</span></span>  <br/> |
|[<span data-ttu-id="9f983-120">Status (MemberStatusType)</span><span class="sxs-lookup"><span data-stu-id="9f983-120">Status (MemberStatusType)</span></span>](status-memberstatustype.md) <br/> |<span data-ttu-id="9f983-121">配布リストのメンバーの状態に関する情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="9f983-121">Provides information about the status of a distribution list member.</span></span> <span data-ttu-id="9f983-122">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="9f983-122">This element is optional.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9f983-123">親要素</span><span class="sxs-lookup"><span data-stu-id="9f983-123">Parent elements</span></span>

|<span data-ttu-id="9f983-124">**要素**</span><span class="sxs-lookup"><span data-stu-id="9f983-124">**Element**</span></span>|<span data-ttu-id="9f983-125">**説明**</span><span class="sxs-lookup"><span data-stu-id="9f983-125">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9f983-126">Members (MemberListType)</span><span class="sxs-lookup"><span data-stu-id="9f983-126">Members (MemberListType)</span></span>](members-memberlisttype.md) <br/> |<span data-ttu-id="9f983-127">配布リストのメンバーの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9f983-127">Contains a list of distribution list members.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9f983-128">注釈</span><span class="sxs-lookup"><span data-stu-id="9f983-128">Remarks</span></span>

<span data-ttu-id="9f983-129">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9f983-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9f983-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9f983-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9f983-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="9f983-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9f983-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9f983-132">Schema Name</span></span>  <br/> |<span data-ttu-id="9f983-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9f983-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="9f983-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9f983-134">Validation File</span></span>  <br/> |<span data-ttu-id="9f983-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9f983-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9f983-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9f983-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="9f983-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="9f983-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9f983-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="9f983-138">See also</span></span>

- [<span data-ttu-id="9f983-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9f983-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

