---
title: Is会議要求
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsMeetingRequest
api_type:
- schema
ms.assetid: 72102a55-fd51-4ec9-abce-9a4ec45b86d2
description: IsMeetngRequest 要素は、条件または例外を適用するために、受信メッセージが会議出席依頼である必要があるかどうかを示します。
ms.openlocfilehash: 8b4969faaeb7dfa98edbf4fe8747e8b783808313
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465962"
---
# <a name="ismeetingrequest"></a><span data-ttu-id="03ee5-103">Is会議要求</span><span class="sxs-lookup"><span data-stu-id="03ee5-103">IsMeetingRequest</span></span>

<span data-ttu-id="03ee5-104">**IsMeetngRequest**要素は、条件または例外を適用するために、受信メッセージが会議出席依頼である必要があるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="03ee5-104">The **IsMeetngRequest** element indicates whether incoming messages must be a meeting request in order for the condition or exception to apply.</span></span> 
  
```XML
<IsMeetingRequest>true | false</IsMeetingRequest>
```

 <span data-ttu-id="03ee5-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="03ee5-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="03ee5-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="03ee5-106">Attributes and elements</span></span>

<span data-ttu-id="03ee5-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="03ee5-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="03ee5-108">属性</span><span class="sxs-lookup"><span data-stu-id="03ee5-108">Attributes</span></span>

<span data-ttu-id="03ee5-109">なし。</span><span class="sxs-lookup"><span data-stu-id="03ee5-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="03ee5-110">子要素</span><span class="sxs-lookup"><span data-stu-id="03ee5-110">Child elements</span></span>

<span data-ttu-id="03ee5-111">なし。</span><span class="sxs-lookup"><span data-stu-id="03ee5-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="03ee5-112">親要素</span><span class="sxs-lookup"><span data-stu-id="03ee5-112">Parent elements</span></span>

|<span data-ttu-id="03ee5-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="03ee5-113">**Element**</span></span>|<span data-ttu-id="03ee5-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="03ee5-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="03ee5-115">条件</span><span class="sxs-lookup"><span data-stu-id="03ee5-115">Conditions</span></span>](conditions.md) <br/> |<span data-ttu-id="03ee5-116">ルールのルールの処理を開始するときに実行される条件を表します。</span><span class="sxs-lookup"><span data-stu-id="03ee5-116">Represents the conditions that, when fulfilled, will trigger the rule actions for a rule.</span></span>  <br/> |
|[<span data-ttu-id="03ee5-117">例外</span><span class="sxs-lookup"><span data-stu-id="03ee5-117">Exceptions</span></span>](exceptions.md) <br/> |<span data-ttu-id="03ee5-118">受信トレイルールに対して使用可能なすべてのルールの例外条件を表します。</span><span class="sxs-lookup"><span data-stu-id="03ee5-118">Represents all the available rule exception conditions for an Inbox rule.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="03ee5-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="03ee5-119">Text value</span></span>

<span data-ttu-id="03ee5-120">**True**のテキスト値は、条件または例外を適用するために、メッセージが会議出席依頼である必要があることを示します。</span><span class="sxs-lookup"><span data-stu-id="03ee5-120">A text value of **true** indicates that the message must be a meeting request in order for the condition or exception to apply.</span></span> <span data-ttu-id="03ee5-121">**False**の値は、条件または例外を適用するために、メッセージが会議出席依頼ではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="03ee5-121">A value of **false** indicates that the message must not be a meeting request in order for the condition or exception to apply.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="03ee5-122">注釈</span><span class="sxs-lookup"><span data-stu-id="03ee5-122">Remarks</span></span>

<span data-ttu-id="03ee5-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="03ee5-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="03ee5-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="03ee5-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="03ee5-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="03ee5-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="03ee5-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="03ee5-126">Schema Name</span></span>  <br/> |<span data-ttu-id="03ee5-127">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="03ee5-127">Messages schema</span></span>  <br/> |
|<span data-ttu-id="03ee5-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="03ee5-128">Validation File</span></span>  <br/> |<span data-ttu-id="03ee5-129">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="03ee5-129">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="03ee5-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="03ee5-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="03ee5-131">正しい</span><span class="sxs-lookup"><span data-stu-id="03ee5-131">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="03ee5-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="03ee5-132">See also</span></span>



- [<span data-ttu-id="03ee5-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="03ee5-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

