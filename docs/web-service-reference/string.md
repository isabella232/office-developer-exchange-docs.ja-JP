---
title: String
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- String
api_type:
- schema
ms.assetid: e6e362b1-4526-49e1-b283-1c4bc4295874
description: 文字列要素は、項目、連絡先、タスク、および会話で使用される文字列を表します。
ms.openlocfilehash: 66260c7ebcb56049a78c5eddbe057dfa8d61f193
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833607"
---
# <a name="string"></a><span data-ttu-id="15d04-103">String</span><span class="sxs-lookup"><span data-stu-id="15d04-103">String</span></span>

<span data-ttu-id="15d04-104">**文字列**要素は、項目、連絡先、タスク、および会話で使用される文字列を表します。</span><span class="sxs-lookup"><span data-stu-id="15d04-104">The **String** element represents a string that is used by items, contacts, tasks, and conversations.</span></span> 
  
```XML
<String/>
```

 <span data-ttu-id="15d04-105">**string**</span><span class="sxs-lookup"><span data-stu-id="15d04-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="15d04-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="15d04-106">Attributes and elements</span></span>

<span data-ttu-id="15d04-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="15d04-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="15d04-108">属性</span><span class="sxs-lookup"><span data-stu-id="15d04-108">Attributes</span></span>

<span data-ttu-id="15d04-109">なし。</span><span class="sxs-lookup"><span data-stu-id="15d04-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="15d04-110">子要素</span><span class="sxs-lookup"><span data-stu-id="15d04-110">Child elements</span></span>

<span data-ttu-id="15d04-111">なし。</span><span class="sxs-lookup"><span data-stu-id="15d04-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="15d04-112">親要素</span><span class="sxs-lookup"><span data-stu-id="15d04-112">Parent elements</span></span>

