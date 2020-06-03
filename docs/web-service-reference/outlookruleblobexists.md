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
description: OutlookRuleBlobExists 要素は、Microsoft Outlook のルール blob がユーザーのメールボックス内に存在するかどうかを示します。
ms.openlocfilehash: 6a5c2a2ec0246d38b22279b86772972ea81922c7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529029"
---
# <a name="outlookruleblobexists"></a><span data-ttu-id="9a445-103">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="9a445-103">OutlookRuleBlobExists</span></span>

<span data-ttu-id="9a445-104">**Outlookruleblobexists**要素は、Microsoft Outlook のルール blob がユーザーのメールボックス内に存在するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9a445-104">The **OutlookRuleBlobExists** element indicates whether a Microsoft Outlook rule blob exists in the user's mailbox.</span></span> 
  
[<span data-ttu-id="9a445-105">Get受信規則の応答</span><span class="sxs-lookup"><span data-stu-id="9a445-105">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md)
  
[<span data-ttu-id="9a445-106">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="9a445-106">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md)
  
```XML
<OutlookRuleBlobExists>true | false</OutlookRuleBlobExists>
```

 <span data-ttu-id="9a445-107">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="9a445-107">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9a445-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9a445-108">Attributes and elements</span></span>

<span data-ttu-id="9a445-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9a445-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9a445-110">属性</span><span class="sxs-lookup"><span data-stu-id="9a445-110">Attributes</span></span>

<span data-ttu-id="9a445-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9a445-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9a445-112">子要素</span><span class="sxs-lookup"><span data-stu-id="9a445-112">Child elements</span></span>

<span data-ttu-id="9a445-113">なし。</span><span class="sxs-lookup"><span data-stu-id="9a445-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9a445-114">親要素</span><span class="sxs-lookup"><span data-stu-id="9a445-114">Parent elements</span></span>

|<span data-ttu-id="9a445-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="9a445-115">**Element**</span></span>|<span data-ttu-id="9a445-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="9a445-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9a445-117">Get受信規則の応答</span><span class="sxs-lookup"><span data-stu-id="9a445-117">GetInboxRulesResponse</span></span>](getinboxrulesresponse.md) <br/> |<span data-ttu-id="9a445-118">[Get受信トレイの操作](getinboxrules-operation.md)要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="9a445-118">Represents a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9a445-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9a445-119">Text value</span></span>

<span data-ttu-id="9a445-120">テキスト値が**true の場合**は、Outlook ルール blob が存在することを示します。</span><span class="sxs-lookup"><span data-stu-id="9a445-120">A text value of **true** indicates that an Outlook rule blob exists.</span></span> <span data-ttu-id="9a445-121">テキスト値が**false**の場合は、Outlook ルール blob が存在しないことを示します。</span><span class="sxs-lookup"><span data-stu-id="9a445-121">A text value of **false** indicates that an Outlook rule blob does not exist.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9a445-122">注釈</span><span class="sxs-lookup"><span data-stu-id="9a445-122">Remarks</span></span>

<span data-ttu-id="9a445-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9a445-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9a445-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9a445-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9a445-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="9a445-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9a445-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9a445-126">Schema Name</span></span>  <br/> |<span data-ttu-id="9a445-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="9a445-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9a445-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9a445-128">Validation File</span></span>  <br/> |<span data-ttu-id="9a445-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="9a445-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9a445-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9a445-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="9a445-131">正しい</span><span class="sxs-lookup"><span data-stu-id="9a445-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9a445-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="9a445-132">See also</span></span>



- [<span data-ttu-id="9a445-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9a445-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

