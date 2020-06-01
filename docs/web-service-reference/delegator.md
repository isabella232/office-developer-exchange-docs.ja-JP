---
title: Delegator
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Delegator
api_type:
- schema
ms.assetid: d359f7e8-765f-40ba-a7a0-9ce428f84523
description: 委任者要素には、タスクを割り当てた委任者の名前が含まれています。
ms.openlocfilehash: 63f97838d732c29e1e434783e7a12cf45e195e76
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457362"
---
# <a name="delegator"></a><span data-ttu-id="1f827-103">Delegator</span><span class="sxs-lookup"><span data-stu-id="1f827-103">Delegator</span></span>

<span data-ttu-id="1f827-104">**委任者**要素には、タスクを割り当てた委任者の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1f827-104">The **Delegator** element contains the name of the delegator who assigned the task.</span></span> 
  
```xml
<Delegator/>
```

<span data-ttu-id="1f827-105">**String**</span><span class="sxs-lookup"><span data-stu-id="1f827-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1f827-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1f827-106">Attributes and elements</span></span>

<span data-ttu-id="1f827-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1f827-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f827-108">属性</span><span class="sxs-lookup"><span data-stu-id="1f827-108">Attributes</span></span>

<span data-ttu-id="1f827-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1f827-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1f827-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1f827-110">Child elements</span></span>

<span data-ttu-id="1f827-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1f827-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1f827-112">親要素</span><span class="sxs-lookup"><span data-stu-id="1f827-112">Parent elements</span></span>

|<span data-ttu-id="1f827-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="1f827-113">**Element**</span></span>|<span data-ttu-id="1f827-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f827-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f827-115">Task</span><span class="sxs-lookup"><span data-stu-id="1f827-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="1f827-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="1f827-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1f827-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1f827-117">Text value</span></span>

<span data-ttu-id="1f827-118">テキスト値は、委任者の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="1f827-118">The text value represents the name of the delegator.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1f827-119">注釈</span><span class="sxs-lookup"><span data-stu-id="1f827-119">Remarks</span></span>

<span data-ttu-id="1f827-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1f827-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f827-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1f827-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f827-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="1f827-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1f827-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1f827-123">Schema name</span></span>  <br/> |<span data-ttu-id="1f827-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="1f827-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="1f827-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1f827-125">Validation file</span></span>  <br/> |<span data-ttu-id="1f827-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1f827-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="1f827-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1f827-127">Can be empty</span></span>  <br/> |<span data-ttu-id="1f827-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="1f827-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f827-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="1f827-129">See also</span></span>

- [<span data-ttu-id="1f827-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1f827-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

