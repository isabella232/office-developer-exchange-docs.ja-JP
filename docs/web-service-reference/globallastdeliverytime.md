---
title: GlobalLastDeliveryTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GlobalLastDeliveryTime
api_type:
- schema
ms.assetid: a88dada9-c527-43a7-b2d3-31aad330def9
description: GlobalLastDeliveryTime 要素には、メールボックス内のすべてのフォルダー間でこの会話の最後に受信したメッセージの配信時刻が含まれています。
ms.openlocfilehash: fded5cd1891a406f0979cf4bec7321779d70ab3a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831733"
---
# <a name="globallastdeliverytime"></a><span data-ttu-id="7b3b1-103">GlobalLastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="7b3b1-103">GlobalLastDeliveryTime</span></span>

<span data-ttu-id="7b3b1-104">**GlobalLastDeliveryTime**要素には、メールボックス内のすべてのフォルダー間でこの会話の最後に受信したメッセージの配信時刻が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7b3b1-104">The **GlobalLastDeliveryTime** element contains the delivery time of the message that was last received in this conversation across all folders in the mailbox.</span></span> 
  
[<span data-ttu-id="7b3b1-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="7b3b1-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
[<span data-ttu-id="7b3b1-106">スレッド</span><span class="sxs-lookup"><span data-stu-id="7b3b1-106">Conversations</span></span>](conversations-ex15websvcsotherref.md)
  
[<span data-ttu-id="7b3b1-107">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="7b3b1-107">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
[<span data-ttu-id="7b3b1-108">GlobalLastDeliveryTime</span><span class="sxs-lookup"><span data-stu-id="7b3b1-108">GlobalLastDeliveryTime</span></span>](globallastdeliverytime.md)
  
```XML
<GlobalLastDeliveryTime/>
```

 <span data-ttu-id="7b3b1-109">**xs:dateTime**</span><span class="sxs-lookup"><span data-stu-id="7b3b1-109">**xs:dateTime**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7b3b1-110">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7b3b1-110">Attributes and elements</span></span>

<span data-ttu-id="7b3b1-111">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7b3b1-111">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7b3b1-112">属性</span><span class="sxs-lookup"><span data-stu-id="7b3b1-112">Attributes</span></span>

<span data-ttu-id="7b3b1-113">なし。</span><span class="sxs-lookup"><span data-stu-id="7b3b1-113">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7b3b1-114">子要素</span><span class="sxs-lookup"><span data-stu-id="7b3b1-114">Child elements</span></span>

<span data-ttu-id="7b3b1-115">なし。</span><span class="sxs-lookup"><span data-stu-id="7b3b1-115">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7b3b1-116">親要素</span><span class="sxs-lookup"><span data-stu-id="7b3b1-116">Parent elements</span></span>

|<span data-ttu-id="7b3b1-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="7b3b1-117">**Element**</span></span>|<span data-ttu-id="7b3b1-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="7b3b1-118">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7b3b1-119">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="7b3b1-119">Conversation (ConversationType)</span></span>](conversation-conversationtype.md) <br/> |<span data-ttu-id="7b3b1-120">1 つのテーマを表します。</span><span class="sxs-lookup"><span data-stu-id="7b3b1-120">Represents a single conversation.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7b3b1-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7b3b1-121">Text value</span></span>

<span data-ttu-id="7b3b1-122">**GlobalLastDeliveryTime**要素のテキスト値とは、メッセージ、メールボックス内のすべてのフォルダーをこの会話に受信した最後の日時です。</span><span class="sxs-lookup"><span data-stu-id="7b3b1-122">The text value of the **GlobalLastDeliveryTime** element is the date and time of the message that was last received in this conversation across all folders in the mailbox.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="7b3b1-123">備考</span><span class="sxs-lookup"><span data-stu-id="7b3b1-123">Remarks</span></span>

<span data-ttu-id="7b3b1-124">この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7b3b1-124">This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7b3b1-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="7b3b1-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7b3b1-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="7b3b1-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7b3b1-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7b3b1-127">Schema name</span></span>  <br/> |<span data-ttu-id="7b3b1-128">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7b3b1-128">Types schema</span></span>  <br/> |
|<span data-ttu-id="7b3b1-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7b3b1-129">Validation file</span></span>  <br/> |<span data-ttu-id="7b3b1-130">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7b3b1-130">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7b3b1-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7b3b1-131">Can be empty</span></span>  <br/> |<span data-ttu-id="7b3b1-132">False</span><span class="sxs-lookup"><span data-stu-id="7b3b1-132">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7b3b1-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="7b3b1-133">See also</span></span>



<span data-ttu-id="7b3b1-134">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="7b3b1-134">[FindConversation operation](findconversation-operation.md)</span></span>
  
[<span data-ttu-id="7b3b1-135">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="7b3b1-135">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)


[<span data-ttu-id="7b3b1-136">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="7b3b1-136">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

