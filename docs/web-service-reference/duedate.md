---
title: DueDate
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DueDate
api_type:
- schema
ms.assetid: dd9b6c43-a512-4b3b-a071-4abde02ed55f
description: DueDate 要素は、アイテムの期限の日付を表します。
ms.openlocfilehash: b88bb5c64ee48e02b1600c6865ce650e7bcdaa3b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463560"
---
# <a name="duedate"></a><span data-ttu-id="7ec30-103">DueDate</span><span class="sxs-lookup"><span data-stu-id="7ec30-103">DueDate</span></span>

<span data-ttu-id="7ec30-104">**DueDate**要素は、アイテムの期限の日付を表します。</span><span class="sxs-lookup"><span data-stu-id="7ec30-104">The **DueDate** element represents the date an item is due.</span></span> 
  
```xml
<DueDate/>
```

 <span data-ttu-id="7ec30-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="7ec30-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7ec30-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7ec30-106">Attributes and elements</span></span>

<span data-ttu-id="7ec30-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7ec30-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ec30-108">属性</span><span class="sxs-lookup"><span data-stu-id="7ec30-108">Attributes</span></span>

<span data-ttu-id="7ec30-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7ec30-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7ec30-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7ec30-110">Child elements</span></span>

<span data-ttu-id="7ec30-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7ec30-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7ec30-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7ec30-112">Parent elements</span></span>

|<span data-ttu-id="7ec30-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="7ec30-113">**Element**</span></span>|<span data-ttu-id="7ec30-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="7ec30-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ec30-115">タスク</span><span class="sxs-lookup"><span data-stu-id="7ec30-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="7ec30-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="7ec30-116">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7ec30-117">Flag</span><span class="sxs-lookup"><span data-stu-id="7ec30-117">Flag</span></span>](flag.md) <br/> |<span data-ttu-id="7ec30-118">メールボックスアイテムのフラグを指定します。</span><span class="sxs-lookup"><span data-stu-id="7ec30-118">Specifies a flag on a mailbox item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7ec30-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7ec30-119">Text value</span></span>

<span data-ttu-id="7ec30-120">この要素を使用する場合は、日付と時刻を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="7ec30-120">A text value that represents the date and time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7ec30-121">注釈</span><span class="sxs-lookup"><span data-stu-id="7ec30-121">Remarks</span></span>

<span data-ttu-id="7ec30-122">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7ec30-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ec30-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7ec30-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ec30-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="7ec30-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7ec30-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7ec30-125">Schema name</span></span>  <br/> |<span data-ttu-id="7ec30-126">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7ec30-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="7ec30-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7ec30-127">Validation file</span></span>  <br/> |<span data-ttu-id="7ec30-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7ec30-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7ec30-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7ec30-129">Can be empty</span></span>  <br/> |<span data-ttu-id="7ec30-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="7ec30-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ec30-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="7ec30-131">See also</span></span>

- [<span data-ttu-id="7ec30-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7ec30-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

