---
title: BillingInformation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- BillingInformation
api_type:
- schema
ms.assetid: 35aec4d1-5264-4b25-8b8f-cdee886da109
description: BillingInformation 要素は、タスクの課金情報を保持します。
ms.openlocfilehash: 88c79851eda4f22b3f89084f90ccb9847c3e2daf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759496"
---
# <a name="billinginformation"></a><span data-ttu-id="0bffa-103">BillingInformation</span><span class="sxs-lookup"><span data-stu-id="0bffa-103">BillingInformation</span></span>

<span data-ttu-id="0bffa-104">**BillingInformation**要素は、タスクの課金情報を保持します。</span><span class="sxs-lookup"><span data-stu-id="0bffa-104">The **BillingInformation** element holds billing information for a task.</span></span> 
  
```xml
<BillingInformation/>
```

 <span data-ttu-id="0bffa-105">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="0bffa-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0bffa-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0bffa-106">Attributes and elements</span></span>

<span data-ttu-id="0bffa-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0bffa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0bffa-108">属性</span><span class="sxs-lookup"><span data-stu-id="0bffa-108">Attributes</span></span>

<span data-ttu-id="0bffa-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0bffa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0bffa-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0bffa-110">Child elements</span></span>

<span data-ttu-id="0bffa-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0bffa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0bffa-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0bffa-112">Parent elements</span></span>

|<span data-ttu-id="0bffa-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="0bffa-113">**Element**</span></span>|<span data-ttu-id="0bffa-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="0bffa-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0bffa-115">タスク</span><span class="sxs-lookup"><span data-stu-id="0bffa-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="0bffa-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="0bffa-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0bffa-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0bffa-117">Text value</span></span>

<span data-ttu-id="0bffa-118">テキスト値は、タスク関連の課金情報を表します。</span><span class="sxs-lookup"><span data-stu-id="0bffa-118">The text value represents task-related billing information.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0bffa-119">備考</span><span class="sxs-lookup"><span data-stu-id="0bffa-119">Remarks</span></span>

<span data-ttu-id="0bffa-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="0bffa-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0bffa-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="0bffa-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0bffa-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="0bffa-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0bffa-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0bffa-123">Schema name</span></span>  <br/> |<span data-ttu-id="0bffa-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="0bffa-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="0bffa-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0bffa-125">Validation file</span></span>  <br/> |<span data-ttu-id="0bffa-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="0bffa-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0bffa-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0bffa-127">Can be empty</span></span>  <br/> |<span data-ttu-id="0bffa-128">False</span><span class="sxs-lookup"><span data-stu-id="0bffa-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0bffa-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="0bffa-129">See also</span></span>



- [<span data-ttu-id="0bffa-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0bffa-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

