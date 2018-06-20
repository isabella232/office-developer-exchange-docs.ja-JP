---
title: 優先度
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Priority
api_type:
- schema
ms.assetid: e1adb8b9-e3d5-469a-b188-822733d2503e
description: 優先順位の要素は、ルールの実行順序を示します。
ms.openlocfilehash: 49e9bda063d8766ff49c8a2e9574c986bcfdbeb2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/15/2018
ms.locfileid: "19832888"
---
# <a name="priority"></a><span data-ttu-id="6162c-103">優先度</span><span class="sxs-lookup"><span data-stu-id="6162c-103">Priority</span></span>

<span data-ttu-id="6162c-104">**優先順位**の要素は、ルールの実行順序を示します。</span><span class="sxs-lookup"><span data-stu-id="6162c-104">The **Priority** element indicates the order in which a rule is to be run.</span></span> 
  
```XML
<Priority/>
```

 <span data-ttu-id="6162c-105">**int**</span><span class="sxs-lookup"><span data-stu-id="6162c-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6162c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6162c-106">Attributes and elements</span></span>

<span data-ttu-id="6162c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6162c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6162c-108">属性</span><span class="sxs-lookup"><span data-stu-id="6162c-108">Attributes</span></span>

<span data-ttu-id="6162c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6162c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6162c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6162c-110">Child elements</span></span>

<span data-ttu-id="6162c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6162c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6162c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6162c-112">Parent elements</span></span>

|<span data-ttu-id="6162c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6162c-113">**Element**</span></span>|<span data-ttu-id="6162c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6162c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6162c-115">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="6162c-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="6162c-116">ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="6162c-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6162c-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6162c-117">Text value</span></span>

<span data-ttu-id="6162c-118">**優先順位**の要素のテキスト値は、ルールの実行の実行順序を示す整数です。</span><span class="sxs-lookup"><span data-stu-id="6162c-118">The text value for the **Priority** element is an integer that indicates the execution order in which a rule should be run.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6162c-119">備考</span><span class="sxs-lookup"><span data-stu-id="6162c-119">Remarks</span></span>

<span data-ttu-id="6162c-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6162c-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6162c-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="6162c-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6162c-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="6162c-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6162c-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6162c-123">Schema Name</span></span>  <br/> |<span data-ttu-id="6162c-124">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="6162c-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6162c-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6162c-125">Validation File</span></span>  <br/> |<span data-ttu-id="6162c-126">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6162c-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6162c-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6162c-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="6162c-128">False</span><span class="sxs-lookup"><span data-stu-id="6162c-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6162c-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="6162c-129">See also</span></span>



- [<span data-ttu-id="6162c-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6162c-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

