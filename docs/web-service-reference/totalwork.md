---
title: TotalWork
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TotalWork
api_type:
- schema
ms.assetid: 1348ffab-bd19-48fc-90dc-fd35e7031700
description: TotalWork 要素には、タスクに関連付けられている作業量の説明が含まれています。
ms.openlocfilehash: a8a9b8cb2325bf7f43d833fcb4cd111254b0babb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839735"
---
# <a name="totalwork"></a><span data-ttu-id="2f7b8-103">TotalWork</span><span class="sxs-lookup"><span data-stu-id="2f7b8-103">TotalWork</span></span>

<span data-ttu-id="2f7b8-104">**TotalWork**要素には、タスクに関連付けられている作業量の説明が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2f7b8-104">The **TotalWork** element contains a description of how much work is associated with a task.</span></span> 
  
```xml
<TotalWork/>
```

 <span data-ttu-id="2f7b8-105">**Int**</span><span class="sxs-lookup"><span data-stu-id="2f7b8-105">**Int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2f7b8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2f7b8-106">Attributes and elements</span></span>

<span data-ttu-id="2f7b8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2f7b8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2f7b8-108">属性</span><span class="sxs-lookup"><span data-stu-id="2f7b8-108">Attributes</span></span>

<span data-ttu-id="2f7b8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2f7b8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2f7b8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2f7b8-110">Child elements</span></span>

<span data-ttu-id="2f7b8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2f7b8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2f7b8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2f7b8-112">Parent elements</span></span>

|<span data-ttu-id="2f7b8-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="2f7b8-113">**Element**</span></span>|<span data-ttu-id="2f7b8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="2f7b8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2f7b8-115">タスク</span><span class="sxs-lookup"><span data-stu-id="2f7b8-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="2f7b8-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="2f7b8-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2f7b8-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2f7b8-117">Text value</span></span>

<span data-ttu-id="2f7b8-118">テキスト値は、タスクに関連付けられている作業量の合計を表す整数に対応します。</span><span class="sxs-lookup"><span data-stu-id="2f7b8-118">The text value corresponds to an integer that represents the total amount of work that is associated with a task.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2f7b8-119">備考</span><span class="sxs-lookup"><span data-stu-id="2f7b8-119">Remarks</span></span>

<span data-ttu-id="2f7b8-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="2f7b8-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2f7b8-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="2f7b8-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2f7b8-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="2f7b8-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2f7b8-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2f7b8-123">Schema name</span></span>  <br/> |<span data-ttu-id="2f7b8-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="2f7b8-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="2f7b8-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2f7b8-125">Validation file</span></span>  <br/> |<span data-ttu-id="2f7b8-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2f7b8-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2f7b8-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2f7b8-127">Can be empty</span></span>  <br/> |<span data-ttu-id="2f7b8-128">False</span><span class="sxs-lookup"><span data-stu-id="2f7b8-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2f7b8-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="2f7b8-129">See also</span></span>



- [<span data-ttu-id="2f7b8-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2f7b8-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="2f7b8-131">タスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="2f7b8-131">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="2f7b8-132">タスクを削除します。</span><span class="sxs-lookup"><span data-stu-id="2f7b8-132">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)
  
[<span data-ttu-id="2f7b8-133">タスクの更新</span><span class="sxs-lookup"><span data-stu-id="2f7b8-133">Updating Tasks</span></span>](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

