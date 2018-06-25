---
title: IsInError
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsInError
api_type:
- schema
ms.assetid: f56e6c31-a566-4761-8755-d90ffe6fe790
description: IsInError 要素は、ルールにエラーが発生するかどうかを示します。
ms.openlocfilehash: 9f77bbe11106174d0e82c5257e08c3728d67c60c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832033"
---
# <a name="isinerror"></a><span data-ttu-id="82d91-103">IsInError</span><span class="sxs-lookup"><span data-stu-id="82d91-103">IsInError</span></span>

<span data-ttu-id="82d91-104">**IsInError**要素は、ルールにエラーが発生するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="82d91-104">The **IsInError** element indicates whether the rule is in an error condition.</span></span> 
  
```XML
<IsInError/>
```

 <span data-ttu-id="82d91-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="82d91-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="82d91-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="82d91-106">Attributes and elements</span></span>

<span data-ttu-id="82d91-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="82d91-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="82d91-108">属性</span><span class="sxs-lookup"><span data-stu-id="82d91-108">Attributes</span></span>

<span data-ttu-id="82d91-109">なし。</span><span class="sxs-lookup"><span data-stu-id="82d91-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="82d91-110">子要素</span><span class="sxs-lookup"><span data-stu-id="82d91-110">Child elements</span></span>

<span data-ttu-id="82d91-111">なし。</span><span class="sxs-lookup"><span data-stu-id="82d91-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="82d91-112">親要素</span><span class="sxs-lookup"><span data-stu-id="82d91-112">Parent elements</span></span>

|<span data-ttu-id="82d91-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="82d91-113">**Element**</span></span>|<span data-ttu-id="82d91-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="82d91-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="82d91-115">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="82d91-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="82d91-116">ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="82d91-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="82d91-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="82d91-117">Text value</span></span>

<span data-ttu-id="82d91-118">**True**の場合、テキスト値は、ルールが、エラー状態にあることを示します。</span><span class="sxs-lookup"><span data-stu-id="82d91-118">A text value of **true** indicates that the rule is in an error condition.</span></span> <span data-ttu-id="82d91-119">**False**の値は、ルールがエラー状態でないことを示します。</span><span class="sxs-lookup"><span data-stu-id="82d91-119">A value of **false** indicates that the rule is not in an error condition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="82d91-120">備考</span><span class="sxs-lookup"><span data-stu-id="82d91-120">Remarks</span></span>

<span data-ttu-id="82d91-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="82d91-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="82d91-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="82d91-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="82d91-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="82d91-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="82d91-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="82d91-124">Schema Name</span></span>  <br/> |<span data-ttu-id="82d91-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="82d91-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="82d91-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="82d91-126">Validation File</span></span>  <br/> |<span data-ttu-id="82d91-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="82d91-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="82d91-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="82d91-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="82d91-129">True</span><span class="sxs-lookup"><span data-stu-id="82d91-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="82d91-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="82d91-130">See also</span></span>



- [<span data-ttu-id="82d91-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="82d91-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

