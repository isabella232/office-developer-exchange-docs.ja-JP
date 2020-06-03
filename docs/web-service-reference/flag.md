---
title: フラグ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b47bc74-a60d-4308-8674-5d52444a1753
description: Flag 要素は、メールボックスアイテムのフラグを指定します。
ms.openlocfilehash: 7229a26181ee9baf80be5c32c0ef99483310ccb3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466263"
---
# <a name="flag"></a><span data-ttu-id="5370d-103">フラグ</span><span class="sxs-lookup"><span data-stu-id="5370d-103">Flag</span></span>

<span data-ttu-id="5370d-104">**Flag**要素は、メールボックスアイテムのフラグを指定します。</span><span class="sxs-lookup"><span data-stu-id="5370d-104">The **Flag** element specifies a flag on a mailbox item.</span></span> 
  
```XML
<Flag>
    <FlagStatus/>
    <StartDate/>
    <DueDate/>
    <CompleteDate/>
</Flag>
```

 <span data-ttu-id="5370d-105">**FlagType**</span><span class="sxs-lookup"><span data-stu-id="5370d-105">**FlagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5370d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5370d-106">Attributes and elements</span></span>

<span data-ttu-id="5370d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5370d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5370d-108">属性</span><span class="sxs-lookup"><span data-stu-id="5370d-108">Attributes</span></span>

<span data-ttu-id="5370d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5370d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5370d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5370d-110">Child elements</span></span>

|<span data-ttu-id="5370d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="5370d-111">**Element**</span></span>|<span data-ttu-id="5370d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5370d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5370d-113">FlagStatus</span><span class="sxs-lookup"><span data-stu-id="5370d-113">FlagStatus</span></span>](flagstatus.md) <br/> |<span data-ttu-id="5370d-114">現在のフォルダー内のアイテムの集計フラグの状態を含みます。</span><span class="sxs-lookup"><span data-stu-id="5370d-114">Contains the aggregated flag status for items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="5370d-115">StartDate</span><span class="sxs-lookup"><span data-stu-id="5370d-115">StartDate</span></span>](startdate.md) <br/> |<span data-ttu-id="5370d-116">アイテムの開始日を表します。</span><span class="sxs-lookup"><span data-stu-id="5370d-116">Represents the start date of an item.</span></span>  <br/> |
|[<span data-ttu-id="5370d-117">DueDate</span><span class="sxs-lookup"><span data-stu-id="5370d-117">DueDate</span></span>](duedate.md) <br/> |<span data-ttu-id="5370d-118">アイテムの期限の日付を表します。</span><span class="sxs-lookup"><span data-stu-id="5370d-118">Represents the date when an item is due.</span></span>  <br/> |
|[<span data-ttu-id="5370d-119">CompleteDate</span><span class="sxs-lookup"><span data-stu-id="5370d-119">CompleteDate</span></span>](completedate.md) <br/> |<span data-ttu-id="5370d-120">アイテムが完了した日付を表します。</span><span class="sxs-lookup"><span data-stu-id="5370d-120">Represents the date on which an item was completed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5370d-121">親要素</span><span class="sxs-lookup"><span data-stu-id="5370d-121">Parent elements</span></span>

|<span data-ttu-id="5370d-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="5370d-122">**Element**</span></span>|<span data-ttu-id="5370d-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="5370d-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5370d-124">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="5370d-124">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="5370d-125">単一の会話に適用される1つのアクションが含まれます。</span><span class="sxs-lookup"><span data-stu-id="5370d-125">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="5370d-126">Item</span><span class="sxs-lookup"><span data-stu-id="5370d-126">Item</span></span>](item.md) <br/> |<span data-ttu-id="5370d-127">Exchange ストア内の汎用アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="5370d-127">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5370d-128">注釈</span><span class="sxs-lookup"><span data-stu-id="5370d-128">Remarks</span></span>

<span data-ttu-id="5370d-129">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5370d-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5370d-130">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5370d-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5370d-131">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5370d-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5370d-132">Namespace</span><span class="sxs-lookup"><span data-stu-id="5370d-132">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5370d-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5370d-133">Schema Name</span></span>  <br/> |<span data-ttu-id="5370d-134">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="5370d-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="5370d-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5370d-135">Validation File</span></span>  <br/> |<span data-ttu-id="5370d-136">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="5370d-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="5370d-137">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5370d-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="5370d-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="5370d-138">See also</span></span>



- [<span data-ttu-id="5370d-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5370d-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

