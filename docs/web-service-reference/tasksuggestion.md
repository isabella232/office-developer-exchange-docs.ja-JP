---
title: TaskSuggestion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ade9ea3b-bdf1-4999-ac7d-44c6452cef36
description: TaskSuggestion 要素には、アイテムから抽出されたエンティティから発生したタスクの提案が含まれています。
ms.openlocfilehash: 49564c246596dabbf7fbacf2924eeb877698ea1a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468125"
---
# <a name="tasksuggestion"></a><span data-ttu-id="a2b4c-103">TaskSuggestion</span><span class="sxs-lookup"><span data-stu-id="a2b4c-103">TaskSuggestion</span></span>

<span data-ttu-id="a2b4c-104">**Tasksuggestion**要素には、アイテムから抽出されたエンティティから発生したタスクの提案が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a2b4c-104">The **TaskSuggestion** element contains a task suggestion that resulted from an entity extracted from an item.</span></span> 
  
```XML
<TaskSuggestion>
   <Position/>
   <TaskString/>
   <Assignees/>
</TaskSuggestion>
```

<span data-ttu-id="a2b4c-105">**TaskSuggestionType**</span><span class="sxs-lookup"><span data-stu-id="a2b4c-105">**TaskSuggestionType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a2b4c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a2b4c-106">Attributes and elements</span></span>

<span data-ttu-id="a2b4c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a2b4c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2b4c-108">属性</span><span class="sxs-lookup"><span data-stu-id="a2b4c-108">Attributes</span></span>

<span data-ttu-id="a2b4c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a2b4c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2b4c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a2b4c-110">Child elements</span></span>

<span data-ttu-id="a2b4c-111">[Position](position.md)  | [Taskstring](taskstring.md)  | [タスク](assignees.md)実施者</span><span class="sxs-lookup"><span data-stu-id="a2b4c-111">[Position](position.md) | [TaskString](taskstring.md) | [Assignees](assignees.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a2b4c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a2b4c-112">Parent elements</span></span>

[<span data-ttu-id="a2b4c-113">TaskSuggestions</span><span class="sxs-lookup"><span data-stu-id="a2b4c-113">TaskSuggestions</span></span>](tasksuggestions.md)
  
## <a name="remarks"></a><span data-ttu-id="a2b4c-114">注釈</span><span class="sxs-lookup"><span data-stu-id="a2b4c-114">Remarks</span></span>

<span data-ttu-id="a2b4c-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a2b4c-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a2b4c-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a2b4c-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2b4c-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a2b4c-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2b4c-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="a2b4c-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a2b4c-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a2b4c-119">Schema name</span></span>  <br/> |<span data-ttu-id="a2b4c-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a2b4c-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="a2b4c-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a2b4c-121">Validation file</span></span>  <br/> |<span data-ttu-id="a2b4c-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a2b4c-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a2b4c-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a2b4c-123">Can be empty</span></span>  <br/> ||
   

