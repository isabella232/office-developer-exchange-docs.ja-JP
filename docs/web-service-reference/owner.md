---
title: Owner
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Owner
api_type:
- schema
ms.assetid: 9d643246-f5ea-462c-9a76-c3b5cce8e740
description: Owner 要素は、タスクの所有者を表します。
ms.openlocfilehash: d4a49367c4a012e8e3c64aa16a4661b285474e0d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465437"
---
# <a name="owner"></a><span data-ttu-id="074ca-103">Owner</span><span class="sxs-lookup"><span data-stu-id="074ca-103">Owner</span></span>

<span data-ttu-id="074ca-104">**Owner**要素は、タスクの所有者を表します。</span><span class="sxs-lookup"><span data-stu-id="074ca-104">The **Owner** element represents the owner of a task.</span></span> 
  
```xml
<Owner/>
```

<span data-ttu-id="074ca-105">**string**</span><span class="sxs-lookup"><span data-stu-id="074ca-105">**string**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="074ca-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="074ca-106">Attributes and elements</span></span>

<span data-ttu-id="074ca-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="074ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="074ca-108">属性</span><span class="sxs-lookup"><span data-stu-id="074ca-108">Attributes</span></span>

<span data-ttu-id="074ca-109">なし。</span><span class="sxs-lookup"><span data-stu-id="074ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="074ca-110">子要素</span><span class="sxs-lookup"><span data-stu-id="074ca-110">Child elements</span></span>

<span data-ttu-id="074ca-111">なし。</span><span class="sxs-lookup"><span data-stu-id="074ca-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="074ca-112">親要素</span><span class="sxs-lookup"><span data-stu-id="074ca-112">Parent elements</span></span>

|<span data-ttu-id="074ca-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="074ca-113">**Element**</span></span>|<span data-ttu-id="074ca-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="074ca-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="074ca-115">Task</span><span class="sxs-lookup"><span data-stu-id="074ca-115">Task</span></span>](task.md) <br/> |<span data-ttu-id="074ca-116">Exchange ストア内のタスクを表します。</span><span class="sxs-lookup"><span data-stu-id="074ca-116">Represents a task in the Exchange store.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="074ca-117">注釈</span><span class="sxs-lookup"><span data-stu-id="074ca-117">Remarks</span></span>

<span data-ttu-id="074ca-118">これは読み取り専用のプロパティです。</span><span class="sxs-lookup"><span data-stu-id="074ca-118">This is a read-only property.</span></span>
  
<span data-ttu-id="074ca-119">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="074ca-119">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="074ca-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="074ca-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="074ca-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="074ca-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="074ca-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="074ca-122">Schema Name</span></span>  <br/> |<span data-ttu-id="074ca-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="074ca-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="074ca-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="074ca-124">Validation File</span></span>  <br/> |<span data-ttu-id="074ca-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="074ca-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="074ca-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="074ca-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="074ca-127">正しくない</span><span class="sxs-lookup"><span data-stu-id="074ca-127">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="074ca-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="074ca-128">See also</span></span>

- [<span data-ttu-id="074ca-129">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="074ca-129">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="074ca-130">タスクの作成</span><span class="sxs-lookup"><span data-stu-id="074ca-130">Creating Tasks</span></span>](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx) 
- [<span data-ttu-id="074ca-131">タスクの削除</span><span class="sxs-lookup"><span data-stu-id="074ca-131">Deleting Tasks</span></span>](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

