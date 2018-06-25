---
title: GlobalHasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 425272b2-7a4e-4376-aea9-d9b10c1ad6ee
description: GlobalHasIrm 要素は、会話ではすべてのフォルダーの 1 つ以上のメッセージは、IRM で保護されたメッセージかどうかを指定します。
ms.openlocfilehash: ad3eafcb38829e7ea57cbc7535b0f5411ad595d2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831717"
---
# <a name="globalhasirm"></a><span data-ttu-id="4b935-103">GlobalHasIrm</span><span class="sxs-lookup"><span data-stu-id="4b935-103">GlobalHasIrm</span></span>

<span data-ttu-id="4b935-104">**GlobalHasIrm**要素は、会話ではすべてのフォルダーの 1 つ以上のメッセージは、IRM で保護されたメッセージかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="4b935-104">The **GlobalHasIrm** element specifies whether at least one message in the conversation and across all folders is an IRM protected message.</span></span> 
  
```XML
<GlobalHasIrm> true | false </GlobalHasIrm>
```

 <span data-ttu-id="4b935-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="4b935-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4b935-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4b935-106">Attributes and elements</span></span>

<span data-ttu-id="4b935-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4b935-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4b935-108">属性</span><span class="sxs-lookup"><span data-stu-id="4b935-108">Attributes</span></span>

<span data-ttu-id="4b935-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4b935-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4b935-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4b935-110">Child elements</span></span>

<span data-ttu-id="4b935-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4b935-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4b935-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4b935-112">Parent elements</span></span>

[<span data-ttu-id="4b935-113">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="4b935-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="text-value"></a><span data-ttu-id="4b935-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4b935-114">Text value</span></span>

<span data-ttu-id="4b935-115">**会話ではすべてのフォルダーの 1 つ以上のメッセージが IRM で保護されたメッセージの場合、 **GlobalHasIrm**要素のテキスト値は**</span><span class="sxs-lookup"><span data-stu-id="4b935-115">The text value of the **GlobalHasIrm** element is **true** if at least one message in the conversation and across all folders is an IRM protected message.</span></span> <span data-ttu-id="4b935-116">それ以外の場合、値は、 **false**です。</span><span class="sxs-lookup"><span data-stu-id="4b935-116">Otherwise the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4b935-117">備考</span><span class="sxs-lookup"><span data-stu-id="4b935-117">Remarks</span></span>

<span data-ttu-id="4b935-118">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4b935-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="4b935-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4b935-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4b935-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="4b935-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4b935-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="4b935-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4b935-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4b935-122">Schema Name</span></span>  <br/> |<span data-ttu-id="4b935-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="4b935-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="4b935-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4b935-124">Validation File</span></span>  <br/> |<span data-ttu-id="4b935-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="4b935-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="4b935-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4b935-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="4b935-127">True</span><span class="sxs-lookup"><span data-stu-id="4b935-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4b935-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="4b935-128">See also</span></span>



[<span data-ttu-id="4b935-129">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="4b935-129">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)


- [<span data-ttu-id="4b935-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4b935-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

