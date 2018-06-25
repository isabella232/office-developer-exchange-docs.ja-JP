---
title: UnreadCount
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnreadCount
api_type:
- schema
ms.assetid: 53b22647-1453-4707-9ea0-6a8369748d56
description: UnreadCount 要素には、フォルダー内の未読アイテムの数が含まれています。
ms.openlocfilehash: fbe887f8f6d83fbcf48ed9593b3d19322a7f48be
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839814"
---
# <a name="unreadcount"></a><span data-ttu-id="d1cf4-103">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="d1cf4-103">UnreadCount</span></span>

<span data-ttu-id="d1cf4-104">**UnreadCount**要素には、フォルダー内の未読アイテムの数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d1cf4-104">The **UnreadCount** element contains the count of unread items within a folder.</span></span> 
  
```XML
<UnreadCount/>
```

 <span data-ttu-id="d1cf4-105">**xs:int**</span><span class="sxs-lookup"><span data-stu-id="d1cf4-105">**xs:int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d1cf4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d1cf4-106">Attributes and elements</span></span>

<span data-ttu-id="d1cf4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d1cf4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d1cf4-108">属性</span><span class="sxs-lookup"><span data-stu-id="d1cf4-108">Attributes</span></span>

<span data-ttu-id="d1cf4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d1cf4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d1cf4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d1cf4-110">Child elements</span></span>

<span data-ttu-id="d1cf4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d1cf4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d1cf4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d1cf4-112">Parent elements</span></span>

|<span data-ttu-id="d1cf4-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d1cf4-113">**Element**</span></span>|<span data-ttu-id="d1cf4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d1cf4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d1cf4-115">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="d1cf4-115">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="d1cf4-116">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="d1cf4-116">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="d1cf4-117">Folder</span><span class="sxs-lookup"><span data-stu-id="d1cf4-117">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="d1cf4-118">メールボックス内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="d1cf4-118">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d1cf4-119">ModifiedEvent</span><span class="sxs-lookup"><span data-stu-id="d1cf4-119">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="d1cf4-120">アイテムまたはフォルダーが変更されたイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="d1cf4-120">Represents an event where an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="d1cf4-121">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="d1cf4-121">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="d1cf4-122">メールボックス内の検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="d1cf4-122">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="d1cf4-123">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="d1cf4-123">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="d1cf4-124">メールボックス内のタスク フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="d1cf4-124">Represents a task folder in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d1cf4-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d1cf4-125">Text value</span></span>

<span data-ttu-id="d1cf4-126">テキスト値は、整数値を表します。</span><span class="sxs-lookup"><span data-stu-id="d1cf4-126">The text value represents an integer value.</span></span> <span data-ttu-id="d1cf4-127">このプロパティは値の取得のみ可能です。</span><span class="sxs-lookup"><span data-stu-id="d1cf4-127">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d1cf4-128">備考</span><span class="sxs-lookup"><span data-stu-id="d1cf4-128">Remarks</span></span>

<span data-ttu-id="d1cf4-129">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d1cf4-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d1cf4-130">要素情報</span><span class="sxs-lookup"><span data-stu-id="d1cf4-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d1cf4-131">名前空間</span><span class="sxs-lookup"><span data-stu-id="d1cf4-131">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d1cf4-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d1cf4-132">Schema Name</span></span>  <br/> |<span data-ttu-id="d1cf4-133">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d1cf4-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="d1cf4-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d1cf4-134">Validation File</span></span>  <br/> |<span data-ttu-id="d1cf4-135">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d1cf4-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d1cf4-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d1cf4-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="d1cf4-137">False</span><span class="sxs-lookup"><span data-stu-id="d1cf4-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d1cf4-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="d1cf4-138">See also</span></span>



- [<span data-ttu-id="d1cf4-139">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d1cf4-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

