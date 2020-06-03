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
description: HiddenRecipient 要素は、権限のないユーザーから非表示にする必要がある組織のポリシーによって受信者が追加されたことを示します。
ms.openlocfilehash: bfe57fabc02ff00c801672b71ccdb0bf1b916bd9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457642"
---
# <a name="hiddenrecipient"></a><span data-ttu-id="ff7a9-103">HiddenRecipient</span><span class="sxs-lookup"><span data-stu-id="ff7a9-103">HiddenRecipient</span></span>

<span data-ttu-id="ff7a9-104">**HiddenRecipient**要素は、権限のないユーザーから非表示にする必要がある組織のポリシーによって受信者が追加されたことを示します。</span><span class="sxs-lookup"><span data-stu-id="ff7a9-104">The **HiddenRecipient** element indicates that the recipient was added by an organization policy that should be hidden from unprivileged users.</span></span> 
  
```XML
<HiddenRecipient>true | false</HiddenRecipient>
```

 <span data-ttu-id="ff7a9-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="ff7a9-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ff7a9-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ff7a9-106">Attributes and elements</span></span>

<span data-ttu-id="ff7a9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ff7a9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ff7a9-108">属性</span><span class="sxs-lookup"><span data-stu-id="ff7a9-108">Attributes</span></span>

<span data-ttu-id="ff7a9-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ff7a9-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ff7a9-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ff7a9-110">Child elements</span></span>

<span data-ttu-id="ff7a9-111">なし。</span><span class="sxs-lookup"><span data-stu-id="ff7a9-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ff7a9-112">親要素</span><span class="sxs-lookup"><span data-stu-id="ff7a9-112">Parent elements</span></span>

|<span data-ttu-id="ff7a9-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="ff7a9-113">**Element**</span></span>|<span data-ttu-id="ff7a9-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="ff7a9-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ff7a9-115">受信者 Trackingイベント</span><span class="sxs-lookup"><span data-stu-id="ff7a9-115">RecipientTrackingEvent</span></span>](recipienttrackingevent.md) <br/> |<span data-ttu-id="ff7a9-116">受信者に対する1つのイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ff7a9-116">Contains information for a single event for a recipient.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ff7a9-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ff7a9-117">Text value</span></span>

<span data-ttu-id="ff7a9-118">この要素は、 **true**または**false**のいずれかになります。</span><span class="sxs-lookup"><span data-stu-id="ff7a9-118">This element can be either **true** or **false**.</span></span> <span data-ttu-id="ff7a9-119">値**true**は、ユーザーが組織のポリシーによって追加されたことを示します。値が**false**の場合は、ユーザーが組織のポリシーによって追加されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="ff7a9-119">A value of **true** indicates that the user was added by an organization policy; a value of **false** indicates that the user was not added by an organization policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="ff7a9-120">注釈</span><span class="sxs-lookup"><span data-stu-id="ff7a9-120">Remarks</span></span>

<span data-ttu-id="ff7a9-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ff7a9-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ff7a9-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ff7a9-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ff7a9-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="ff7a9-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ff7a9-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ff7a9-124">Schema Name</span></span>  <br/> |<span data-ttu-id="ff7a9-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ff7a9-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="ff7a9-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ff7a9-126">Validation File</span></span>  <br/> |<span data-ttu-id="ff7a9-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ff7a9-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ff7a9-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ff7a9-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="ff7a9-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="ff7a9-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ff7a9-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="ff7a9-130">See also</span></span>



- [<span data-ttu-id="ff7a9-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ff7a9-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

