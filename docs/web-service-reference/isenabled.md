---
title: IsEnabled
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsEnabled
api_type:
- schema
ms.assetid: c7e3035e-a4ef-4c11-8cb0-214790a554ff
description: 有効要素では、ルールが有効になっているかどうかを示します。
ms.openlocfilehash: d0f0a77ec1ec952ac1cd9d9ad686ccfcb8f70c42
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832000"
---
# <a name="isenabled"></a><span data-ttu-id="d831b-103">IsEnabled</span><span class="sxs-lookup"><span data-stu-id="d831b-103">IsEnabled</span></span>

<span data-ttu-id="d831b-104">**有効**要素では、ルールが有効になっているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="d831b-104">The **IsEnabled** element indicates whether the rule is enabled.</span></span> 
  
```XML
<IsEnabled/>
```

 <span data-ttu-id="d831b-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="d831b-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d831b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d831b-106">Attributes and elements</span></span>

<span data-ttu-id="d831b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d831b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d831b-108">属性</span><span class="sxs-lookup"><span data-stu-id="d831b-108">Attributes</span></span>

<span data-ttu-id="d831b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d831b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d831b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d831b-110">Child elements</span></span>

<span data-ttu-id="d831b-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d831b-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d831b-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d831b-112">Parent elements</span></span>

|<span data-ttu-id="d831b-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d831b-113">**Element**</span></span>|<span data-ttu-id="d831b-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d831b-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d831b-115">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="d831b-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="d831b-116">ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="d831b-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d831b-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d831b-117">Text value</span></span>

<span data-ttu-id="d831b-118">**True**の場合、テキスト値は、ルールが有効で、実行できることを示します。</span><span class="sxs-lookup"><span data-stu-id="d831b-118">A text value of **true** indicates that the rule is enabled and can be executed.</span></span> <span data-ttu-id="d831b-119">**False**の値は、ルールを実行できないことを示します。</span><span class="sxs-lookup"><span data-stu-id="d831b-119">A value of **false** indicates that the rule cannot be executed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d831b-120">備考</span><span class="sxs-lookup"><span data-stu-id="d831b-120">Remarks</span></span>

<span data-ttu-id="d831b-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d831b-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d831b-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="d831b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d831b-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="d831b-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d831b-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d831b-124">Schema Name</span></span>  <br/> |<span data-ttu-id="d831b-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="d831b-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d831b-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d831b-126">Validation File</span></span>  <br/> |<span data-ttu-id="d831b-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d831b-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d831b-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d831b-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="d831b-129">True</span><span class="sxs-lookup"><span data-stu-id="d831b-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d831b-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="d831b-130">See also</span></span>



- [<span data-ttu-id="d831b-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d831b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

