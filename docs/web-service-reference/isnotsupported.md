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
description: IsNotSupported 要素は、マネージコード Api を使用してルールを変更できないかどうかを示します。
ms.openlocfilehash: e2d0c506209978fd5e8702e0de6cddf2e9c4b7fa
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465836"
---
# <a name="isnotsupported"></a><span data-ttu-id="a93ef-103">IsNotSupported</span><span class="sxs-lookup"><span data-stu-id="a93ef-103">IsNotSupported</span></span>

<span data-ttu-id="a93ef-104">**IsNotSupported**要素は、マネージコード api を使用してルールを変更できないかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="a93ef-104">The **IsNotSupported** element indicates whether the rule cannot be modified by using the managed code APIs.</span></span> 
  
```XML
<IsNotSupported/>
```

 <span data-ttu-id="a93ef-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="a93ef-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a93ef-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a93ef-106">Attributes and elements</span></span>

<span data-ttu-id="a93ef-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a93ef-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a93ef-108">属性</span><span class="sxs-lookup"><span data-stu-id="a93ef-108">Attributes</span></span>

<span data-ttu-id="a93ef-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a93ef-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a93ef-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a93ef-110">Child elements</span></span>

<span data-ttu-id="a93ef-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a93ef-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a93ef-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a93ef-112">Parent elements</span></span>

|<span data-ttu-id="a93ef-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a93ef-113">**Element**</span></span>|<span data-ttu-id="a93ef-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a93ef-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a93ef-115">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="a93ef-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="a93ef-116">ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="a93ef-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a93ef-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a93ef-117">Text value</span></span>

<span data-ttu-id="a93ef-118">テキスト値が**true の場合**は、マネージコード api を使用してルールを変更できないことを示します。</span><span class="sxs-lookup"><span data-stu-id="a93ef-118">A text value of **true** indicates that the rule cannot be modified by using the managed code APIs.</span></span> <span data-ttu-id="a93ef-119">値が**false**の場合、マネージコード api を使用してルールを変更できることを示します。</span><span class="sxs-lookup"><span data-stu-id="a93ef-119">A value of **false** indicates that the rule can be modified by using the managed code APIs.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a93ef-120">注釈</span><span class="sxs-lookup"><span data-stu-id="a93ef-120">Remarks</span></span>

<span data-ttu-id="a93ef-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a93ef-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a93ef-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a93ef-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a93ef-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="a93ef-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a93ef-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a93ef-124">Schema Name</span></span>  <br/> |<span data-ttu-id="a93ef-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="a93ef-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a93ef-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a93ef-126">Validation File</span></span>  <br/> |<span data-ttu-id="a93ef-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="a93ef-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a93ef-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a93ef-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="a93ef-129">正しい</span><span class="sxs-lookup"><span data-stu-id="a93ef-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a93ef-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="a93ef-130">See also</span></span>



- [<span data-ttu-id="a93ef-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a93ef-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

