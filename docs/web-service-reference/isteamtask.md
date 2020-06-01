---
title: IsTeamTask
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsTeamTask
api_type:
- schema
ms.assetid: af0095da-e5bb-4138-a01c-c203f1a5a33f
description: IsTeamTask 要素は、タスクがチームに所有されているかどうかを示します。
ms.openlocfilehash: 27b5efbac028dbe7cf5858b198e3a33f9f6cdc86
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468447"
---
# <a name="isteamtask"></a><span data-ttu-id="01bb7-103">IsTeamTask</span><span class="sxs-lookup"><span data-stu-id="01bb7-103">IsTeamTask</span></span>

<span data-ttu-id="01bb7-104">**Isteamtask**要素は、タスクがチームに所有されているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="01bb7-104">The **IsTeamTask** element indicates whether the task is owned by a team.</span></span> 
  
```xml
<IsTeamTask/>
```

 <span data-ttu-id="01bb7-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="01bb7-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01bb7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="01bb7-106">Attributes and elements</span></span>

<span data-ttu-id="01bb7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="01bb7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01bb7-108">属性</span><span class="sxs-lookup"><span data-stu-id="01bb7-108">Attributes</span></span>

<span data-ttu-id="01bb7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="01bb7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="01bb7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="01bb7-110">Child elements</span></span>

<span data-ttu-id="01bb7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="01bb7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="01bb7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="01bb7-112">Parent elements</span></span>

|<span data-ttu-id="01bb7-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="01bb7-113">**Element**</span></span>|<span data-ttu-id="01bb7-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="01bb7-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01bb7-115">Task</span><span class="sxs-lookup"><span data-stu-id="01bb7-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="01bb7-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="01bb7-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="01bb7-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="01bb7-117">Text value</span></span>

<span data-ttu-id="01bb7-118">テキスト値は、タスクがチームによって所有されているかどうかを示すブール値を表します。</span><span class="sxs-lookup"><span data-stu-id="01bb7-118">The text value represents a Boolean value that indicates whether a task is owned by a team.</span></span> <span data-ttu-id="01bb7-119">これは読み取り専用のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="01bb7-119">This is a read-only property.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="01bb7-120">注釈</span><span class="sxs-lookup"><span data-stu-id="01bb7-120">Remarks</span></span>

<span data-ttu-id="01bb7-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="01bb7-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01bb7-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="01bb7-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01bb7-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="01bb7-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="01bb7-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="01bb7-124">Schema Name</span></span>  <br/> |<span data-ttu-id="01bb7-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="01bb7-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="01bb7-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="01bb7-126">Validation File</span></span>  <br/> |<span data-ttu-id="01bb7-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="01bb7-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="01bb7-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="01bb7-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="01bb7-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="01bb7-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01bb7-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="01bb7-130">See also</span></span>



- [<span data-ttu-id="01bb7-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="01bb7-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="01bb7-132">タスクの作成</span><span class="sxs-lookup"><span data-stu-id="01bb7-132">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="01bb7-133">タスクの削除</span><span class="sxs-lookup"><span data-stu-id="01bb7-133">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

