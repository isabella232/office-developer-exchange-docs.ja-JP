---
title: MarkAsRead
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MarkAsRead
api_type:
- schema
ms.assetid: 404842e1-fbdb-480d-a1d8-ba1ab2c9fb1e
description: MarkAsRead 要素は、メッセージを開封済みとしてマークするかどうかを示します。
ms.openlocfilehash: 691409a4eace8885d36f4b30b8eef1aca8c332a6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461766"
---
# <a name="markasread"></a><span data-ttu-id="c6674-103">MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="c6674-103">MarkAsRead</span></span>

<span data-ttu-id="c6674-104">**Markasread**要素は、メッセージを開封済みとしてマークするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="c6674-104">The **MarkAsRead** element indicates whether messages are to be marked as read.</span></span> 
  
```XML
<MarkAsRead>true | false</MarkAsRead>
```

 <span data-ttu-id="c6674-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="c6674-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c6674-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c6674-106">Attributes and elements</span></span>

<span data-ttu-id="c6674-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c6674-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6674-108">属性</span><span class="sxs-lookup"><span data-stu-id="c6674-108">Attributes</span></span>

<span data-ttu-id="c6674-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c6674-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c6674-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c6674-110">Child elements</span></span>

<span data-ttu-id="c6674-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c6674-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c6674-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c6674-112">Parent elements</span></span>

|<span data-ttu-id="c6674-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c6674-113">**Element**</span></span>|<span data-ttu-id="c6674-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c6674-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6674-115">Actions</span><span class="sxs-lookup"><span data-stu-id="c6674-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="c6674-116">条件が満たされたときに、メッセージに対して実行できるアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="c6674-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c6674-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c6674-117">Text value</span></span>

<span data-ttu-id="c6674-118">テキスト値が**true の場合**は、メッセージが開封済みとしてマークされている必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="c6674-118">A text value of **true** indicates that the message must be marked as read.</span></span> <span data-ttu-id="c6674-119">値が**false**の場合、メッセージは開封済みとしてマークされていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="c6674-119">A value of **false** indicates that messages must not be marked as read.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c6674-120">注釈</span><span class="sxs-lookup"><span data-stu-id="c6674-120">Remarks</span></span>

<span data-ttu-id="c6674-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c6674-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c6674-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c6674-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6674-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="c6674-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c6674-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c6674-124">Schema Name</span></span>  <br/> |<span data-ttu-id="c6674-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="c6674-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c6674-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c6674-126">Validation File</span></span>  <br/> |<span data-ttu-id="c6674-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c6674-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c6674-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c6674-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="c6674-129">正しい</span><span class="sxs-lookup"><span data-stu-id="c6674-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c6674-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="c6674-130">See also</span></span>



- [<span data-ttu-id="c6674-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c6674-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

