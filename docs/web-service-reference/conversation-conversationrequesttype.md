---
title: 会話 (ConversationRequestType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0308b71c-d4ff-44a8-b9ca-d5965291ee1d
description: テーマ要素は、GetConversationItems 応答で返される 1 つのテーマを表します。
ms.openlocfilehash: ef56e26fda7d2bf6556069355918aa576ce14cb6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759746"
---
# <a name="conversation-conversationrequesttype"></a><span data-ttu-id="16d11-103">会話 (ConversationRequestType)</span><span class="sxs-lookup"><span data-stu-id="16d11-103">Conversation (ConversationRequestType)</span></span>

<span data-ttu-id="16d11-104">**テーマ**要素は、 **GetConversationItems**応答で返される 1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="16d11-104">The **Conversation** element represents a single conversation returned in a **GetConversationItems** response.</span></span> 
  
```XML
<Conversation>
   <ConversationId/>
   <SyncState/>
</Conversation>
```

 ****
## <a name="attributes-and-elements"></a><span data-ttu-id="16d11-105">属性および要素</span><span class="sxs-lookup"><span data-stu-id="16d11-105">Attributes and elements</span></span>

<span data-ttu-id="16d11-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="16d11-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="16d11-107">属性</span><span class="sxs-lookup"><span data-stu-id="16d11-107">Attributes</span></span>

<span data-ttu-id="16d11-108">なし。</span><span class="sxs-lookup"><span data-stu-id="16d11-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="16d11-109">子要素</span><span class="sxs-lookup"><span data-stu-id="16d11-109">Child elements</span></span>

<span data-ttu-id="16d11-110">[ConversationId](conversationid.md) | [同期状態 (base64Binary)](syncstate-base64binary.md)</span><span class="sxs-lookup"><span data-stu-id="16d11-110">[ConversationId](conversationid.md) | [SyncState (base64Binary)](syncstate-base64binary.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="16d11-111">親要素</span><span class="sxs-lookup"><span data-stu-id="16d11-111">Parent elements</span></span>

[<span data-ttu-id="16d11-112">スレッド</span><span class="sxs-lookup"><span data-stu-id="16d11-112">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
## <a name="remarks"></a><span data-ttu-id="16d11-113">備考</span><span class="sxs-lookup"><span data-stu-id="16d11-113">Remarks</span></span>

<span data-ttu-id="16d11-114">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="16d11-114">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="16d11-115">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="16d11-115">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="16d11-116">要素情報</span><span class="sxs-lookup"><span data-stu-id="16d11-116">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="16d11-117">名前空間</span><span class="sxs-lookup"><span data-stu-id="16d11-117">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="16d11-118">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="16d11-118">Schema name</span></span>  <br/> |<span data-ttu-id="16d11-119">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="16d11-119">Types schema</span></span>  <br/> |
|<span data-ttu-id="16d11-120">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="16d11-120">Validation file</span></span>  <br/> |<span data-ttu-id="16d11-121">types.xsd</span><span class="sxs-lookup"><span data-stu-id="16d11-121">types.xsd</span></span>  <br/> |
|<span data-ttu-id="16d11-122">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="16d11-122">Can be empty</span></span>  <br/> |<span data-ttu-id="16d11-123">false</span><span class="sxs-lookup"><span data-stu-id="16d11-123">false</span></span>  <br/> |
   

