---
title: PermanentDelete
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PermanentDelete
api_type:
- schema
ms.assetid: 1a0e0f46-1472-4eb7-bb54-f193a2603587
description: PermanentDelete 要素は、メッセージが完全に削除され、削除済みアイテムフォルダーに保存されないようにするかどうかを示します。
ms.openlocfilehash: da7680eefca9ad359948af38eac49d18e9055988
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467768"
---
# <a name="permanentdelete"></a><span data-ttu-id="5b2b6-103">PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="5b2b6-103">PermanentDelete</span></span>

<span data-ttu-id="5b2b6-104">**PermanentDelete**要素は、メッセージが完全に削除され、削除済みアイテムフォルダーに保存されないようにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="5b2b6-104">The **PermanentDelete** element indicates whether messages are to be permanently deleted and not saved to the Deleted Items folder.</span></span> 
  
```XML
<PermanentDelete>true | false</PermanentDelete>
```

 <span data-ttu-id="5b2b6-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="5b2b6-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5b2b6-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5b2b6-106">Attributes and elements</span></span>

<span data-ttu-id="5b2b6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5b2b6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5b2b6-108">属性</span><span class="sxs-lookup"><span data-stu-id="5b2b6-108">Attributes</span></span>

<span data-ttu-id="5b2b6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5b2b6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5b2b6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5b2b6-110">Child elements</span></span>

<span data-ttu-id="5b2b6-111">なし。</span><span class="sxs-lookup"><span data-stu-id="5b2b6-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5b2b6-112">親要素</span><span class="sxs-lookup"><span data-stu-id="5b2b6-112">Parent elements</span></span>

|<span data-ttu-id="5b2b6-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="5b2b6-113">**Element**</span></span>|<span data-ttu-id="5b2b6-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="5b2b6-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5b2b6-115">Actions</span><span class="sxs-lookup"><span data-stu-id="5b2b6-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="5b2b6-116">条件が満たされたときに、メッセージに対して実行できるアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="5b2b6-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="5b2b6-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="5b2b6-117">Text value</span></span>

<span data-ttu-id="5b2b6-118">テキスト値が**true の場合**は、メッセージを完全に削除するようにマークする必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="5b2b6-118">A text value of **true** indicates that the message must be marked to be permanently deleted.</span></span> <span data-ttu-id="5b2b6-119">値が**false**の場合、メッセージを完全に削除するようにマークすることはできません。</span><span class="sxs-lookup"><span data-stu-id="5b2b6-119">A value of **false** indicates that the message must not be marked to be permanently deleted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="5b2b6-120">注釈</span><span class="sxs-lookup"><span data-stu-id="5b2b6-120">Remarks</span></span>

<span data-ttu-id="5b2b6-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5b2b6-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5b2b6-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5b2b6-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5b2b6-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="5b2b6-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5b2b6-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5b2b6-124">Schema Name</span></span>  <br/> |<span data-ttu-id="5b2b6-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="5b2b6-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5b2b6-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5b2b6-126">Validation File</span></span>  <br/> |<span data-ttu-id="5b2b6-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="5b2b6-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5b2b6-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5b2b6-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="5b2b6-129">正しい</span><span class="sxs-lookup"><span data-stu-id="5b2b6-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5b2b6-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="5b2b6-130">See also</span></span>



- [<span data-ttu-id="5b2b6-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5b2b6-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

