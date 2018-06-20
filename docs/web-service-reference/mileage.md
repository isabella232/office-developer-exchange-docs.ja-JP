---
title: Mileage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Mileage
api_type:
- schema
ms.assetid: 461ba447-1b04-4115-9919-dc378fd3bf24
description: マイレージ要素は、タスク、または連絡先アイテムの経費情報を表します。
ms.openlocfilehash: ee0625f281473622d302ab6ace7a02207c8f80e7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832495"
---
# <a name="mileage"></a><span data-ttu-id="7ccea-103">Mileage</span><span class="sxs-lookup"><span data-stu-id="7ccea-103">Mileage</span></span>

<span data-ttu-id="7ccea-104">**マイレージ**要素は、タスク、または連絡先アイテムの経費情報を表します。</span><span class="sxs-lookup"><span data-stu-id="7ccea-104">The **Mileage** element represents mileage for a task or contact item.</span></span> 
  
```xml
<Mileage/>
```

 <span data-ttu-id="7ccea-105">**string**</span><span class="sxs-lookup"><span data-stu-id="7ccea-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7ccea-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7ccea-106">Attributes and elements</span></span>

<span data-ttu-id="7ccea-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7ccea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ccea-108">属性</span><span class="sxs-lookup"><span data-stu-id="7ccea-108">Attributes</span></span>

<span data-ttu-id="7ccea-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7ccea-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7ccea-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7ccea-110">Child elements</span></span>

<span data-ttu-id="7ccea-111">なし。</span><span class="sxs-lookup"><span data-stu-id="7ccea-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7ccea-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7ccea-112">Parent elements</span></span>

|<span data-ttu-id="7ccea-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="7ccea-113">**Element**</span></span>|<span data-ttu-id="7ccea-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="7ccea-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ccea-115">Contact</span><span class="sxs-lookup"><span data-stu-id="7ccea-115">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="7ccea-116">Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="7ccea-116">Represents a contact item in the Exchange store.</span></span>  <br/> |
|[<span data-ttu-id="7ccea-117">タスク</span><span class="sxs-lookup"><span data-stu-id="7ccea-117">Task</span></span>](task.md) <br/> |<span data-ttu-id="7ccea-118">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="7ccea-118">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7ccea-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7ccea-119">Text value</span></span>

<span data-ttu-id="7ccea-120">テキスト値は、この要素が使用される場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="7ccea-120">A text value is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7ccea-121">備考</span><span class="sxs-lookup"><span data-stu-id="7ccea-121">Remarks</span></span>

<span data-ttu-id="7ccea-122">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="7ccea-122">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ccea-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="7ccea-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ccea-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="7ccea-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7ccea-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7ccea-125">Schema name</span></span>  <br/> |<span data-ttu-id="7ccea-126">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7ccea-126">Types schema</span></span>  <br/> |
|<span data-ttu-id="7ccea-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7ccea-127">Validation file</span></span>  <br/> |<span data-ttu-id="7ccea-128">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7ccea-128">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7ccea-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7ccea-129">Can be empty</span></span>  <br/> |<span data-ttu-id="7ccea-130">False</span><span class="sxs-lookup"><span data-stu-id="7ccea-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ccea-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="7ccea-131">See also</span></span>



- [<span data-ttu-id="7ccea-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7ccea-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

