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
ms.openlocfilehash: 72e5d47eac7618408e46ad11eb19eaebf9835502
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467222"
---
# <a name="unreadcount"></a><span data-ttu-id="0e552-103">UnreadCount</span><span class="sxs-lookup"><span data-stu-id="0e552-103">UnreadCount</span></span>

<span data-ttu-id="0e552-104">**UnreadCount**要素には、フォルダー内の未読アイテムの数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0e552-104">The **UnreadCount** element contains the count of unread items within a folder.</span></span> 
  
```XML
<UnreadCount/>
```

 <span data-ttu-id="0e552-105">**xs: int**</span><span class="sxs-lookup"><span data-stu-id="0e552-105">**xs:int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0e552-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0e552-106">Attributes and elements</span></span>

<span data-ttu-id="0e552-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0e552-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0e552-108">属性</span><span class="sxs-lookup"><span data-stu-id="0e552-108">Attributes</span></span>

<span data-ttu-id="0e552-109">なし。</span><span class="sxs-lookup"><span data-stu-id="0e552-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0e552-110">子要素</span><span class="sxs-lookup"><span data-stu-id="0e552-110">Child elements</span></span>

<span data-ttu-id="0e552-111">なし。</span><span class="sxs-lookup"><span data-stu-id="0e552-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="0e552-112">親要素</span><span class="sxs-lookup"><span data-stu-id="0e552-112">Parent elements</span></span>

|<span data-ttu-id="0e552-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="0e552-113">**Element**</span></span>|<span data-ttu-id="0e552-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="0e552-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0e552-115">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="0e552-115">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="0e552-116">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="0e552-116">Represents a single conversation.</span></span>  <br/> |
|[<span data-ttu-id="0e552-117">Folder</span><span class="sxs-lookup"><span data-stu-id="0e552-117">Folder</span></span>](folder.md) <br/> |<span data-ttu-id="0e552-118">メールボックス内のフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="0e552-118">Represents a folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0e552-119">対する modifiedevent</span><span class="sxs-lookup"><span data-stu-id="0e552-119">ModifiedEvent</span></span>](modifiedevent.md) <br/> |<span data-ttu-id="0e552-120">アイテムまたはフォルダーが変更されるイベントを表します。</span><span class="sxs-lookup"><span data-stu-id="0e552-120">Represents an event where an item or folder is modified.</span></span>  <br/> |
|[<span data-ttu-id="0e552-121">SearchFolder</span><span class="sxs-lookup"><span data-stu-id="0e552-121">SearchFolder</span></span>](searchfolder.md) <br/> |<span data-ttu-id="0e552-122">メールボックス内の検索フォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="0e552-122">Represents a search folder in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="0e552-123">TasksFolder</span><span class="sxs-lookup"><span data-stu-id="0e552-123">TasksFolder</span></span>](tasksfolder.md) <br/> |<span data-ttu-id="0e552-124">メールボックス内のタスクフォルダーを表します。</span><span class="sxs-lookup"><span data-stu-id="0e552-124">Represents a task folder in a mailbox.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="0e552-125">テキスト値</span><span class="sxs-lookup"><span data-stu-id="0e552-125">Text value</span></span>

<span data-ttu-id="0e552-126">テキスト値は、整数値を表します。</span><span class="sxs-lookup"><span data-stu-id="0e552-126">The text value represents an integer value.</span></span> <span data-ttu-id="0e552-127">このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。</span><span class="sxs-lookup"><span data-stu-id="0e552-127">This property is read-only.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="0e552-128">注釈</span><span class="sxs-lookup"><span data-stu-id="0e552-128">Remarks</span></span>

<span data-ttu-id="0e552-129">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0e552-129">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0e552-130">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0e552-130">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0e552-131">Namespace</span><span class="sxs-lookup"><span data-stu-id="0e552-131">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="0e552-132">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0e552-132">Schema Name</span></span>  <br/> |<span data-ttu-id="0e552-133">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="0e552-133">Types schema</span></span>  <br/> |
|<span data-ttu-id="0e552-134">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0e552-134">Validation File</span></span>  <br/> |<span data-ttu-id="0e552-135">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="0e552-135">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="0e552-136">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0e552-136">Can be Empty</span></span>  <br/> |<span data-ttu-id="0e552-137">正しくない</span><span class="sxs-lookup"><span data-stu-id="0e552-137">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0e552-138">関連項目</span><span class="sxs-lookup"><span data-stu-id="0e552-138">See also</span></span>



- [<span data-ttu-id="0e552-139">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0e552-139">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

