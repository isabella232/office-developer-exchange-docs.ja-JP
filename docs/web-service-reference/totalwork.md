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
ms.openlocfilehash: 39abd8c670cd8365198d7ebb7b25b865ab8d5188
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467502"
---
# <a name="totalwork"></a><span data-ttu-id="9a794-103">TotalWork</span><span class="sxs-lookup"><span data-stu-id="9a794-103">TotalWork</span></span>

<span data-ttu-id="9a794-104">**Totalwork**要素には、タスクに関連付けられている作業量の説明が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9a794-104">The **TotalWork** element contains a description of how much work is associated with a task.</span></span> 
  
```xml
<TotalWork/>
```

 <span data-ttu-id="9a794-105">**Int**</span><span class="sxs-lookup"><span data-stu-id="9a794-105">**Int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9a794-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9a794-106">Attributes and elements</span></span>

<span data-ttu-id="9a794-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9a794-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a794-108">属性</span><span class="sxs-lookup"><span data-stu-id="9a794-108">Attributes</span></span>

<span data-ttu-id="9a794-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9a794-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a794-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9a794-110">Child elements</span></span>

<span data-ttu-id="9a794-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9a794-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9a794-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9a794-112">Parent elements</span></span>

|<span data-ttu-id="9a794-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9a794-113">**Element**</span></span>|<span data-ttu-id="9a794-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9a794-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a794-115">タスク</span><span class="sxs-lookup"><span data-stu-id="9a794-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="9a794-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="9a794-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9a794-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9a794-117">Text value</span></span>

<span data-ttu-id="9a794-118">Text 値は、タスクに関連付けられている作業時間の合計を表す整数に対応しています。</span><span class="sxs-lookup"><span data-stu-id="9a794-118">The text value corresponds to an integer that represents the total amount of work that is associated with a task.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9a794-119">注釈</span><span class="sxs-lookup"><span data-stu-id="9a794-119">Remarks</span></span>

<span data-ttu-id="9a794-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9a794-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a794-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9a794-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a794-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="9a794-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9a794-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9a794-123">Schema name</span></span>  <br/> |<span data-ttu-id="9a794-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="9a794-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="9a794-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9a794-125">Validation file</span></span>  <br/> |<span data-ttu-id="9a794-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9a794-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9a794-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9a794-127">Can be empty</span></span>  <br/> |<span data-ttu-id="9a794-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="9a794-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9a794-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="9a794-129">See also</span></span>



- [<span data-ttu-id="9a794-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9a794-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="9a794-131">タスクの作成</span><span class="sxs-lookup"><span data-stu-id="9a794-131">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="9a794-132">タスクの削除</span><span class="sxs-lookup"><span data-stu-id="9a794-132">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)
  
[<span data-ttu-id="9a794-133">タスクの更新</span><span class="sxs-lookup"><span data-stu-id="9a794-133">Updating Tasks</span></span>](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

