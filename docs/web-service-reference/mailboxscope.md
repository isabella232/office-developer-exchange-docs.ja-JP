---
title: MailboxScope
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9778823-f290-4827-ba19-5f391ed4f877
description: MailboxScope 要素は、検索、または会話をフェッチする必要があります、プライマリ メールボックス、アーカイブ メールボックス、または両方のプライマリ、メールボックスをアーカイブするかどうかを識別します。
ms.openlocfilehash: 89c9776079d686b114d6b744150f1c6df3711eab
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832293"
---
# <a name="mailboxscope"></a><span data-ttu-id="023ca-103">MailboxScope</span><span class="sxs-lookup"><span data-stu-id="023ca-103">MailboxScope</span></span>

<span data-ttu-id="023ca-104">**MailboxScope**要素は、検索、または会話をフェッチする必要があります、プライマリ メールボックス、アーカイブ メールボックス、または両方のプライマリ、メールボックスをアーカイブするかどうかを識別します。</span><span class="sxs-lookup"><span data-stu-id="023ca-104">The **MailboxScope** element identifies whether a search or fetch for a conversation should span either the primary mailbox, archive mailbox, or both the primary and archive mailbox.</span></span> 
  
```XML
<MailboxScope> PrimaryOnly | ArchiveOnly | All </MailboxScope>
```

<span data-ttu-id="023ca-105">**MailboxSearchLocationType**</span><span class="sxs-lookup"><span data-stu-id="023ca-105">**MailboxSearchLocationType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="023ca-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="023ca-106">Attributes and elements</span></span>

<span data-ttu-id="023ca-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="023ca-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="023ca-108">属性</span><span class="sxs-lookup"><span data-stu-id="023ca-108">Attributes</span></span>

<span data-ttu-id="023ca-109">なし。</span><span class="sxs-lookup"><span data-stu-id="023ca-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="023ca-110">子要素</span><span class="sxs-lookup"><span data-stu-id="023ca-110">Child elements</span></span>

<span data-ttu-id="023ca-111">なし。</span><span class="sxs-lookup"><span data-stu-id="023ca-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="023ca-112">親要素</span><span class="sxs-lookup"><span data-stu-id="023ca-112">Parent elements</span></span>

<span data-ttu-id="023ca-113">[FindConversation](findconversation.md) | [GetConversationItems](getconversationitems.md) | [(ConversationType) の会話](conversation-conversationtype.md)</span><span class="sxs-lookup"><span data-stu-id="023ca-113">[FindConversation](findconversation.md) | [GetConversationItems](getconversationitems.md) | [Conversation (ConversationType)](conversation-conversationtype.md)</span></span>
  
## <a name="text-value"></a><span data-ttu-id="023ca-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="023ca-114">Text value</span></span>

<span data-ttu-id="023ca-115">**MailboxScope**要素のテキスト値は、検索のスコープをまたはいずれかのプライマリ メールボックス間での会話でアーカイブ メールボックス、または両方のプライマリおよびアーカイブ メールボックス アイテムを取得します。</span><span class="sxs-lookup"><span data-stu-id="023ca-115">The text value of the **MailboxScope** element is the scope for finding or getting items in a conversation across either primary mailboxes, archive mailboxes, or both primary and archive mailboxes.</span></span> <span data-ttu-id="023ca-116">**PrimaryOnly**のテキスト値は、ユーザーのプライマリ メールボックスを対象とする範囲を示します。</span><span class="sxs-lookup"><span data-stu-id="023ca-116">A text value of **PrimaryOnly** indicates a scope that targets the primary mailbox for a user.</span></span> <span data-ttu-id="023ca-117">**ArchiveOnly**のテキスト値は、ユーザーのアーカイブ メールボックスを対象とする範囲を示します。</span><span class="sxs-lookup"><span data-stu-id="023ca-117">A text value of **ArchiveOnly** indicates a scope that targets the archive mailbox for a user.</span></span> <span data-ttu-id="023ca-118">**すべて**のテキスト値は、プライマリ メールボックスとアーカイブ メールボックスの両方を対象とする範囲を示します。</span><span class="sxs-lookup"><span data-stu-id="023ca-118">A text value of **All** indicates a scope that targets both the primary mailbox and archive mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="023ca-119">備考</span><span class="sxs-lookup"><span data-stu-id="023ca-119">Remarks</span></span>

<span data-ttu-id="023ca-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="023ca-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="023ca-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="023ca-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="023ca-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="023ca-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="023ca-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="023ca-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="023ca-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="023ca-124">Schema name</span></span>  <br/> |<span data-ttu-id="023ca-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="023ca-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="023ca-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="023ca-126">Validation file</span></span>  <br/> |<span data-ttu-id="023ca-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="023ca-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="023ca-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="023ca-128">Can be empty</span></span>  <br/> |<span data-ttu-id="023ca-129">false</span><span class="sxs-lookup"><span data-stu-id="023ca-129">false</span></span>  <br/> |
   

