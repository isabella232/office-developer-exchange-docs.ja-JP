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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759270"
---
# <a name="actualwork"></a><span data-ttu-id="6fcdc-103">ActualWork</span><span class="sxs-lookup"><span data-stu-id="6fcdc-103">ActualWork</span></span>

<span data-ttu-id="6fcdc-104">**ActualWork**要素は、タスクに費やされた時間の実際の量を表します。</span><span class="sxs-lookup"><span data-stu-id="6fcdc-104">The **ActualWork** element represents the actual amount of time that is spent on a task.</span></span> 
  
```xml
<ActualWork/>
```

 <span data-ttu-id="6fcdc-105">**int**</span><span class="sxs-lookup"><span data-stu-id="6fcdc-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6fcdc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6fcdc-106">Attributes and elements</span></span>

<span data-ttu-id="6fcdc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6fcdc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6fcdc-108">属性</span><span class="sxs-lookup"><span data-stu-id="6fcdc-108">Attributes</span></span>

<span data-ttu-id="6fcdc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6fcdc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6fcdc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6fcdc-110">Child elements</span></span>

<span data-ttu-id="6fcdc-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6fcdc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6fcdc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6fcdc-112">Parent elements</span></span>

|<span data-ttu-id="6fcdc-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6fcdc-113">**Element**</span></span>|<span data-ttu-id="6fcdc-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6fcdc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6fcdc-115">タスク</span><span class="sxs-lookup"><span data-stu-id="6fcdc-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="6fcdc-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="6fcdc-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6fcdc-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6fcdc-117">Text value</span></span>

<span data-ttu-id="6fcdc-118">この要素のテキスト値は、整数を表します。</span><span class="sxs-lookup"><span data-stu-id="6fcdc-118">The text value for this element represents an integer.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6fcdc-119">備考</span><span class="sxs-lookup"><span data-stu-id="6fcdc-119">Remarks</span></span>

<span data-ttu-id="6fcdc-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="6fcdc-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6fcdc-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="6fcdc-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6fcdc-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="6fcdc-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6fcdc-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6fcdc-123">Schema name</span></span>  <br/> |<span data-ttu-id="6fcdc-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6fcdc-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="6fcdc-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6fcdc-125">Validation file</span></span>  <br/> |<span data-ttu-id="6fcdc-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6fcdc-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6fcdc-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6fcdc-127">Can be empty</span></span>  <br/> |<span data-ttu-id="6fcdc-128">False</span><span class="sxs-lookup"><span data-stu-id="6fcdc-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6fcdc-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="6fcdc-129">See also</span></span>

- [<span data-ttu-id="6fcdc-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6fcdc-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

