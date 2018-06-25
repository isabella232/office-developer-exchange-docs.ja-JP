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
description: IsTeamTask 要素は、タスクが、チームが所有しているかどうかを示します。
ms.openlocfilehash: 25a60b44dbdca89d431dc202f06acb3055958a72
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832109"
---
# <a name="isteamtask"></a><span data-ttu-id="d5746-103">IsTeamTask</span><span class="sxs-lookup"><span data-stu-id="d5746-103">IsTeamTask</span></span>

<span data-ttu-id="d5746-104">**IsTeamTask**要素は、タスクが、チームが所有しているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d5746-104">The **IsTeamTask** element indicates whether the task is owned by a team.</span></span> 
  
```xml
<IsTeamTask/>
```

 <span data-ttu-id="d5746-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="d5746-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d5746-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d5746-106">Attributes and elements</span></span>

<span data-ttu-id="d5746-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d5746-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d5746-108">属性</span><span class="sxs-lookup"><span data-stu-id="d5746-108">Attributes</span></span>

<span data-ttu-id="d5746-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d5746-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d5746-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d5746-110">Child elements</span></span>

<span data-ttu-id="d5746-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d5746-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d5746-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d5746-112">Parent elements</span></span>

|<span data-ttu-id="d5746-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d5746-113">**Element**</span></span>|<span data-ttu-id="d5746-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d5746-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d5746-115">タスク</span><span class="sxs-lookup"><span data-stu-id="d5746-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="d5746-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="d5746-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d5746-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d5746-117">Text value</span></span>

<span data-ttu-id="d5746-118">テキスト値は、タスクが、チームが所有しているかどうかを示すブール値を表します。</span><span class="sxs-lookup"><span data-stu-id="d5746-118">The text value represents a Boolean value that indicates whether a task is owned by a team.</span></span> <span data-ttu-id="d5746-119">これは、プロパティは読み取り専用プロパティです。</span><span class="sxs-lookup"><span data-stu-id="d5746-119">This is a read-only property.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d5746-120">備考</span><span class="sxs-lookup"><span data-stu-id="d5746-120">Remarks</span></span>

<span data-ttu-id="d5746-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="d5746-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d5746-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="d5746-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d5746-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="d5746-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d5746-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d5746-124">Schema Name</span></span>  <br/> |<span data-ttu-id="d5746-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d5746-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="d5746-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d5746-126">Validation File</span></span>  <br/> |<span data-ttu-id="d5746-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d5746-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d5746-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d5746-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="d5746-129">False</span><span class="sxs-lookup"><span data-stu-id="d5746-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d5746-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="d5746-130">See also</span></span>



- [<span data-ttu-id="d5746-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d5746-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="d5746-132">タスクを作成します。</span><span class="sxs-lookup"><span data-stu-id="d5746-132">Creating Tasks</span></span>](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
  
[<span data-ttu-id="d5746-133">タスクを削除します。</span><span class="sxs-lookup"><span data-stu-id="d5746-133">Deleting Tasks</span></span>](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

