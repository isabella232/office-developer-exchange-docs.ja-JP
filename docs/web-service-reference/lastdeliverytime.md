---
title: LastDeliveryTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- LastDeliveryTime
api_type:
- schema
ms.assetid: 23d02ceb-f28e-40f2-8f63-673723a50e2a
description: LastDeliveryTime 要素には、現在の会話で最後に受信したメッセージの配信時刻が現在のフォルダーに含まれています。
ms.openlocfilehash: 77147693a9394e983575afa6fcfda242f8f76ae3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458111"
---
# <a name="lastdeliverytime"></a><span data-ttu-id="08226-103">LastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="08226-103">LastDeliveryTime</span></span>

<span data-ttu-id="08226-104">**Lastdeliverytime**要素には、現在の会話で最後に受信したメッセージの配信時刻が現在のフォルダーに含まれています。</span><span class="sxs-lookup"><span data-stu-id="08226-104">The **LastDeliveryTime** element contains the delivery time of the message that was last received in this conversation in the current folder.</span></span> 
  
[<span data-ttu-id="08226-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="08226-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="08226-106">会話</span><span class="sxs-lookup"><span data-stu-id="08226-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="08226-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="08226-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="08226-108">LastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="08226-108">LastDeliveryTime</span></span>](lastdeliverytime.md)
  
```XML
<LastDeliveryTime/>
```

 <span data-ttu-id="08226-109">**xs: dateTime**</span><span class="sxs-lookup"><span data-stu-id="08226-109">**xs:dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08226-110">属性と要素</span><span class="sxs-lookup"><span data-stu-id="08226-110">Attributes and elements</span></span>

<span data-ttu-id="08226-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="08226-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08226-112">属性</span><span class="sxs-lookup"><span data-stu-id="08226-112">Attributes</span></span>

<span data-ttu-id="08226-113">なし。</span><span class="sxs-lookup"><span data-stu-id="08226-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08226-114">子要素</span><span class="sxs-lookup"><span data-stu-id="08226-114">Child elements</span></span>

<span data-ttu-id="08226-115">なし。</span><span class="sxs-lookup"><span data-stu-id="08226-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="08226-116">親要素</span><span class="sxs-lookup"><span data-stu-id="08226-116">Parent elements</span></span>

|<span data-ttu-id="08226-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="08226-117">**Element**</span></span>|<span data-ttu-id="08226-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="08226-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08226-119">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="08226-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="08226-120">単一の会話を表します。</span><span class="sxs-lookup"><span data-stu-id="08226-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="08226-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="08226-121">Text value</span></span>

<span data-ttu-id="08226-122">**Lastdeliverytime**要素のテキスト値は、現在のフォルダーでこのスレッドで最後に受信されたメッセージの日時です。</span><span class="sxs-lookup"><span data-stu-id="08226-122">The text value of the **LastDeliveryTime** element is the date and time of the message that was last received in this conversation in the current folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="08226-123">注釈</span><span class="sxs-lookup"><span data-stu-id="08226-123">Remarks</span></span>

<span data-ttu-id="08226-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="08226-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08226-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="08226-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08226-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="08226-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="08226-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="08226-127">Schema name</span></span>  <br/> |<span data-ttu-id="08226-128">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="08226-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="08226-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="08226-129">Validation file</span></span>  <br/> |<span data-ttu-id="08226-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="08226-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="08226-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="08226-131">Can be empty</span></span>  <br/> |<span data-ttu-id="08226-132">正しくない</span><span class="sxs-lookup"><span data-stu-id="08226-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08226-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="08226-133">See also</span></span>



[<span data-ttu-id="08226-134">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="08226-134">FindConversation operation</span></span>](findconversation-operation.md)
  
[<span data-ttu-id="08226-135">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="08226-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="08226-136">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="08226-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="08226-137">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="08226-137">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

