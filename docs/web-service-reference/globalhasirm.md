---
title: GlobalHasIrm
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 425272b2-7a4e-4376-aea9-d9b10c1ad6ee
description: GlobalHasIrm 要素は、会話内の少なくとも1つのメッセージが IRM で保護されたメッセージであるかどうかを指定します。
ms.openlocfilehash: 10b99c9a6421a89a549b69e918087f3e542ffa09
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459470"
---
# <a name="globalhasirm"></a><span data-ttu-id="606b7-103">GlobalHasIrm</span><span class="sxs-lookup"><span data-stu-id="606b7-103">GlobalHasIrm</span></span>

<span data-ttu-id="606b7-104">**Globalhasirm**要素は、会話内の少なくとも1つのメッセージが IRM で保護されたメッセージであるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="606b7-104">The **GlobalHasIrm** element specifies whether at least one message in the conversation and across all folders is an IRM protected message.</span></span> 
  
```XML
<GlobalHasIrm> true | false </GlobalHasIrm>
```

 <span data-ttu-id="606b7-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="606b7-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="606b7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="606b7-106">Attributes and elements</span></span>

<span data-ttu-id="606b7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="606b7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="606b7-108">属性</span><span class="sxs-lookup"><span data-stu-id="606b7-108">Attributes</span></span>

<span data-ttu-id="606b7-109">なし。</span><span class="sxs-lookup"><span data-stu-id="606b7-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="606b7-110">子要素</span><span class="sxs-lookup"><span data-stu-id="606b7-110">Child elements</span></span>

<span data-ttu-id="606b7-111">なし。</span><span class="sxs-lookup"><span data-stu-id="606b7-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="606b7-112">親要素</span><span class="sxs-lookup"><span data-stu-id="606b7-112">Parent elements</span></span>

[<span data-ttu-id="606b7-113">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="606b7-113">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)
  
## <a name="text-value"></a><span data-ttu-id="606b7-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="606b7-114">Text value</span></span>

<span data-ttu-id="606b7-115">**Globalhasirm**要素のテキスト値は、会話内の少なくとも1つのメッセージが IRM で保護されたメッセージである場合は**true**です。</span><span class="sxs-lookup"><span data-stu-id="606b7-115">The text value of the **GlobalHasIrm** element is **true** if at least one message in the conversation and across all folders is an IRM protected message.</span></span> <span data-ttu-id="606b7-116">それ以外の場合、値は**false**になります。</span><span class="sxs-lookup"><span data-stu-id="606b7-116">Otherwise the value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="606b7-117">注釈</span><span class="sxs-lookup"><span data-stu-id="606b7-117">Remarks</span></span>

<span data-ttu-id="606b7-118">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="606b7-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="606b7-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="606b7-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="606b7-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="606b7-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="606b7-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="606b7-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="606b7-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="606b7-122">Schema Name</span></span>  <br/> |<span data-ttu-id="606b7-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="606b7-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="606b7-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="606b7-124">Validation File</span></span>  <br/> |<span data-ttu-id="606b7-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="606b7-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="606b7-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="606b7-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="606b7-127">正しい</span><span class="sxs-lookup"><span data-stu-id="606b7-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="606b7-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="606b7-128">See also</span></span>



[<span data-ttu-id="606b7-129">会話 (ConversationType)</span><span class="sxs-lookup"><span data-stu-id="606b7-129">Conversation (ConversationType)</span></span>](conversation-conversationtype.md)


- [<span data-ttu-id="606b7-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="606b7-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

