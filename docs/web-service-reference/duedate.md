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
description: DueDate 要素は、項目が期限の日付を表します。
ms.openlocfilehash: b24891972f240bc6ee5d0fe868445b96abdc089a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760169"
---
# <a name="duedate"></a><span data-ttu-id="af4cb-103">DueDate</span><span class="sxs-lookup"><span data-stu-id="af4cb-103">DueDate</span></span>

<span data-ttu-id="af4cb-104">**DueDate**要素は、項目が期限の日付を表します。</span><span class="sxs-lookup"><span data-stu-id="af4cb-104">The **DueDate** element represents the date an item is due.</span></span> 
  
```xml
<DueDate/>
```

 <span data-ttu-id="af4cb-105">**dateTime**</span><span class="sxs-lookup"><span data-stu-id="af4cb-105">**dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="af4cb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="af4cb-106">Attributes and elements</span></span>

<span data-ttu-id="af4cb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="af4cb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="af4cb-108">属性</span><span class="sxs-lookup"><span data-stu-id="af4cb-108">Attributes</span></span>

<span data-ttu-id="af4cb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="af4cb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="af4cb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="af4cb-110">Child elements</span></span>

<span data-ttu-id="af4cb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="af4cb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="af4cb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="af4cb-112">Parent elements</span></span>

|<span data-ttu-id="af4cb-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="af4cb-113">**Element**</span></span>|<span data-ttu-id="af4cb-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="af4cb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="af4cb-115">タスク</span><span class="sxs-lookup"><span data-stu-id="af4cb-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="af4cb-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="af4cb-116">Represents a task in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="af4cb-117">Flag</span><span class="sxs-lookup"><span data-stu-id="af4cb-117">Flag</span></span>](flag.md) <br/> |<span data-ttu-id="af4cb-118">メールボックス アイテムにフラグを指定します。</span><span class="sxs-lookup"><span data-stu-id="af4cb-118">Specifies a flag on a mailbox item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="af4cb-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="af4cb-119">Text value</span></span>

<span data-ttu-id="af4cb-120">日付と時刻を表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="af4cb-120">A text value that represents the date and time is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="af4cb-121">備考</span><span class="sxs-lookup"><span data-stu-id="af4cb-121">Remarks</span></span>

<span data-ttu-id="af4cb-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="af4cb-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="af4cb-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="af4cb-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="af4cb-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="af4cb-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="af4cb-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="af4cb-125">Schema name</span></span>  <br/> |<span data-ttu-id="af4cb-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="af4cb-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="af4cb-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="af4cb-127">Validation file</span></span>  <br/> |<span data-ttu-id="af4cb-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="af4cb-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="af4cb-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="af4cb-129">Can be empty</span></span>  <br/> |<span data-ttu-id="af4cb-130">False</span><span class="sxs-lookup"><span data-stu-id="af4cb-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="af4cb-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="af4cb-131">See also</span></span>

- [<span data-ttu-id="af4cb-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="af4cb-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

