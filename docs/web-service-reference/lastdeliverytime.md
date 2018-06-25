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
description: LastDeliveryTime 要素には、現在のフォルダーには、この会話の最後に受信したメッセージの配信時刻が含まれています。
ms.openlocfilehash: 240f6acaf3e5249686ab26501a26ee3e0f337b0f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832198"
---
# <a name="lastdeliverytime"></a><span data-ttu-id="2d531-103">LastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="2d531-103">LastDeliveryTime</span></span>

<span data-ttu-id="2d531-104">**LastDeliveryTime**要素には、現在のフォルダーには、この会話の最後に受信したメッセージの配信時刻が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2d531-104">The **LastDeliveryTime** element contains the delivery time of the message that was last received in this conversation in the current folder.</span></span> 
  
[<span data-ttu-id="2d531-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="2d531-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="2d531-106">スレッド</span><span class="sxs-lookup"><span data-stu-id="2d531-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="2d531-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="2d531-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="2d531-108">LastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="2d531-108">LastDeliveryTime</span></span>](lastdeliverytime.md)
  
```XML
<LastDeliveryTime/>
```

 <span data-ttu-id="2d531-109">**xs:dateTime**</span><span class="sxs-lookup"><span data-stu-id="2d531-109">**xs:dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2d531-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2d531-110">Attributes and elements</span></span>

<span data-ttu-id="2d531-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2d531-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2d531-112">属性</span><span class="sxs-lookup"><span data-stu-id="2d531-112">Attributes</span></span>

<span data-ttu-id="2d531-113">なし。</span><span class="sxs-lookup"><span data-stu-id="2d531-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2d531-114">子要素</span><span class="sxs-lookup"><span data-stu-id="2d531-114">Child elements</span></span>

<span data-ttu-id="2d531-115">なし。</span><span class="sxs-lookup"><span data-stu-id="2d531-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2d531-116">親要素</span><span class="sxs-lookup"><span data-stu-id="2d531-116">Parent elements</span></span>

|<span data-ttu-id="2d531-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="2d531-117">**Element**</span></span>|<span data-ttu-id="2d531-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="2d531-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2d531-119">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="2d531-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="2d531-120">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="2d531-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2d531-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2d531-121">Text value</span></span>

<span data-ttu-id="2d531-122">**LastDeliveryTime**要素のテキスト値とは、現在のフォルダーには、この会話の最後に受信したメッセージの日時です。</span><span class="sxs-lookup"><span data-stu-id="2d531-122">The text value of the **LastDeliveryTime** element is the date and time of the message that was last received in this conversation in the current folder.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2d531-123">備考</span><span class="sxs-lookup"><span data-stu-id="2d531-123">Remarks</span></span>

<span data-ttu-id="2d531-124">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2d531-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2d531-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="2d531-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2d531-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="2d531-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2d531-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2d531-127">Schema name</span></span>  <br/> |<span data-ttu-id="2d531-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="2d531-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="2d531-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2d531-129">Validation file</span></span>  <br/> |<span data-ttu-id="2d531-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2d531-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2d531-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2d531-131">Can be empty</span></span>  <br/> |<span data-ttu-id="2d531-132">False</span><span class="sxs-lookup"><span data-stu-id="2d531-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2d531-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="2d531-133">See also</span></span>



<span data-ttu-id="2d531-134">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="2d531-134">[FindConversation operation](findconversation-operation.md)</span></span>
  
[<span data-ttu-id="2d531-135">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="2d531-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


- [<span data-ttu-id="2d531-136">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2d531-136">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)


[<span data-ttu-id="2d531-137">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="2d531-137">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

