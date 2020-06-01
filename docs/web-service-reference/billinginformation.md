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
description: 国の情報要素は、タスクの請求情報を保持します。
ms.openlocfilehash: 6a3cd1ef402a67e896c2ed3afcca6c7c126d3e1b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462767"
---
# <a name="billinginformation"></a><span data-ttu-id="d99cf-103">BillingInformation</span><span class="sxs-lookup"><span data-stu-id="d99cf-103">BillingInformation</span></span>

<span data-ttu-id="d99cf-104">**国の情報**要素は、タスクの請求情報を保持します。</span><span class="sxs-lookup"><span data-stu-id="d99cf-104">The **BillingInformation** element holds billing information for a task.</span></span> 
  
```xml
<BillingInformation/>
```

 <span data-ttu-id="d99cf-105">**String**</span><span class="sxs-lookup"><span data-stu-id="d99cf-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d99cf-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d99cf-106">Attributes and elements</span></span>

<span data-ttu-id="d99cf-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d99cf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d99cf-108">属性</span><span class="sxs-lookup"><span data-stu-id="d99cf-108">Attributes</span></span>

<span data-ttu-id="d99cf-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d99cf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d99cf-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d99cf-110">Child elements</span></span>

<span data-ttu-id="d99cf-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d99cf-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d99cf-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d99cf-112">Parent elements</span></span>

|<span data-ttu-id="d99cf-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d99cf-113">**Element**</span></span>|<span data-ttu-id="d99cf-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d99cf-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d99cf-115">Task</span><span class="sxs-lookup"><span data-stu-id="d99cf-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="d99cf-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="d99cf-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d99cf-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d99cf-117">Text value</span></span>

<span data-ttu-id="d99cf-118">Text 値は、タスク関連の請求情報を表します。</span><span class="sxs-lookup"><span data-stu-id="d99cf-118">The text value represents task-related billing information.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d99cf-119">注釈</span><span class="sxs-lookup"><span data-stu-id="d99cf-119">Remarks</span></span>

<span data-ttu-id="d99cf-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d99cf-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d99cf-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d99cf-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d99cf-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="d99cf-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d99cf-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d99cf-123">Schema name</span></span>  <br/> |<span data-ttu-id="d99cf-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d99cf-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="d99cf-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d99cf-125">Validation file</span></span>  <br/> |<span data-ttu-id="d99cf-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d99cf-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d99cf-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d99cf-127">Can be empty</span></span>  <br/> |<span data-ttu-id="d99cf-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="d99cf-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d99cf-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="d99cf-129">See also</span></span>



- [<span data-ttu-id="d99cf-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d99cf-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

