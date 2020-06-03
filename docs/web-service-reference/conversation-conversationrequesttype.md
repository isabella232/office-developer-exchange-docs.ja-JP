---
title: 会話 (ConversationRequestType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0308b71c-d4ff-44a8-b9ca-d5965291ee1d
description: 会話要素は、GetConversationItems 応答で返される1つの会話を表します。
ms.openlocfilehash: 925fd6fce83cad36f4a0e95bb6228ba65e4e9c43
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466781"
---
# <a name="conversation-conversationrequesttype"></a><span data-ttu-id="1e9ea-103">会話 (ConversationRequestType)</span><span class="sxs-lookup"><span data-stu-id="1e9ea-103">Conversation (ConversationRequestType)</span></span>

<span data-ttu-id="1e9ea-104">**会話**要素は、 **GetConversationItems**応答で返される1つの会話を表します。</span><span class="sxs-lookup"><span data-stu-id="1e9ea-104">The **Conversation** element represents a single conversation returned in a **GetConversationItems** response.</span></span> 
  
```XML
<Conversation>
   <ConversationId/>
   <SyncState/>
</Conversation>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="1e9ea-105">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1e9ea-105">Attributes and elements</span></span>

<span data-ttu-id="1e9ea-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1e9ea-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1e9ea-107">属性</span><span class="sxs-lookup"><span data-stu-id="1e9ea-107">Attributes</span></span>

<span data-ttu-id="1e9ea-108">なし。</span><span class="sxs-lookup"><span data-stu-id="1e9ea-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1e9ea-109">子要素</span><span class="sxs-lookup"><span data-stu-id="1e9ea-109">Child elements</span></span>

<span data-ttu-id="1e9ea-110">[ConversationId](conversationid.md)  | [Syncstate (base64Binary)](syncstate-base64binary.md)</span><span class="sxs-lookup"><span data-stu-id="1e9ea-110">[ConversationId](conversationid.md) | [SyncState (base64Binary)](syncstate-base64binary.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="1e9ea-111">親要素</span><span class="sxs-lookup"><span data-stu-id="1e9ea-111">Parent elements</span></span>

[<span data-ttu-id="1e9ea-112">会話</span><span class="sxs-lookup"><span data-stu-id="1e9ea-112">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="1e9ea-113">注釈</span><span class="sxs-lookup"><span data-stu-id="1e9ea-113">Remarks</span></span>

<span data-ttu-id="1e9ea-114">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1e9ea-114">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="1e9ea-115">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1e9ea-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1e9ea-116">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1e9ea-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1e9ea-117">Namespace</span><span class="sxs-lookup"><span data-stu-id="1e9ea-117">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="1e9ea-118">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1e9ea-118">Schema name</span></span>  <br/> |<span data-ttu-id="1e9ea-119">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="1e9ea-119">Types schema</span></span>  <br/> |
|<span data-ttu-id="1e9ea-120">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1e9ea-120">Validation file</span></span>  <br/> |<span data-ttu-id="1e9ea-121">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="1e9ea-121">types.xsd</span></span>  <br/> |
|<span data-ttu-id="1e9ea-122">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="1e9ea-122">Can be empty</span></span>  <br/> |<span data-ttu-id="1e9ea-123">false</span><span class="sxs-lookup"><span data-stu-id="1e9ea-123">false</span></span>  <br/> |
   

