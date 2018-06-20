---
title: GetConversationItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4f7bcd0f-140c-4cbc-a5ed-daeffded1df1
description: GetConversationItems 要素は、同じスレッドであることによって関連付けられている項目のセットを取得する要求を定義します。
ms.openlocfilehash: 9be300318a07173e4a8e11e5a6ca78b885de1199
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760664"
---
# <a name="getconversationitems"></a><span data-ttu-id="e8274-103">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="e8274-103">GetConversationItems</span></span>

<span data-ttu-id="e8274-104">**GetConversationItems**要素は、同じスレッドであることによって関連付けられている項目のセットを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="e8274-104">The **GetConversationItems** element defines a request to get a set of items that are related by being in the same conversation.</span></span> 
  
```XML
<GetConversationItems>
   <ItemShape/>
   <FoldersToIgnore/>
   <MaxItemsToReturn/>
   <SortOrder/>
   <MailboxScope/>
   <Conversations/>
</GetConversationItems>
```

 <span data-ttu-id="e8274-105">**GetConversationItemsType**</span><span class="sxs-lookup"><span data-stu-id="e8274-105">**GetConversationItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8274-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e8274-106">Attributes and elements</span></span>

<span data-ttu-id="e8274-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e8274-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8274-108">属性</span><span class="sxs-lookup"><span data-stu-id="e8274-108">Attributes</span></span>

<span data-ttu-id="e8274-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e8274-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8274-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e8274-110">Child elements</span></span>

<span data-ttu-id="e8274-111">[ItemShape](itemshape.md) | [FoldersToIgnore](folderstoignore.md) | [MaxItemsToReturn](maxitemstoreturn.md) | [ソート順序 (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md) | [MailboxScope](mailboxscope.md) | [会話](conversations-ex15websvcsotherref.md)</span><span class="sxs-lookup"><span data-stu-id="e8274-111">[ItemShape](itemshape.md) | [FoldersToIgnore](folderstoignore.md) | [MaxItemsToReturn](maxitemstoreturn.md) | [SortOrder (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md) | [MailboxScope](mailboxscope.md) | [Conversations](conversations-ex15websvcsotherref.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e8274-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e8274-112">Parent elements</span></span>

<span data-ttu-id="e8274-113">なし。</span><span class="sxs-lookup"><span data-stu-id="e8274-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e8274-114">備考</span><span class="sxs-lookup"><span data-stu-id="e8274-114">Remarks</span></span>

<span data-ttu-id="e8274-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e8274-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e8274-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e8274-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8274-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="e8274-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8274-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="e8274-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e8274-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e8274-119">Schema name</span></span>  <br/> |<span data-ttu-id="e8274-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e8274-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e8274-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e8274-121">Validation file</span></span>  <br/> |<span data-ttu-id="e8274-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e8274-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e8274-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e8274-123">Can be empty</span></span>  <br/> |<span data-ttu-id="e8274-124">false</span><span class="sxs-lookup"><span data-stu-id="e8274-124">false</span></span>  <br/> |
   

