---
title: TaskSuggestion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ade9ea3b-bdf1-4999-ac7d-44c6452cef36
description: TaskSuggestion 要素には、アイテムから抽出されたエンティティに起因するタスクのヒントが含まれています。
ms.openlocfilehash: bf12c3dc8b58b6be873e0a9b0863c80051eb4e11
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839651"
---
# <a name="tasksuggestion"></a><span data-ttu-id="7e4bc-103">TaskSuggestion</span><span class="sxs-lookup"><span data-stu-id="7e4bc-103">TaskSuggestion</span></span>

<span data-ttu-id="7e4bc-104">**TaskSuggestion**要素には、アイテムから抽出されたエンティティに起因するタスクのヒントが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e4bc-104">The **TaskSuggestion** element contains a task suggestion that resulted from an entity extracted from an item.</span></span> 
  
```XML
<TaskSuggestion>
   <Position/>
   <TaskString/>
   <Assignees/>
</TaskSuggestion>
```

<span data-ttu-id="7e4bc-105">**TaskSuggestionType**</span><span class="sxs-lookup"><span data-stu-id="7e4bc-105">**TaskSuggestionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7e4bc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7e4bc-106">Attributes and elements</span></span>

<span data-ttu-id="7e4bc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7e4bc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e4bc-108">属性</span><span class="sxs-lookup"><span data-stu-id="7e4bc-108">Attributes</span></span>

<span data-ttu-id="7e4bc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7e4bc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7e4bc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7e4bc-110">Child elements</span></span>

<span data-ttu-id="7e4bc-111">[位置](position.md) | [TaskString](taskstring.md) | [タスク実施者](assignees.md)</span><span class="sxs-lookup"><span data-stu-id="7e4bc-111">[Position](position.md) | [TaskString](taskstring.md) | [Assignees](assignees.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7e4bc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="7e4bc-112">Parent elements</span></span>

[<span data-ttu-id="7e4bc-113">TaskSuggestions</span><span class="sxs-lookup"><span data-stu-id="7e4bc-113">TaskSuggestions</span></span>](tasksuggestions.md)
  
## <a name="remarks"></a><span data-ttu-id="7e4bc-114">備考</span><span class="sxs-lookup"><span data-stu-id="7e4bc-114">Remarks</span></span>

<span data-ttu-id="7e4bc-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7e4bc-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="7e4bc-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7e4bc-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e4bc-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="7e4bc-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e4bc-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="7e4bc-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7e4bc-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7e4bc-119">Schema name</span></span>  <br/> |<span data-ttu-id="7e4bc-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7e4bc-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="7e4bc-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7e4bc-121">Validation file</span></span>  <br/> |<span data-ttu-id="7e4bc-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7e4bc-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7e4bc-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7e4bc-123">Can be empty</span></span>  <br/> ||
   

