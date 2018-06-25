---
title: OutlookRuleBlobExists
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- OutlookRuleBlobExists
api_type:
- schema
ms.assetid: ae1bc448-deb9-4b5b-ab38-4b276abcb650
description: OutlookRuleBlobExists 要素は、ユーザーのメールボックスに Outlook のルールの blob が存在するかどうかを示します。
ms.openlocfilehash: a738377cd3c1d69b90ac39ca479b03b3220d5bc5
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832679"
---
# <a name="outlookruleblobexists"></a><span data-ttu-id="00a64-103">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="00a64-103">OutlookRuleBlobExists</span></span>

<span data-ttu-id="00a64-104">**OutlookRuleBlobExists**要素は、ユーザーのメールボックスに Outlook のルールの blob が存在するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="00a64-104">The **OutlookRuleBlobExists** element indicates whether a Microsoft Outlook rule blob exists in the user's mailbox.</span></span> 
  
[<span data-ttu-id="00a64-105">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="00a64-105">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md)
  
[<span data-ttu-id="00a64-106">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="00a64-106">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md)
  
```XML
<OutlookRuleBlobExists>true | false</OutlookRuleBlobExists>
```

 <span data-ttu-id="00a64-107">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="00a64-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="00a64-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="00a64-108">Attributes and elements</span></span>

<span data-ttu-id="00a64-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="00a64-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="00a64-110">属性</span><span class="sxs-lookup"><span data-stu-id="00a64-110">Attributes</span></span>

<span data-ttu-id="00a64-111">なし。</span><span class="sxs-lookup"><span data-stu-id="00a64-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="00a64-112">子要素</span><span class="sxs-lookup"><span data-stu-id="00a64-112">Child elements</span></span>

<span data-ttu-id="00a64-113">なし。</span><span class="sxs-lookup"><span data-stu-id="00a64-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="00a64-114">親要素</span><span class="sxs-lookup"><span data-stu-id="00a64-114">Parent elements</span></span>

|<span data-ttu-id="00a64-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="00a64-115">**Element**</span></span>|<span data-ttu-id="00a64-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="00a64-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="00a64-117">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="00a64-117">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md) <br/> |<span data-ttu-id="00a64-118">[GetInboxRules 操作](getinboxrules-operation.md)要求に対する応答を表します。</span><span class="sxs-lookup"><span data-stu-id="00a64-118">Represents a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="00a64-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="00a64-119">Text value</span></span>

<span data-ttu-id="00a64-120">**True**の場合、テキスト値は、Outlook のルール blob が存在することを示します。</span><span class="sxs-lookup"><span data-stu-id="00a64-120">A text value of **true** indicates that an Outlook rule blob exists.</span></span> <span data-ttu-id="00a64-121">**False**のテキスト値は、Outlook のルール blob が存在しないことを示します。</span><span class="sxs-lookup"><span data-stu-id="00a64-121">A text value of **false** indicates that an Outlook rule blob does not exist.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="00a64-122">備考</span><span class="sxs-lookup"><span data-stu-id="00a64-122">Remarks</span></span>

<span data-ttu-id="00a64-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="00a64-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="00a64-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="00a64-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="00a64-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="00a64-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="00a64-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="00a64-126">Schema Name</span></span>  <br/> |<span data-ttu-id="00a64-127">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="00a64-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="00a64-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="00a64-128">Validation File</span></span>  <br/> |<span data-ttu-id="00a64-129">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="00a64-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="00a64-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="00a64-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="00a64-131">True</span><span class="sxs-lookup"><span data-stu-id="00a64-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="00a64-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="00a64-132">See also</span></span>



- [<span data-ttu-id="00a64-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="00a64-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

