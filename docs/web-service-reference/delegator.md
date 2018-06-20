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
description: 代理人の要素には、タスクを割り当てられている代理人の名前が含まれています。
ms.openlocfilehash: 00d9c24e71037c10d7093883491242e665305295
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759955"
---
# <a name="delegator"></a><span data-ttu-id="4a8a5-103">Delegator</span><span class="sxs-lookup"><span data-stu-id="4a8a5-103">Delegator</span></span>

<span data-ttu-id="4a8a5-104">**代理人**の要素には、タスクを割り当てられている代理人の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4a8a5-104">The **Delegator** element contains the name of the delegator who assigned the task.</span></span> 
  
```xml
<Delegator/>
```

<span data-ttu-id="4a8a5-105">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="4a8a5-105">**String**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="4a8a5-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4a8a5-106">Attributes and elements</span></span>

<span data-ttu-id="4a8a5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4a8a5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a8a5-108">属性</span><span class="sxs-lookup"><span data-stu-id="4a8a5-108">Attributes</span></span>

<span data-ttu-id="4a8a5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4a8a5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4a8a5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4a8a5-110">Child elements</span></span>

<span data-ttu-id="4a8a5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4a8a5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4a8a5-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4a8a5-112">Parent elements</span></span>

|<span data-ttu-id="4a8a5-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4a8a5-113">**Element**</span></span>|<span data-ttu-id="4a8a5-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4a8a5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a8a5-115">タスク</span><span class="sxs-lookup"><span data-stu-id="4a8a5-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="4a8a5-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="4a8a5-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4a8a5-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4a8a5-117">Text value</span></span>

<span data-ttu-id="4a8a5-118">テキスト値は、代理人の名前を表します。</span><span class="sxs-lookup"><span data-stu-id="4a8a5-118">The text value represents the name of the delegator.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4a8a5-119">備考</span><span class="sxs-lookup"><span data-stu-id="4a8a5-119">Remarks</span></span>

<span data-ttu-id="4a8a5-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="4a8a5-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a8a5-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="4a8a5-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a8a5-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="4a8a5-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4a8a5-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4a8a5-123">Schema name</span></span>  <br/> |<span data-ttu-id="4a8a5-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4a8a5-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="4a8a5-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4a8a5-125">Validation file</span></span>  <br/> |<span data-ttu-id="4a8a5-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4a8a5-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4a8a5-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4a8a5-127">Can be empty</span></span>  <br/> |<span data-ttu-id="4a8a5-128">False</span><span class="sxs-lookup"><span data-stu-id="4a8a5-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a8a5-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="4a8a5-129">See also</span></span>

- [<span data-ttu-id="4a8a5-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4a8a5-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

