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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760664"
---
# <a name="getconversationitems"></a><span data-ttu-id="299a9-103">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="299a9-103">GetConversationItems</span></span>

<span data-ttu-id="299a9-104">**GetConversationItems**要素は、同じスレッドであることによって関連付けられている項目のセットを取得する要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="299a9-104">The **GetConversationItems** element defines a request to get a set of items that are related by being in the same conversation.</span></span> 
  
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

 <span data-ttu-id="299a9-105">**GetConversationItemsType**</span><span class="sxs-lookup"><span data-stu-id="299a9-105">**GetConversationItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="299a9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="299a9-106">Attributes and elements</span></span>

<span data-ttu-id="299a9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="299a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="299a9-108">属性</span><span class="sxs-lookup"><span data-stu-id="299a9-108">Attributes</span></span>

<span data-ttu-id="299a9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="299a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="299a9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="299a9-110">Child elements</span></span>

<span data-ttu-id="299a9-111">[ItemShape](itemshape.md) | [FoldersToIgnore](folderstoignore.md) | [MaxItemsToReturn](maxitemstoreturn.md) | [ソート順序 (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md) | [MailboxScope](mailboxscope.md) | [会話](conversations-ex15websvcsotherref.md)</span><span class="sxs-lookup"><span data-stu-id="299a9-111">[ItemShape](itemshape.md) | [FoldersToIgnore](folderstoignore.md) | [MaxItemsToReturn](maxitemstoreturn.md) | [SortOrder (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md) | [MailboxScope](mailboxscope.md) | [Conversations](conversations-ex15websvcsotherref.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="299a9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="299a9-112">Parent elements</span></span>

<span data-ttu-id="299a9-113">なし。</span><span class="sxs-lookup"><span data-stu-id="299a9-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="299a9-114">備考</span><span class="sxs-lookup"><span data-stu-id="299a9-114">Remarks</span></span>

<span data-ttu-id="299a9-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="299a9-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="299a9-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="299a9-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="299a9-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="299a9-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="299a9-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="299a9-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="299a9-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="299a9-119">Schema name</span></span>  <br/> |<span data-ttu-id="299a9-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="299a9-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="299a9-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="299a9-121">Validation file</span></span>  <br/> |<span data-ttu-id="299a9-122">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="299a9-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="299a9-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="299a9-123">Can be empty</span></span>  <br/> |<span data-ttu-id="299a9-124">false</span><span class="sxs-lookup"><span data-stu-id="299a9-124">false</span></span>  <br/> |
   

