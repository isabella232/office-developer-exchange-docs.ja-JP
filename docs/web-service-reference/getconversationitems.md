---
title: GetConversationItems
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 4f7bcd0f-140c-4cbc-a5ed-daeffded1df1
description: GetConversationItems 要素は、同じ会話に含まれているアイテムのセットを取得するための要求を定義します。
ms.openlocfilehash: cde4bc2c39ccbc51b7436c87c4bc06e3b8d7e52c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457747"
---
# <a name="getconversationitems"></a><span data-ttu-id="72822-103">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="72822-103">GetConversationItems</span></span>

<span data-ttu-id="72822-104">**GetConversationItems**要素は、同じ会話に含まれているアイテムのセットを取得するための要求を定義します。</span><span class="sxs-lookup"><span data-stu-id="72822-104">The **GetConversationItems** element defines a request to get a set of items that are related by being in the same conversation.</span></span> 
  
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

 <span data-ttu-id="72822-105">**GetConversationItemsType**</span><span class="sxs-lookup"><span data-stu-id="72822-105">**GetConversationItemsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="72822-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="72822-106">Attributes and elements</span></span>

<span data-ttu-id="72822-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="72822-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="72822-108">属性</span><span class="sxs-lookup"><span data-stu-id="72822-108">Attributes</span></span>

<span data-ttu-id="72822-109">なし。</span><span class="sxs-lookup"><span data-stu-id="72822-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="72822-110">子要素</span><span class="sxs-lookup"><span data-stu-id="72822-110">Child elements</span></span>

<span data-ttu-id="72822-111">[Itemshape](itemshape.md)  | [Folderstoignore](folderstoignore.md)  | [Maxitemstoreturn](maxitemstoreturn.md)  | [ソート順序 (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md)  | [MailboxScope](mailboxscope.md)  | [会話](conversations-ex15websvcsotherref.md)</span><span class="sxs-lookup"><span data-stu-id="72822-111">[ItemShape](itemshape.md) | [FoldersToIgnore](folderstoignore.md) | [MaxItemsToReturn](maxitemstoreturn.md) | [SortOrder (ConversationNodeSortOrder)](sortorder-conversationnodesortorder.md) | [MailboxScope](mailboxscope.md) | [Conversations](conversations-ex15websvcsotherref.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="72822-112">親要素</span><span class="sxs-lookup"><span data-stu-id="72822-112">Parent elements</span></span>

<span data-ttu-id="72822-113">なし。</span><span class="sxs-lookup"><span data-stu-id="72822-113">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="72822-114">注釈</span><span class="sxs-lookup"><span data-stu-id="72822-114">Remarks</span></span>

<span data-ttu-id="72822-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="72822-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="72822-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="72822-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="72822-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="72822-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="72822-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="72822-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="72822-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="72822-119">Schema name</span></span>  <br/> |<span data-ttu-id="72822-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="72822-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="72822-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="72822-121">Validation file</span></span>  <br/> |<span data-ttu-id="72822-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="72822-122">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="72822-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="72822-123">Can be empty</span></span>  <br/> |<span data-ttu-id="72822-124">false</span><span class="sxs-lookup"><span data-stu-id="72822-124">false</span></span>  <br/> |
   

