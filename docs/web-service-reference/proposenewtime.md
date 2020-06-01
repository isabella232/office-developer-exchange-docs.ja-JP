---
title: ProposeNewTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6d5977ac-484e-4e53-92ba-58a868eb3395
description: ProposeNewTime 要素は、会議の出席者が新しい会議日時を提案できることを示す response オブジェクトを指定します。
ms.openlocfilehash: 76f590db760826aa2cd26938947a9b0e02a603f7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465542"
---
# <a name="proposenewtime"></a><span data-ttu-id="ba18b-103">ProposeNewTime</span><span class="sxs-lookup"><span data-stu-id="ba18b-103">ProposeNewTime</span></span>

<span data-ttu-id="ba18b-104">**ProposeNewTime**要素は、会議の出席者が新しい会議日時を提案できることを示す response オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="ba18b-104">The **ProposeNewTime** element specifies a response object that indicates that the meeting attendee can propose a new meeting time.</span></span> 
  
```XML
<ProposeNewTime ObjectName=""></ProposeNewTime>
```

 <span data-ttu-id="ba18b-105">**ProposeNewTimeType**</span><span class="sxs-lookup"><span data-stu-id="ba18b-105">**ProposeNewTimeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ba18b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ba18b-106">Attributes and elements</span></span>

<span data-ttu-id="ba18b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ba18b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ba18b-108">属性</span><span class="sxs-lookup"><span data-stu-id="ba18b-108">Attributes</span></span>

****

|<span data-ttu-id="ba18b-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="ba18b-109">**Attribute**</span></span>|<span data-ttu-id="ba18b-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="ba18b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ba18b-111">ObjectName</span><span class="sxs-lookup"><span data-stu-id="ba18b-111">ObjectName</span></span>  <br/> |<span data-ttu-id="ba18b-112">Response オブジェクトの名前を指定します。</span><span class="sxs-lookup"><span data-stu-id="ba18b-112">The name of the response object.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ba18b-113">子要素</span><span class="sxs-lookup"><span data-stu-id="ba18b-113">Child elements</span></span>

<span data-ttu-id="ba18b-114">なし。</span><span class="sxs-lookup"><span data-stu-id="ba18b-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="ba18b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="ba18b-115">Parent elements</span></span>

[<span data-ttu-id="ba18b-116">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="ba18b-116">ResponseObjects</span></span>](responseobjects.md)
  
## <a name="remarks"></a><span data-ttu-id="ba18b-117">注釈</span><span class="sxs-lookup"><span data-stu-id="ba18b-117">Remarks</span></span>

<span data-ttu-id="ba18b-118">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="ba18b-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="ba18b-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ba18b-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ba18b-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ba18b-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ba18b-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="ba18b-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ba18b-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ba18b-122">Schema Name</span></span>  <br/> |<span data-ttu-id="ba18b-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ba18b-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="ba18b-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ba18b-124">Validation File</span></span>  <br/> |<span data-ttu-id="ba18b-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ba18b-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ba18b-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ba18b-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="ba18b-127">正しい</span><span class="sxs-lookup"><span data-stu-id="ba18b-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ba18b-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="ba18b-128">See also</span></span>



[<span data-ttu-id="ba18b-129">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="ba18b-129">ResponseObjects</span></span>](responseobjects.md)


- [<span data-ttu-id="ba18b-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ba18b-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

