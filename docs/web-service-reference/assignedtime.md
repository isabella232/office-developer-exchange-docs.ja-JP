---
title: AssignedTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AssignedTime
api_type:
- schema
ms.assetid: 37b273a4-7595-47d5-87c5-32856d7a045b
description: AssignedTime 要素は、連絡先にタスクを割り当てると時間を表します。
ms.openlocfilehash: 66d1307e143f436f94c51b293ae8189c2ce85980
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759442"
---
# <a name="assignedtime"></a><span data-ttu-id="dd3b2-103">AssignedTime</span><span class="sxs-lookup"><span data-stu-id="dd3b2-103">AssignedTime</span></span>

<span data-ttu-id="dd3b2-104">**AssignedTime**要素は、連絡先にタスクを割り当てると時間を表します。</span><span class="sxs-lookup"><span data-stu-id="dd3b2-104">The **AssignedTime** element represents the time when a task is assigned to a contact.</span></span> 
  
```xml
<AssignedTime/>
```

 <span data-ttu-id="dd3b2-105">**DateTime**</span><span class="sxs-lookup"><span data-stu-id="dd3b2-105">**DateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="dd3b2-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="dd3b2-106">Attributes and elements</span></span>

<span data-ttu-id="dd3b2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="dd3b2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="dd3b2-108">属性</span><span class="sxs-lookup"><span data-stu-id="dd3b2-108">Attributes</span></span>

<span data-ttu-id="dd3b2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="dd3b2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="dd3b2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="dd3b2-110">Child elements</span></span>

<span data-ttu-id="dd3b2-111">なし。</span><span class="sxs-lookup"><span data-stu-id="dd3b2-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="dd3b2-112">親要素</span><span class="sxs-lookup"><span data-stu-id="dd3b2-112">Parent elements</span></span>

|<span data-ttu-id="dd3b2-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="dd3b2-113">**Element**</span></span>|<span data-ttu-id="dd3b2-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="dd3b2-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="dd3b2-115">タスク</span><span class="sxs-lookup"><span data-stu-id="dd3b2-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="dd3b2-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="dd3b2-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="dd3b2-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="dd3b2-117">Text value</span></span>

<span data-ttu-id="dd3b2-118">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="dd3b2-118">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="dd3b2-119">備考</span><span class="sxs-lookup"><span data-stu-id="dd3b2-119">Remarks</span></span>

<span data-ttu-id="dd3b2-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="dd3b2-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="dd3b2-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="dd3b2-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="dd3b2-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="dd3b2-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="dd3b2-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="dd3b2-123">Schema name</span></span>  <br/> |<span data-ttu-id="dd3b2-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="dd3b2-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="dd3b2-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="dd3b2-125">Validation file</span></span>  <br/> |<span data-ttu-id="dd3b2-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="dd3b2-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="dd3b2-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="dd3b2-127">Can be empty</span></span>  <br/> |<span data-ttu-id="dd3b2-128">False</span><span class="sxs-lookup"><span data-stu-id="dd3b2-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dd3b2-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="dd3b2-129">See also</span></span>

- [<span data-ttu-id="dd3b2-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="dd3b2-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

