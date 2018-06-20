---
title: AssignCategories
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- AssignCategories
api_type:
- schema
ms.assetid: f5c73fed-7b00-446d-8296-71a0c86e7fc6
description: AssignCategories 要素は、電子メール メッセージにスタンプされているカテゴリを表します。
ms.openlocfilehash: 96c77306d649677c1be745e8cadc2886e4a84c8a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759441"
---
# <a name="assigncategories"></a><span data-ttu-id="202d4-103">AssignCategories</span><span class="sxs-lookup"><span data-stu-id="202d4-103">AssignCategories</span></span>

<span data-ttu-id="202d4-104">**AssignCategories**要素は、電子メール メッセージにスタンプされているカテゴリを表します。</span><span class="sxs-lookup"><span data-stu-id="202d4-104">The **AssignCategories** element represents the categories that are stamped on e-mail messages.</span></span> 
  
- [<span data-ttu-id="202d4-105">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="202d4-105">Rule (RuleType)</span></span>](rule-ruletype.md)
  
- [<span data-ttu-id="202d4-106">アクション</span><span class="sxs-lookup"><span data-stu-id="202d4-106">Actions</span></span>](actions.md)
  
```XML
<AssignCategories>
   <String/>
</AssignCategories>
```

 <span data-ttu-id="202d4-107">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="202d4-107">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="202d4-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="202d4-108">Attributes and elements</span></span>

<span data-ttu-id="202d4-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="202d4-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="202d4-110">属性</span><span class="sxs-lookup"><span data-stu-id="202d4-110">Attributes</span></span>

<span data-ttu-id="202d4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="202d4-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="202d4-112">子要素</span><span class="sxs-lookup"><span data-stu-id="202d4-112">Child elements</span></span>

|<span data-ttu-id="202d4-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="202d4-113">**Element**</span></span>|<span data-ttu-id="202d4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="202d4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="202d4-115">String</span><span class="sxs-lookup"><span data-stu-id="202d4-115">String</span></span>](string.md) <br/> |<span data-ttu-id="202d4-116">1 つのカテゴリを識別する文字列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="202d4-116">Contains a string that identifies a single category.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="202d4-117">親要素</span><span class="sxs-lookup"><span data-stu-id="202d4-117">Parent elements</span></span>

|<span data-ttu-id="202d4-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="202d4-118">**Element**</span></span>|<span data-ttu-id="202d4-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="202d4-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="202d4-120">アクション</span><span class="sxs-lookup"><span data-stu-id="202d4-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="202d4-121">条件が満たされるときに、メッセージに対して実行される使用可能なアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="202d4-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="202d4-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="202d4-122">Text value</span></span>

<span data-ttu-id="202d4-123">なし。</span><span class="sxs-lookup"><span data-stu-id="202d4-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="202d4-124">備考</span><span class="sxs-lookup"><span data-stu-id="202d4-124">Remarks</span></span>

<span data-ttu-id="202d4-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="202d4-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="202d4-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="202d4-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="202d4-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="202d4-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="202d4-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="202d4-128">Schema Name</span></span>  <br/> |<span data-ttu-id="202d4-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="202d4-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="202d4-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="202d4-130">Validation File</span></span>  <br/> |<span data-ttu-id="202d4-131">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="202d4-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="202d4-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="202d4-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="202d4-133">True</span><span class="sxs-lookup"><span data-stu-id="202d4-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="202d4-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="202d4-134">See also</span></span>

- [<span data-ttu-id="202d4-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="202d4-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

