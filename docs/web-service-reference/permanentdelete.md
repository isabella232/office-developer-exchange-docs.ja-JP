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
description: PermanentDelete 要素は、メッセージを完全に削除され、削除済みアイテム フォルダーに保存されませんにするかどうかを示します。
ms.openlocfilehash: 40cf80e054bb70a3f6d687e8d4361f1d4331a7f8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832724"
---
# <a name="permanentdelete"></a><span data-ttu-id="1ca2a-103">PermanentDelete</span><span class="sxs-lookup"><span data-stu-id="1ca2a-103">PermanentDelete</span></span>

<span data-ttu-id="1ca2a-104">**PermanentDelete**要素は、メッセージを完全に削除され、削除済みアイテム フォルダーに保存されませんにするかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-104">The **PermanentDelete** element indicates whether messages are to be permanently deleted and not saved to the Deleted Items folder.</span></span> 
  
```XML
<PermanentDelete>true | false</PermanentDelete>
```

 <span data-ttu-id="1ca2a-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="1ca2a-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1ca2a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1ca2a-106">Attributes and elements</span></span>

<span data-ttu-id="1ca2a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1ca2a-108">属性</span><span class="sxs-lookup"><span data-stu-id="1ca2a-108">Attributes</span></span>

<span data-ttu-id="1ca2a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1ca2a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1ca2a-110">Child elements</span></span>

<span data-ttu-id="1ca2a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1ca2a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="1ca2a-112">Parent elements</span></span>

|<span data-ttu-id="1ca2a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="1ca2a-113">**Element**</span></span>|<span data-ttu-id="1ca2a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1ca2a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1ca2a-115">アクション</span><span class="sxs-lookup"><span data-stu-id="1ca2a-115">Actions</span></span>](actions.md) <br/> |<span data-ttu-id="1ca2a-116">条件が満たされるときに、メッセージに対して実行される使用可能なアクションのセットを表します。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-116">Represents the set of actions that are available to be taken on a message when the conditions are fulfilled.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1ca2a-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1ca2a-117">Text value</span></span>

<span data-ttu-id="1ca2a-118">**True**の場合、テキスト値は完全に削除するメッセージをマークする必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-118">A text value of **true** indicates that the message must be marked to be permanently deleted.</span></span> <span data-ttu-id="1ca2a-119">**False**の値は、メッセージが完全に削除するのにはマークされていない必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-119">A value of **false** indicates that the message must not be marked to be permanently deleted.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="1ca2a-120">備考</span><span class="sxs-lookup"><span data-stu-id="1ca2a-120">Remarks</span></span>

<span data-ttu-id="1ca2a-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1ca2a-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1ca2a-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="1ca2a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1ca2a-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="1ca2a-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1ca2a-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1ca2a-124">Schema Name</span></span>  <br/> |<span data-ttu-id="1ca2a-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="1ca2a-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1ca2a-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1ca2a-126">Validation File</span></span>  <br/> |<span data-ttu-id="1ca2a-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1ca2a-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1ca2a-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1ca2a-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="1ca2a-129">True</span><span class="sxs-lookup"><span data-stu-id="1ca2a-129">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1ca2a-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="1ca2a-130">See also</span></span>



- [<span data-ttu-id="1ca2a-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1ca2a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

