---
title: フラグ
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7b47bc74-a60d-4308-8674-5d52444a1753
description: フラグの要素は、メールボックスのアイテムにフラグを指定します。
ms.openlocfilehash: f30f435e8f064d7165ae52de737bbd75b0546206
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760549"
---
# <a name="flag"></a><span data-ttu-id="60518-103">フラグ</span><span class="sxs-lookup"><span data-stu-id="60518-103">Flag</span></span>

<span data-ttu-id="60518-104">**フラグ**の要素は、メールボックスのアイテムにフラグを指定します。</span><span class="sxs-lookup"><span data-stu-id="60518-104">The **Flag** element specifies a flag on a mailbox item.</span></span> 
  
```XML
<Flag>
    <FlagStatus/>
    <StartDate/>
    <DueDate/>
    <CompleteDate/>
</Flag>
```

 <span data-ttu-id="60518-105">**FlagType**</span><span class="sxs-lookup"><span data-stu-id="60518-105">**FlagType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="60518-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="60518-106">Attributes and elements</span></span>

<span data-ttu-id="60518-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="60518-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="60518-108">属性</span><span class="sxs-lookup"><span data-stu-id="60518-108">Attributes</span></span>

<span data-ttu-id="60518-109">なし。</span><span class="sxs-lookup"><span data-stu-id="60518-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="60518-110">子要素</span><span class="sxs-lookup"><span data-stu-id="60518-110">Child elements</span></span>

|<span data-ttu-id="60518-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="60518-111">**Element**</span></span>|<span data-ttu-id="60518-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="60518-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60518-113">フラグ</span><span class="sxs-lookup"><span data-stu-id="60518-113">FlagStatus</span></span>](flagstatus.md) <br/> |<span data-ttu-id="60518-114">現在のフォルダー内のアイテムの集計のフラグの状態が含まれています。</span><span class="sxs-lookup"><span data-stu-id="60518-114">Contains the aggregated flag status for items in the current folder.</span></span>  <br/> |
|[<span data-ttu-id="60518-115">開始日</span><span class="sxs-lookup"><span data-stu-id="60518-115">StartDate</span></span>](startdate.md) <br/> |<span data-ttu-id="60518-116">アイテムの開始日を表します。</span><span class="sxs-lookup"><span data-stu-id="60518-116">Represents the start date of an item.</span></span>  <br/> |
|[<span data-ttu-id="60518-117">DueDate</span><span class="sxs-lookup"><span data-stu-id="60518-117">DueDate</span></span>](duedate.md) <br/> |<span data-ttu-id="60518-118">アイテムの期限の日付を表します。</span><span class="sxs-lookup"><span data-stu-id="60518-118">Represents the date when an item is due.</span></span>  <br/> |
|[<span data-ttu-id="60518-119">CompleteDate</span><span class="sxs-lookup"><span data-stu-id="60518-119">CompleteDate</span></span>](completedate.md) <br/> |<span data-ttu-id="60518-120">項目が完了された日付を表します。</span><span class="sxs-lookup"><span data-stu-id="60518-120">Represents the date on which an item was completed.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="60518-121">親要素</span><span class="sxs-lookup"><span data-stu-id="60518-121">Parent elements</span></span>

|<span data-ttu-id="60518-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="60518-122">**Element**</span></span>|<span data-ttu-id="60518-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="60518-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="60518-124">ConversationAction</span><span class="sxs-lookup"><span data-stu-id="60518-124">ConversationAction</span></span>](conversationaction.md) <br/> |<span data-ttu-id="60518-125">1 つのテーマを適用する 1 つのアクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="60518-125">Contains a single action to be applied to a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="60518-126">アイテム</span><span class="sxs-lookup"><span data-stu-id="60518-126">Item</span></span>](item.md) <br/> |<span data-ttu-id="60518-127">Exchange ストア内の一般的な項目を表します。</span><span class="sxs-lookup"><span data-stu-id="60518-127">Represents a generic item in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="60518-128">備考</span><span class="sxs-lookup"><span data-stu-id="60518-128">Remarks</span></span>

<span data-ttu-id="60518-129">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="60518-129">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="60518-130">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="60518-130">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="60518-131">要素情報</span><span class="sxs-lookup"><span data-stu-id="60518-131">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="60518-132">名前空間</span><span class="sxs-lookup"><span data-stu-id="60518-132">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="60518-133">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="60518-133">Schema Name</span></span>  <br/> |<span data-ttu-id="60518-134">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="60518-134">Type schema</span></span>  <br/> |
|<span data-ttu-id="60518-135">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="60518-135">Validation File</span></span>  <br/> |<span data-ttu-id="60518-136">types.xsd</span><span class="sxs-lookup"><span data-stu-id="60518-136">types.xsd</span></span>  <br/> |
|<span data-ttu-id="60518-137">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="60518-137">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="60518-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="60518-138">See also</span></span>



- [<span data-ttu-id="60518-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="60518-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

