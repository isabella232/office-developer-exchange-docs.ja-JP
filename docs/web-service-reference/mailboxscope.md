---
title: MailboxScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: MailboxScope 要素は、会話の検索またはフェッチがプライマリメールボックス、アーカイブメールボックス、またはプライマリメールボックスとアーカイブメールボックスのいずれかにまたがる必要があるかどうかを識別します。
ms.openlocfilehash: 92823c06d4fe186917c3cfb532eda821bd6a95a7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455374"
---
# <a name="mailboxscope"></a><span data-ttu-id="fec00-103">MailboxScope</span><span class="sxs-lookup"><span data-stu-id="fec00-103">MailboxScope</span></span>

<span data-ttu-id="fec00-104">**MailboxScope**要素は、会話の検索またはフェッチがプライマリメールボックス、アーカイブメールボックス、またはプライマリメールボックスとアーカイブメールボックスのいずれかにまたがる必要があるかどうかを識別します。</span><span class="sxs-lookup"><span data-stu-id="fec00-104">The **MailboxScope** element identifies whether a search or fetch for a conversation should span either the primary mailbox, archive mailbox, or both the primary and archive mailbox.</span></span> 
  
```XML
<MailboxScope> PrimaryOnly | ArchiveOnly | All </MailboxScope>
```

<span data-ttu-id="fec00-105">**MailboxSearchLocationType**</span><span class="sxs-lookup"><span data-stu-id="fec00-105">**MailboxSearchLocationType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="fec00-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fec00-106">Attributes and elements</span></span>

<span data-ttu-id="fec00-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fec00-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fec00-108">属性</span><span class="sxs-lookup"><span data-stu-id="fec00-108">Attributes</span></span>

<span data-ttu-id="fec00-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fec00-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fec00-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fec00-110">Child elements</span></span>

<span data-ttu-id="fec00-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fec00-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fec00-112">親要素</span><span class="sxs-lookup"><span data-stu-id="fec00-112">Parent elements</span></span>

<span data-ttu-id="fec00-113">[Findconversation](findconversation.md)  | [GetConversationItems](getconversationitems.md)  | [会話 (ConversationType)](conversation-conversationtype.md)</span><span class="sxs-lookup"><span data-stu-id="fec00-113">[FindConversation](findconversation.md) | [GetConversationItems](getconversationitems.md) | [Conversation (ConversationType)](conversation-conversationtype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="fec00-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fec00-114">Text value</span></span>

<span data-ttu-id="fec00-115">**MailboxScope**要素のテキスト値は、プライマリメールボックス、アーカイブメールボックス、またはプライマリメールボックスとアーカイブメールボックスの両方で、会話内のアイテムを検索または取得するためのスコープです。</span><span class="sxs-lookup"><span data-stu-id="fec00-115">The text value of the **MailboxScope** element is the scope for finding or getting items in a conversation across either primary mailboxes, archive mailboxes, or both primary and archive mailboxes.</span></span> <span data-ttu-id="fec00-116">Text 値が**Primaryonly**の場合は、ユーザーのプライマリメールボックスを対象とするスコープを示します。</span><span class="sxs-lookup"><span data-stu-id="fec00-116">A text value of **PrimaryOnly** indicates a scope that targets the primary mailbox for a user.</span></span> <span data-ttu-id="fec00-117">アーカイブのテキスト値は、ユーザーのアーカイブメールボックスを対象とするスコープ**のみ**を示します。</span><span class="sxs-lookup"><span data-stu-id="fec00-117">A text value of **ArchiveOnly** indicates a scope that targets the archive mailbox for a user.</span></span> <span data-ttu-id="fec00-118">Text 値は、プライマリメールボックスとアーカイブメールボックスの両方をターゲットとするスコープ**を示します**。</span><span class="sxs-lookup"><span data-stu-id="fec00-118">A text value of **All** indicates a scope that targets both the primary mailbox and archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fec00-119">注釈</span><span class="sxs-lookup"><span data-stu-id="fec00-119">Remarks</span></span>

<span data-ttu-id="fec00-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fec00-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fec00-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fec00-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fec00-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fec00-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fec00-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="fec00-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fec00-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fec00-124">Schema name</span></span>  <br/> |<span data-ttu-id="fec00-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="fec00-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="fec00-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fec00-126">Validation file</span></span>  <br/> |<span data-ttu-id="fec00-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="fec00-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fec00-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fec00-128">Can be empty</span></span>  <br/> |<span data-ttu-id="fec00-129">false</span><span class="sxs-lookup"><span data-stu-id="fec00-129">false</span></span>  <br/> |
   

