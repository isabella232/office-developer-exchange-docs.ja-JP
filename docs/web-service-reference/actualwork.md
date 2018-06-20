---
title: ActualWork
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ActualWork
api_type:
- schema
ms.assetid: aa526166-4913-4e3d-ad82-b2b5cff367be
description: ActualWork 要素は、タスクに費やされた時間の実際の量を表します。
ms.openlocfilehash: ff9cfc8ae9256203f8006e8fb4e844efccbe3c37
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759270"
---
# <a name="actualwork"></a><span data-ttu-id="cbc02-103">ActualWork</span><span class="sxs-lookup"><span data-stu-id="cbc02-103">ActualWork</span></span>

<span data-ttu-id="cbc02-104">**ActualWork**要素は、タスクに費やされた時間の実際の量を表します。</span><span class="sxs-lookup"><span data-stu-id="cbc02-104">The **ActualWork** element represents the actual amount of time that is spent on a task.</span></span> 
  
```xml
<ActualWork/>
```

 <span data-ttu-id="cbc02-105">**int**</span><span class="sxs-lookup"><span data-stu-id="cbc02-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cbc02-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cbc02-106">Attributes and elements</span></span>

<span data-ttu-id="cbc02-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cbc02-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cbc02-108">属性</span><span class="sxs-lookup"><span data-stu-id="cbc02-108">Attributes</span></span>

<span data-ttu-id="cbc02-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cbc02-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cbc02-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cbc02-110">Child elements</span></span>

<span data-ttu-id="cbc02-111">なし。</span><span class="sxs-lookup"><span data-stu-id="cbc02-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cbc02-112">親要素</span><span class="sxs-lookup"><span data-stu-id="cbc02-112">Parent elements</span></span>

|<span data-ttu-id="cbc02-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="cbc02-113">**Element**</span></span>|<span data-ttu-id="cbc02-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="cbc02-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cbc02-115">タスク</span><span class="sxs-lookup"><span data-stu-id="cbc02-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="cbc02-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="cbc02-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cbc02-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cbc02-117">Text value</span></span>

<span data-ttu-id="cbc02-118">この要素のテキスト値は、整数を表します。</span><span class="sxs-lookup"><span data-stu-id="cbc02-118">The text value for this element represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cbc02-119">備考</span><span class="sxs-lookup"><span data-stu-id="cbc02-119">Remarks</span></span>

<span data-ttu-id="cbc02-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="cbc02-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cbc02-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="cbc02-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cbc02-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="cbc02-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cbc02-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cbc02-123">Schema name</span></span>  <br/> |<span data-ttu-id="cbc02-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="cbc02-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="cbc02-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cbc02-125">Validation file</span></span>  <br/> |<span data-ttu-id="cbc02-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="cbc02-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cbc02-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cbc02-127">Can be empty</span></span>  <br/> |<span data-ttu-id="cbc02-128">False</span><span class="sxs-lookup"><span data-stu-id="cbc02-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cbc02-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="cbc02-129">See also</span></span>

- [<span data-ttu-id="cbc02-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="cbc02-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

