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
description: IsInError 要素は、ルールがエラー状態であるかどうかを示します。
ms.openlocfilehash: 9e642c9f89434bdcad97b0c16dc35f99196051d7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464218"
---
# <a name="isinerror"></a><span data-ttu-id="6b5c5-103">IsInError</span><span class="sxs-lookup"><span data-stu-id="6b5c5-103">IsInError</span></span>

<span data-ttu-id="6b5c5-104">**IsInError**要素は、ルールがエラー状態であるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="6b5c5-104">The **IsInError** element indicates whether the rule is in an error condition.</span></span> 
  
```XML
<IsInError/>
```

 <span data-ttu-id="6b5c5-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="6b5c5-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b5c5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6b5c5-106">Attributes and elements</span></span>

<span data-ttu-id="6b5c5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6b5c5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b5c5-108">属性</span><span class="sxs-lookup"><span data-stu-id="6b5c5-108">Attributes</span></span>

<span data-ttu-id="6b5c5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6b5c5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b5c5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6b5c5-110">Child elements</span></span>

<span data-ttu-id="6b5c5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6b5c5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6b5c5-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6b5c5-112">Parent elements</span></span>

|<span data-ttu-id="6b5c5-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6b5c5-113">**Element**</span></span>|<span data-ttu-id="6b5c5-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6b5c5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b5c5-115">ルール (RuleType)</span><span class="sxs-lookup"><span data-stu-id="6b5c5-115">Rule (RuleType)</span></span>](rule-ruletype.md) <br/> |<span data-ttu-id="6b5c5-116">ユーザーのメールボックス内のルールを表します。</span><span class="sxs-lookup"><span data-stu-id="6b5c5-116">Represents a rule in the user's mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6b5c5-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6b5c5-117">Text value</span></span>

<span data-ttu-id="6b5c5-118">テキスト値が**true の場合**は、ルールがエラー状態であることを示します。</span><span class="sxs-lookup"><span data-stu-id="6b5c5-118">A text value of **true** indicates that the rule is in an error condition.</span></span> <span data-ttu-id="6b5c5-119">値が**false**の場合は、ルールがエラー状態ではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="6b5c5-119">A value of **false** indicates that the rule is not in an error condition.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6b5c5-120">注釈</span><span class="sxs-lookup"><span data-stu-id="6b5c5-120">Remarks</span></span>

<span data-ttu-id="6b5c5-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6b5c5-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b5c5-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6b5c5-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b5c5-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="6b5c5-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6b5c5-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6b5c5-124">Schema Name</span></span>  <br/> |<span data-ttu-id="6b5c5-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="6b5c5-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6b5c5-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6b5c5-126">Validation File</span></span>  <br/> |<span data-ttu-id="6b5c5-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="6b5c5-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6b5c5-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6b5c5-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="6b5c5-129">正しい</span><span class="sxs-lookup"><span data-stu-id="6b5c5-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6b5c5-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="6b5c5-130">See also</span></span>



- [<span data-ttu-id="6b5c5-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6b5c5-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

