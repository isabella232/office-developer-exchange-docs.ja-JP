---
title: 'Assignees '
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 20ef18c2-daa0-4f65-a515-e84e9993a77f
description: タスク実施者の要素は、タスクの割り当て先ユーザーを指定します。
ms.openlocfilehash: 5fc301cd77268213e95fd33a2a2f36dbe218b512
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759443"
---
# <a name="assignees"></a><span data-ttu-id="f510d-103">Assignees </span><span class="sxs-lookup"><span data-stu-id="f510d-103">Assignees</span></span>

<span data-ttu-id="f510d-104">**タスク実施者**の要素は、タスクの割り当て先ユーザーを指定します。</span><span class="sxs-lookup"><span data-stu-id="f510d-104">The **Assignees** element specifies the people to whom a task is assigned.</span></span> 
  
```XML
<Assignees>
    <Name></Name>
    <UserID></UserID>
</Assignees>
```

 <span data-ttu-id="f510d-105">**EmailUserType**</span><span class="sxs-lookup"><span data-stu-id="f510d-105">**EmailUserType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f510d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f510d-106">Attributes and elements</span></span>

<span data-ttu-id="f510d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f510d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f510d-108">属性</span><span class="sxs-lookup"><span data-stu-id="f510d-108">Attributes</span></span>

<span data-ttu-id="f510d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f510d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f510d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f510d-110">Child elements</span></span>

|<span data-ttu-id="f510d-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="f510d-111">**Element**</span></span>|<span data-ttu-id="f510d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="f510d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f510d-113">名 (EmailAddress)</span><span class="sxs-lookup"><span data-stu-id="f510d-113">Name (EmailAddress)</span></span>](name-emailaddress.md) <br/> |<span data-ttu-id="f510d-114">メールボックス ユーザーの表示名を表します。</span><span class="sxs-lookup"><span data-stu-id="f510d-114">Represents the display name of the mailbox user.</span></span>  <br/> |
|[<span data-ttu-id="f510d-115">ユーザー Id (文字列)</span><span class="sxs-lookup"><span data-stu-id="f510d-115">UserId (string)</span></span>](userid-string.md) <br/> |<span data-ttu-id="f510d-116">メール ユーザーのユーザー識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="f510d-116">Specifies the user identifier of an email user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f510d-117">親要素</span><span class="sxs-lookup"><span data-stu-id="f510d-117">Parent elements</span></span>

|<span data-ttu-id="f510d-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="f510d-118">**Element**</span></span>|<span data-ttu-id="f510d-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="f510d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f510d-120">TaskSuggestion</span><span class="sxs-lookup"><span data-stu-id="f510d-120">TaskSuggestion</span></span>](tasksuggestion.md) <br/> |<span data-ttu-id="f510d-121">提案済みのタスクを指定します。</span><span class="sxs-lookup"><span data-stu-id="f510d-121">Specifies a proposed task.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="f510d-122">備考</span><span class="sxs-lookup"><span data-stu-id="f510d-122">Remarks</span></span>

<span data-ttu-id="f510d-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f510d-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f510d-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f510d-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f510d-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="f510d-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f510d-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="f510d-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f510d-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f510d-127">Schema Name</span></span>  <br/> |<span data-ttu-id="f510d-128">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="f510d-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="f510d-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f510d-129">Validation File</span></span>  <br/> |<span data-ttu-id="f510d-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="f510d-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f510d-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f510d-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f510d-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="f510d-132">See also</span></span>

- [<span data-ttu-id="f510d-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f510d-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

