---
title: IsNotSupported
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsNotSupported
api_type:
- schema
ms.assetid: 4db469ae-1515-47ea-9905-6aabf199febd
description: IsNotSupported 要素は、マネージ コードの Api を使用してルールを変更できないかどうかを示します。
ms.openlocfilehash: 2468d47dbfdcaf1a28ed1a4afb1e7ea60147d1dc
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832057"
---
# <a name="isnotsupported"></a><span data-ttu-id="a6604-103">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="a6604-103">IsNotSupported</span></span>

<span data-ttu-id="a6604-104">**IsNotSupported**要素は、マネージ コードの Api を使用してルールを変更できないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a6604-104">The **IsNotSupported** element indicates whether the rule cannot be modified by using the managed code APIs.</span></span> 
  
```XML
<IsNotSupported/>
```

 <span data-ttu-id="a6604-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="a6604-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a6604-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a6604-106">Attributes and elements</span></span>

<span data-ttu-id="a6604-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a6604-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a6604-108">属性</span><span class="sxs-lookup"><span data-stu-id="a6604-108">Attributes</span></span>

<span data-ttu-id="a6604-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a6604-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a6604-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a6604-110">Child elements</span></span>

<span data-ttu-id="a6604-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a6604-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a6604-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a6604-112">Parent elements</span></span>

|<span data-ttu-id="a6604-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a6604-113">**Element**</span></span>|<span data-ttu-id="a6604-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a6604-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a6604-115">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="a6604-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="a6604-116">ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="a6604-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a6604-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a6604-117">Text value</span></span>

<span data-ttu-id="a6604-118">**True**の場合、テキスト値は、マネージ コードの Api を使用してルールを変更できないことを示します。</span><span class="sxs-lookup"><span data-stu-id="a6604-118">A text value of **true** indicates that the rule cannot be modified by using the managed code APIs.</span></span> <span data-ttu-id="a6604-119">**False**の値は、マネージ コードの Api を使用してルールを変更できることをことを示します。</span><span class="sxs-lookup"><span data-stu-id="a6604-119">A value of **false** indicates that the rule can be modified by using the managed code APIs.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a6604-120">備考</span><span class="sxs-lookup"><span data-stu-id="a6604-120">Remarks</span></span>

<span data-ttu-id="a6604-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a6604-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a6604-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="a6604-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a6604-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="a6604-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a6604-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a6604-124">Schema Name</span></span>  <br/> |<span data-ttu-id="a6604-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="a6604-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a6604-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a6604-126">Validation File</span></span>  <br/> |<span data-ttu-id="a6604-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a6604-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a6604-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a6604-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="a6604-129">True</span><span class="sxs-lookup"><span data-stu-id="a6604-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a6604-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="a6604-130">See also</span></span>



- [<span data-ttu-id="a6604-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a6604-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

