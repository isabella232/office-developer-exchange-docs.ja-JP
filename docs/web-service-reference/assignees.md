---
title: 実施
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 20ef18c2-daa0-4f65-a515-e84e9993a77f
description: '[タスク] 要素は、タスクを割り当てるユーザーを指定します。'
ms.openlocfilehash: 3e98273e859dbe2128b0ad3b4df42c8016fd3bc5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464715"
---
# <a name="assignees"></a><span data-ttu-id="3619a-103">実施</span><span class="sxs-lookup"><span data-stu-id="3619a-103">Assignees</span></span>

<span data-ttu-id="3619a-104">[タスク **] 要素は、タスク**を割り当てるユーザーを指定します。</span><span class="sxs-lookup"><span data-stu-id="3619a-104">The **Assignees** element specifies the people to whom a task is assigned.</span></span> 
  
```XML
<Assignees>
    <Name></Name>
    <UserID></UserID>
</Assignees>
```

 <span data-ttu-id="3619a-105">**EmailUserType**</span><span class="sxs-lookup"><span data-stu-id="3619a-105">**EmailUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3619a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3619a-106">Attributes and elements</span></span>

<span data-ttu-id="3619a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3619a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3619a-108">属性</span><span class="sxs-lookup"><span data-stu-id="3619a-108">Attributes</span></span>

<span data-ttu-id="3619a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3619a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3619a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3619a-110">Child elements</span></span>

|<span data-ttu-id="3619a-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="3619a-111">**Element**</span></span>|<span data-ttu-id="3619a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3619a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3619a-113">Name (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="3619a-113">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="3619a-114">メールボックスユーザーの表示名を表します。</span><span class="sxs-lookup"><span data-stu-id="3619a-114">Represents the display name of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="3619a-115">UserId (文字列)</span><span class="sxs-lookup"><span data-stu-id="3619a-115">UserId (string)</span></span>](userid-string.md) <br/> |<span data-ttu-id="3619a-116">電子メールユーザーのユーザー識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="3619a-116">Specifies the user identifier of an email user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3619a-117">親要素</span><span class="sxs-lookup"><span data-stu-id="3619a-117">Parent elements</span></span>

|<span data-ttu-id="3619a-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="3619a-118">**Element**</span></span>|<span data-ttu-id="3619a-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="3619a-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3619a-120">TaskSuggestion</span><span class="sxs-lookup"><span data-stu-id="3619a-120">TaskSuggestion</span></span>](tasksuggestion.md) <br/> |<span data-ttu-id="3619a-121">提案されたタスクを指定します。</span><span class="sxs-lookup"><span data-stu-id="3619a-121">Specifies a proposed task.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3619a-122">注釈</span><span class="sxs-lookup"><span data-stu-id="3619a-122">Remarks</span></span>

<span data-ttu-id="3619a-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3619a-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3619a-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3619a-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3619a-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3619a-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3619a-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="3619a-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3619a-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3619a-127">Schema Name</span></span>  <br/> |<span data-ttu-id="3619a-128">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="3619a-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="3619a-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3619a-129">Validation File</span></span>  <br/> |<span data-ttu-id="3619a-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="3619a-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="3619a-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3619a-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3619a-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="3619a-132">See also</span></span>

- [<span data-ttu-id="3619a-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3619a-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

