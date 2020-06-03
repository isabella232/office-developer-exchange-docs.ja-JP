---
title: IsApprovalRequest
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsApprovalRequest
api_type:
- schema
ms.assetid: 293ed01b-f6a4-4459-819c-933bbfaa2dd7
description: IsApprovalRequest 要素は、条件または例外を適用するために、受信メッセージが承認要求である必要があるかどうかを示します。
ms.openlocfilehash: 08ea36820b2680bb2c7e5695eb2dd481154c05eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530017"
---
# <a name="isapprovalrequest"></a><span data-ttu-id="3531f-103">IsApprovalRequest</span><span class="sxs-lookup"><span data-stu-id="3531f-103">IsApprovalRequest</span></span>

<span data-ttu-id="3531f-104">**Isapprovalrequest**要素は、条件または例外を適用するために、受信メッセージが承認要求である必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="3531f-104">The **IsApprovalRequest** element indicates whether incoming messages must be approval requests in order for the condition or exception to apply.</span></span> 
  
```XML
<IsApprovalRequest/>
```

 <span data-ttu-id="3531f-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="3531f-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3531f-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3531f-106">Attributes and elements</span></span>

<span data-ttu-id="3531f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3531f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3531f-108">属性</span><span class="sxs-lookup"><span data-stu-id="3531f-108">Attributes</span></span>

<span data-ttu-id="3531f-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3531f-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3531f-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3531f-110">Child elements</span></span>

<span data-ttu-id="3531f-111">なし。</span><span class="sxs-lookup"><span data-stu-id="3531f-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="3531f-112">親要素</span><span class="sxs-lookup"><span data-stu-id="3531f-112">Parent elements</span></span>

|<span data-ttu-id="3531f-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="3531f-113">**Element**</span></span>|<span data-ttu-id="3531f-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3531f-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3531f-115">条件</span><span class="sxs-lookup"><span data-stu-id="3531f-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="3531f-116">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="3531f-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="3531f-117">例外</span><span class="sxs-lookup"><span data-stu-id="3531f-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="3531f-118">受信トレイルールに対して使用可能なすべてのルールの例外条件を表します。</span><span class="sxs-lookup"><span data-stu-id="3531f-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="3531f-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3531f-119">Text value</span></span>

<span data-ttu-id="3531f-120">**True**のテキスト値は、条件または例外を適用するために、メッセージが承認要求である必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="3531f-120">A text value of **true** indicates that the message must be an approval request in order for the condition or exception to apply.</span></span> <span data-ttu-id="3531f-121">値が**false**の場合、条件または例外を適用するために、メッセージが承認要求ではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="3531f-121">A value of **false** indicates that the message must not be an approval request in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="3531f-122">注釈</span><span class="sxs-lookup"><span data-stu-id="3531f-122">Remarks</span></span>

<span data-ttu-id="3531f-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3531f-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3531f-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3531f-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3531f-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="3531f-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3531f-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3531f-126">Schema Name</span></span>  <br/> |<span data-ttu-id="3531f-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="3531f-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3531f-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3531f-128">Validation File</span></span>  <br/> |<span data-ttu-id="3531f-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3531f-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3531f-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3531f-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="3531f-131">正しい</span><span class="sxs-lookup"><span data-stu-id="3531f-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3531f-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="3531f-132">See also</span></span>



- [<span data-ttu-id="3531f-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3531f-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

