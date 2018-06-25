---
title: HasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fedc04e0-cfd2-4652-a2a8-51de859ae847
description: HasIrm 要素は、会話と現在のフォルダー内の 1 つ以上のメッセージが IRM で保護されたメッセージかどうかを指定します。
ms.openlocfilehash: c129370d7920da7cf1f9f32eed2f075e6c21cf8b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831803"
---
# <a name="hasirm"></a><span data-ttu-id="55632-103">HasIrm</span><span class="sxs-lookup"><span data-stu-id="55632-103">HasIrm</span></span>

<span data-ttu-id="55632-104">**HasIrm**要素は、会話と現在のフォルダー内の 1 つ以上のメッセージが IRM で保護されたメッセージかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="55632-104">The **HasIrm** element specifies whether at least one message in the conversation and the current folder is an IRM protected message.</span></span> 
  
```XML
<HasIrm> true | false </HasIrm>
```

 <span data-ttu-id="55632-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="55632-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55632-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="55632-106">Attributes and elements</span></span>

<span data-ttu-id="55632-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="55632-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55632-108">属性</span><span class="sxs-lookup"><span data-stu-id="55632-108">Attributes</span></span>

<span data-ttu-id="55632-109">なし。</span><span class="sxs-lookup"><span data-stu-id="55632-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55632-110">子要素</span><span class="sxs-lookup"><span data-stu-id="55632-110">Child elements</span></span>

<span data-ttu-id="55632-111">なし。</span><span class="sxs-lookup"><span data-stu-id="55632-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="55632-112">親要素</span><span class="sxs-lookup"><span data-stu-id="55632-112">Parent elements</span></span>

[<span data-ttu-id="55632-113">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="55632-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="text-value"></a><span data-ttu-id="55632-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="55632-114">Text value</span></span>

<span data-ttu-id="55632-115">**会話し、現在のフォルダー内の 1 つ以上のメッセージが IRM を持つ場合、 **HasIrm**要素のテキスト値は**</span><span class="sxs-lookup"><span data-stu-id="55632-115">The text value of the **HasIrm** element is **true** if at least one message in the conversation and the current folder has IRM.</span></span> <span data-ttu-id="55632-116">それ以外の場合、値が**false**にします。</span><span class="sxs-lookup"><span data-stu-id="55632-116">Otherwise, the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="55632-117">備考</span><span class="sxs-lookup"><span data-stu-id="55632-117">Remarks</span></span>

<span data-ttu-id="55632-118">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="55632-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="55632-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="55632-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55632-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="55632-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55632-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="55632-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="55632-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="55632-122">Schema Name</span></span>  <br/> |<span data-ttu-id="55632-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="55632-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="55632-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="55632-124">Validation File</span></span>  <br/> |<span data-ttu-id="55632-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="55632-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="55632-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="55632-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="55632-127">True</span><span class="sxs-lookup"><span data-stu-id="55632-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55632-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="55632-128">See also</span></span>



[<span data-ttu-id="55632-129">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="55632-129">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)


- [<span data-ttu-id="55632-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="55632-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

