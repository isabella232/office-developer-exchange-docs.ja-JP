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
description: MarkAsRead 要素は、メッセージを既読としてマークするかどうかを示します。
ms.openlocfilehash: b453ad73912e99b6fd3aed84b03a7d2fc2b6a294
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832355"
---
# <a name="markasread"></a><span data-ttu-id="e6431-103">MarkAsRead</span><span class="sxs-lookup"><span data-stu-id="e6431-103">MarkAsRead</span></span>

<span data-ttu-id="e6431-104">**MarkAsRead**要素は、メッセージを既読としてマークするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e6431-104">The **MarkAsRead** element indicates whether messages are to be marked as read.</span></span> 
  
```XML
<MarkAsRead>true | false</MarkAsRead>
```

 <span data-ttu-id="e6431-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="e6431-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e6431-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e6431-106">Attributes and elements</span></span>

<span data-ttu-id="e6431-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e6431-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e6431-108">属性</span><span class="sxs-lookup"><span data-stu-id="e6431-108">Attributes</span></span>

<span data-ttu-id="e6431-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e6431-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e6431-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e6431-110">Child elements</span></span>

<span data-ttu-id="e6431-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e6431-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e6431-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e6431-112">Parent elements</span></span>

|<span data-ttu-id="e6431-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e6431-113">**Element**</span></span>|<span data-ttu-id="e6431-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e6431-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e6431-115">アクション</span><span class="sxs-lookup"><span data-stu-id="e6431-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="e6431-116">条件が満たされるときに、メッセージに対して実行される使用可能なアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="e6431-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e6431-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e6431-117">Text value</span></span>

<span data-ttu-id="e6431-118">**True**の場合、テキスト値は、メッセージは開封としてマークする必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="e6431-118">A text value of **true** indicates that the message must be marked as read.</span></span> <span data-ttu-id="e6431-119">**False**の値は、メッセージが既読としてマークされていない必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="e6431-119">A value of **false** indicates that messages must not be marked as read.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e6431-120">備考</span><span class="sxs-lookup"><span data-stu-id="e6431-120">Remarks</span></span>

<span data-ttu-id="e6431-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e6431-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e6431-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="e6431-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e6431-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="e6431-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e6431-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e6431-124">Schema Name</span></span>  <br/> |<span data-ttu-id="e6431-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e6431-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e6431-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e6431-126">Validation File</span></span>  <br/> |<span data-ttu-id="e6431-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e6431-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e6431-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e6431-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="e6431-129">True</span><span class="sxs-lookup"><span data-stu-id="e6431-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e6431-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="e6431-130">See also</span></span>



- [<span data-ttu-id="e6431-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e6431-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

