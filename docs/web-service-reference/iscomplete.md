---
title: IsComplete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsComplete
api_type:
- schema
ms.assetid: 5331f0a8-51b2-46e1-a07b-a2358f2d5ab0
description: 完了要素は、タスクが完了したかどうかを示します。
ms.openlocfilehash: ca1b2c189da8a56ed728e71fe0e09283cc19b414
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832006"
---
# <a name="iscomplete"></a><span data-ttu-id="3f193-103">IsComplete</span><span class="sxs-lookup"><span data-stu-id="3f193-103">IsComplete</span></span>

<span data-ttu-id="3f193-104">**完了**要素は、タスクが完了したかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3f193-104">The **IsComplete** element indicates whether the task has been completed.</span></span> 
  
```xml
<IsComplete/>
```

 <span data-ttu-id="3f193-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="3f193-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3f193-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3f193-106">Attributes and elements</span></span>

<span data-ttu-id="3f193-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3f193-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3f193-108">属性</span><span class="sxs-lookup"><span data-stu-id="3f193-108">Attributes</span></span>

<span data-ttu-id="3f193-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3f193-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3f193-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3f193-110">Child elements</span></span>

<span data-ttu-id="3f193-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3f193-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3f193-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3f193-112">Parent elements</span></span>

|<span data-ttu-id="3f193-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="3f193-113">**Element**</span></span>|<span data-ttu-id="3f193-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3f193-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3f193-115">タスク</span><span class="sxs-lookup"><span data-stu-id="3f193-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="3f193-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="3f193-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3f193-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3f193-117">Text value</span></span>

<span data-ttu-id="3f193-118">テキスト値は、タスクが完了したかどうかを示すブール値です。</span><span class="sxs-lookup"><span data-stu-id="3f193-118">The text value is a Boolean value that indicates whether the task has been completed.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3f193-119">備考</span><span class="sxs-lookup"><span data-stu-id="3f193-119">Remarks</span></span>

<span data-ttu-id="3f193-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="3f193-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3f193-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="3f193-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3f193-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="3f193-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="3f193-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3f193-123">Schema name</span></span>  <br/> |<span data-ttu-id="3f193-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="3f193-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="3f193-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3f193-125">Validation file</span></span>  <br/> |<span data-ttu-id="3f193-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="3f193-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="3f193-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3f193-127">Can be empty</span></span>  <br/> |<span data-ttu-id="3f193-128">False</span><span class="sxs-lookup"><span data-stu-id="3f193-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3f193-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="3f193-129">See also</span></span>



- [<span data-ttu-id="3f193-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3f193-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="3f193-131">タスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="3f193-131">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="3f193-132">タスクを削除します。</span><span class="sxs-lookup"><span data-stu-id="3f193-132">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