|<span data-ttu-id="15d04-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="15d04-113">**Element**</span></span>|<span data-ttu-id="15d04-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="15d04-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="15d04-115">Categories</span><span class="sxs-lookup"><span data-stu-id="15d04-115">Categories</span></span>](categories-ex15websvcsotherref.md) <br/> |<span data-ttu-id="15d04-116">メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="15d04-116">Contains a collection of strings that identify to which categories an item in the mailbox belongs.</span></span>  <br/> |
|[<span data-ttu-id="15d04-117">Children</span><span class="sxs-lookup"><span data-stu-id="15d04-117">Children</span></span>](children.md) <br/> |<span data-ttu-id="15d04-118">連絡先の子供の名前が含まれています。</span><span class="sxs-lookup"><span data-stu-id="15d04-118">Contains the names of the children of a contact.</span></span>  <br/> |
|[<span data-ttu-id="15d04-119">Companies</span><span class="sxs-lookup"><span data-stu-id="15d04-119">Companies</span></span>](companies.md) <br/> |<span data-ttu-id="15d04-120">連絡先またはタスクに関連付けられている企業のコレクションを表します。</span><span class="sxs-lookup"><span data-stu-id="15d04-120">Represents the collection of companies that are associated with a contact or task.</span></span>  <br/> |
|[<span data-ttu-id="15d04-121">連絡先</span><span class="sxs-lookup"><span data-stu-id="15d04-121">Contacts</span></span>](contacts-ex15websvcsotherref.md) <br/> |<span data-ttu-id="15d04-122">タスクに関連付けられている連絡先の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="15d04-122">Contains a list of contacts that are associated with a task.</span></span>  <br/> |
|[<span data-ttu-id="15d04-123">GlobalCategories</span><span class="sxs-lookup"><span data-stu-id="15d04-123">GlobalCategories</span></span>](globalcategories.md) <br/> |<span data-ttu-id="15d04-124">メールボックス内のすべての会話項目のカテゴリの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="15d04-124">Contains the category list for all conversation items in a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="15d04-125">GlobalUniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="15d04-125">GlobalUniqueRecipients</span></span>](globaluniquerecipients.md) <br/> |<span data-ttu-id="15d04-126">メールボックス間で集計する対話の受信者のリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="15d04-126">Contains the recipient list of a conversation aggregated across a mailbox.</span></span>  <br/> |
|[<span data-ttu-id="15d04-127">GlobalUniqueSenders</span><span class="sxs-lookup"><span data-stu-id="15d04-127">GlobalUniqueSenders</span></span>](globaluniquesenders.md) <br/> |<span data-ttu-id="15d04-128">メールボックス内のアイテムの会話のすべての送信者の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="15d04-128">Contains a list of all the senders of conversation items in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="15d04-129">GlobalUniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="15d04-129">GlobalUniqueUnreadSenders</span></span>](globaluniqueunreadsenders.md) <br/> |<span data-ttu-id="15d04-130">現在この会話で、メールボックス内のすべてのフォルダー間でメッセージを送信したすべての人のリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="15d04-130">Contains a list of all the people who have sent messages that are currently unread in this conversation across all folders in the mailbox.</span></span>  <br/> |
|[<span data-ttu-id="15d04-131">ItemClasses</span><span class="sxs-lookup"><span data-stu-id="15d04-131">ItemClasses</span></span>](itemclasses.md) <br/> |<span data-ttu-id="15d04-132">項目のクラスに適用する条件または例外の順序で受信したメッセージにスタンプする必要がありますの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="15d04-132">Contains a list of the item classes that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="15d04-133">MessageClassifications</span><span class="sxs-lookup"><span data-stu-id="15d04-133">MessageClassifications</span></span>](messageclassifications.md) <br/> |<span data-ttu-id="15d04-134">適用する場合の条件または例外の順序で受信したメッセージにスタンプする必要がありますメッセージの分類の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="15d04-134">Contains a list of the message classifications that must be stamped on incoming messages in order for the condition or exception to apply.</span></span>  <br/> |
|[<span data-ttu-id="15d04-135">UniqueRecipients</span><span class="sxs-lookup"><span data-stu-id="15d04-135">UniqueRecipients</span></span>](uniquerecipients.md) <br/> |<span data-ttu-id="15d04-136">会話の受信者の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="15d04-136">Contains the list of recipients of the conversation.</span></span> <span data-ttu-id="15d04-137">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="15d04-137">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="15d04-138">UniqueSenders</span><span class="sxs-lookup"><span data-stu-id="15d04-138">UniqueSenders</span></span>](uniquesenders.md) <br/> |<span data-ttu-id="15d04-139">会話項目を現在のフォルダー内のすべての送信者の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="15d04-139">Contains a list of all the senders of conversation items in the current folder.</span></span> <span data-ttu-id="15d04-140">この要素は、読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="15d04-140">This element is read-only.</span></span>  <br/> |
|[<span data-ttu-id="15d04-141">UniqueUnreadSenders</span><span class="sxs-lookup"><span data-stu-id="15d04-141">UniqueUnreadSenders</span></span>](uniqueunreadsenders.md) <br/> |<span data-ttu-id="15d04-142">現在この会話を [現在のフォルダーにメッセージを送信したすべての人のリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="15d04-142">Contains a list of all the people who have sent messages that are currently unread in this conversation in the current folder.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="15d04-143">テキスト値</span><span class="sxs-lookup"><span data-stu-id="15d04-143">Text value</span></span>

<span data-ttu-id="15d04-144">この要素のテキスト値は、連絡先、会社、会話、またはタスクに関連付けられている連絡先の一意の受信者の子カテゴリを表す文字列です。</span><span class="sxs-lookup"><span data-stu-id="15d04-144">The text value of this element is a string that represents a category, the child of a contact, a company, a unique recipient of a conversation, or a contact that is associated with a task.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="15d04-145">備考</span><span class="sxs-lookup"><span data-stu-id="15d04-145">Remarks</span></span>

<span data-ttu-id="15d04-146">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="15d04-146">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="15d04-147">要素情報</span><span class="sxs-lookup"><span data-stu-id="15d04-147">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="15d04-148">名前空間</span><span class="sxs-lookup"><span data-stu-id="15d04-148">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="15d04-149">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="15d04-149">Schema Name</span></span>  <br/> |<span data-ttu-id="15d04-150">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="15d04-150">Types schema</span></span>  <br/> |
|<span data-ttu-id="15d04-151">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="15d04-151">Validation File</span></span>  <br/> |<span data-ttu-id="15d04-152">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="15d04-152">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="15d04-153">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="15d04-153">Can be Empty</span></span>  <br/> |<span data-ttu-id="15d04-154">False</span><span class="sxs-lookup"><span data-stu-id="15d04-154">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="15d04-155">関連項目</span><span class="sxs-lookup"><span data-stu-id="15d04-155">See also</span></span>



<span data-ttu-id="15d04-156">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="15d04-156">[FindConversation operation](findconversation-operation.md)</span></span>


- [<span data-ttu-id="15d04-157">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="15d04-157">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

