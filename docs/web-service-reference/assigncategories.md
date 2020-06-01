---
title: カテゴリを割り当てる
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
description: 割り当てカテゴリ要素は、電子メールメッセージにスタンプされる分類項目を表します。
ms.openlocfilehash: e2dad0e2ef46421ae92a0d2826d161e5e2af3b93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464743"
---
# <a name="assigncategories"></a><span data-ttu-id="75815-103">カテゴリを割り当てる</span><span class="sxs-lookup"><span data-stu-id="75815-103">AssignCategories</span></span>

<span data-ttu-id="75815-104">割り当て**カテゴリ**要素は、電子メールメッセージにスタンプされる分類項目を表します。</span><span class="sxs-lookup"><span data-stu-id="75815-104">The **AssignCategories** element represents the categories that are stamped on e-mail messages.</span></span> 
  
- [<span data-ttu-id="75815-105">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="75815-105">Rule (RuleType)</span></span>](rule-ruletype.md)
  
- [<span data-ttu-id="75815-106">Actions</span><span class="sxs-lookup"><span data-stu-id="75815-106">Actions</span></span>](actions.md)
  
```XML
<AssignCategories>
   <String/>
</AssignCategories>
```

 <span data-ttu-id="75815-107">**ArrayOfStringsType**</span><span class="sxs-lookup"><span data-stu-id="75815-107">**ArrayOfStringsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="75815-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="75815-108">Attributes and elements</span></span>

<span data-ttu-id="75815-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="75815-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="75815-110">属性</span><span class="sxs-lookup"><span data-stu-id="75815-110">Attributes</span></span>

<span data-ttu-id="75815-111">なし。</span><span class="sxs-lookup"><span data-stu-id="75815-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="75815-112">子要素</span><span class="sxs-lookup"><span data-stu-id="75815-112">Child elements</span></span>

|<span data-ttu-id="75815-113">**Element**</span><span class="sxs-lookup"><span data-stu-id="75815-113">**Element**</span></span>|<span data-ttu-id="75815-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="75815-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75815-115">String</span><span class="sxs-lookup"><span data-stu-id="75815-115">String</span></span>](string.md) <br/> |<span data-ttu-id="75815-116">1つのカテゴリを識別する文字列を格納します。</span><span class="sxs-lookup"><span data-stu-id="75815-116">Contains a string that identifies a single category.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="75815-117">親要素</span><span class="sxs-lookup"><span data-stu-id="75815-117">Parent elements</span></span>

|<span data-ttu-id="75815-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="75815-118">**Element**</span></span>|<span data-ttu-id="75815-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="75815-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="75815-120">Actions</span><span class="sxs-lookup"><span data-stu-id="75815-120">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="75815-121">条件が満たされたときに、メッセージに対して実行できるアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="75815-121">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="75815-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="75815-122">Text value</span></span>

<span data-ttu-id="75815-123">なし。</span><span class="sxs-lookup"><span data-stu-id="75815-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="75815-124">注釈</span><span class="sxs-lookup"><span data-stu-id="75815-124">Remarks</span></span>

<span data-ttu-id="75815-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="75815-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="75815-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="75815-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="75815-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="75815-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="75815-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="75815-128">Schema Name</span></span>  <br/> |<span data-ttu-id="75815-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="75815-129">Messages schema</span></span>  <br/> |
|<span data-ttu-id="75815-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="75815-130">Validation File</span></span>  <br/> |<span data-ttu-id="75815-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="75815-131">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="75815-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="75815-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="75815-133">正しい</span><span class="sxs-lookup"><span data-stu-id="75815-133">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="75815-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="75815-134">See also</span></span>

- [<span data-ttu-id="75815-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="75815-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

