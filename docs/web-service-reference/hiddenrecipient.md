---
title: HiddenRecipient
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HiddenRecipient
api_type:
- schema
ms.assetid: a8209f75-0070-4424-8dcd-273cfd192728
description: HiddenRecipient 要素は、権限のないユーザーから非表示にする必要があります組織のポリシーによって、受信者が追加されたことを示します。
ms.openlocfilehash: 73b2e3e39c675cf3e2bc56105b1e76009d4a2451
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831810"
---
# <a name="hiddenrecipient"></a><span data-ttu-id="2a9ac-103">HiddenRecipient</span><span class="sxs-lookup"><span data-stu-id="2a9ac-103">HiddenRecipient</span></span>

<span data-ttu-id="2a9ac-104">**HiddenRecipient**要素は、権限のないユーザーから非表示にする必要があります組織のポリシーによって、受信者が追加されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="2a9ac-104">The **HiddenRecipient** element indicates that the recipient was added by an organization policy that should be hidden from unprivileged users.</span></span> 
  
```XML
<HiddenRecipient>true | false</HiddenRecipient>
```

 <span data-ttu-id="2a9ac-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="2a9ac-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2a9ac-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2a9ac-106">Attributes and elements</span></span>

<span data-ttu-id="2a9ac-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2a9ac-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a9ac-108">属性</span><span class="sxs-lookup"><span data-stu-id="2a9ac-108">Attributes</span></span>

<span data-ttu-id="2a9ac-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2a9ac-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2a9ac-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2a9ac-110">Child elements</span></span>

<span data-ttu-id="2a9ac-111">なし。</span><span class="sxs-lookup"><span data-stu-id="2a9ac-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="2a9ac-112">親要素</span><span class="sxs-lookup"><span data-stu-id="2a9ac-112">Parent elements</span></span>

|<span data-ttu-id="2a9ac-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="2a9ac-113">**Element**</span></span>|<span data-ttu-id="2a9ac-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="2a9ac-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a9ac-115">RecipientTrackingEvent</span><span class="sxs-lookup"><span data-stu-id="2a9ac-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="2a9ac-116">受信者の 1 つのイベントの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2a9ac-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2a9ac-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2a9ac-117">Text value</span></span>

<span data-ttu-id="2a9ac-118">この要素には、 **true**または**false**のいずれかができます。</span><span class="sxs-lookup"><span data-stu-id="2a9ac-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="2a9ac-119">**True**の場合は、組織のポリシーは、ユーザーが追加されたことを示します**false**の値は、組織のポリシーによってユーザーを追加しないことを示します。</span><span class="sxs-lookup"><span data-stu-id="2a9ac-119">A value of **true** indicates that the user was added by an organization policy; a value of **false** indicates that the user was not added by an organization policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="2a9ac-120">備考</span><span class="sxs-lookup"><span data-stu-id="2a9ac-120">Remarks</span></span>

<span data-ttu-id="2a9ac-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2a9ac-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2a9ac-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="2a9ac-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2a9ac-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="2a9ac-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2a9ac-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2a9ac-124">Schema Name</span></span>  <br/> |<span data-ttu-id="2a9ac-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="2a9ac-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="2a9ac-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2a9ac-126">Validation File</span></span>  <br/> |<span data-ttu-id="2a9ac-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2a9ac-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2a9ac-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2a9ac-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="2a9ac-129">False</span><span class="sxs-lookup"><span data-stu-id="2a9ac-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2a9ac-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="2a9ac-130">See also</span></span>



- [<span data-ttu-id="2a9ac-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2a9ac-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

