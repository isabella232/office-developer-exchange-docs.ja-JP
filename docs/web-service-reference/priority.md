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
description: Priority 要素は、ルールを実行する順序を示します。
ms.openlocfilehash: a5a894bba583618dd04430fc89f125c8920b0202
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462403"
---
# <a name="priority"></a><span data-ttu-id="cc262-103">優先度</span><span class="sxs-lookup"><span data-stu-id="cc262-103">Priority</span></span>

<span data-ttu-id="cc262-104">**Priority**要素は、ルールを実行する順序を示します。</span><span class="sxs-lookup"><span data-stu-id="cc262-104">The **Priority** element indicates the order in which a rule is to be run.</span></span> 
  
```XML
<Priority/>
```

 <span data-ttu-id="cc262-105">**int**</span><span class="sxs-lookup"><span data-stu-id="cc262-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cc262-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cc262-106">Attributes and elements</span></span>

<span data-ttu-id="cc262-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cc262-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc262-108">属性</span><span class="sxs-lookup"><span data-stu-id="cc262-108">Attributes</span></span>

<span data-ttu-id="cc262-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cc262-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cc262-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cc262-110">Child elements</span></span>

<span data-ttu-id="cc262-111">なし。</span><span class="sxs-lookup"><span data-stu-id="cc262-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cc262-112">親要素</span><span class="sxs-lookup"><span data-stu-id="cc262-112">Parent elements</span></span>

|<span data-ttu-id="cc262-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="cc262-113">**Element**</span></span>|<span data-ttu-id="cc262-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="cc262-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc262-115">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="cc262-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="cc262-116">ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="cc262-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cc262-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cc262-117">Text value</span></span>

<span data-ttu-id="cc262-118">**Priority**要素のテキスト値は、ルールを実行する実行順序を示す整数です。</span><span class="sxs-lookup"><span data-stu-id="cc262-118">The text value for the **Priority** element is an integer that indicates the execution order in which a rule should be run.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="cc262-119">注釈</span><span class="sxs-lookup"><span data-stu-id="cc262-119">Remarks</span></span>

<span data-ttu-id="cc262-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cc262-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cc262-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cc262-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc262-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="cc262-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cc262-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cc262-123">Schema Name</span></span>  <br/> |<span data-ttu-id="cc262-124">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="cc262-124">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cc262-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cc262-125">Validation File</span></span>  <br/> |<span data-ttu-id="cc262-126">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="cc262-126">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cc262-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cc262-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="cc262-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="cc262-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cc262-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="cc262-129">See also</span></span>



- [<span data-ttu-id="cc262-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="cc262-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

