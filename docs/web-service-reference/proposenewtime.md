---
title: ProposeNewTime
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6d5977ac-484e-4e53-92ba-58a868eb3395
description: ProposeNewTime 要素は、会議の出席者が会議の新しい日時を提案できることを示す応答オブジェクトを指定します。
ms.openlocfilehash: 4a0238d94b29993def8009fae62380bb2c02e8b6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832904"
---
# <a name="proposenewtime"></a><span data-ttu-id="e4a39-103">ProposeNewTime</span><span class="sxs-lookup"><span data-stu-id="e4a39-103">ProposeNewTime</span></span>

<span data-ttu-id="e4a39-104">**ProposeNewTime**要素は、会議の出席者が会議の新しい日時を提案できることを示す応答オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="e4a39-104">The **ProposeNewTime** element specifies a response object that indicates that the meeting attendee can propose a new meeting time.</span></span> 
  
```XML
<ProposeNewTime ObjectName=""></ProposeNewTime>
```

 <span data-ttu-id="e4a39-105">**ProposeNewTimeType**</span><span class="sxs-lookup"><span data-stu-id="e4a39-105">**ProposeNewTimeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e4a39-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e4a39-106">Attributes and elements</span></span>

<span data-ttu-id="e4a39-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e4a39-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4a39-108">属性</span><span class="sxs-lookup"><span data-stu-id="e4a39-108">Attributes</span></span>

****

|<span data-ttu-id="e4a39-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="e4a39-109">**Attribute**</span></span>|<span data-ttu-id="e4a39-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="e4a39-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e4a39-111">オブジェクト名</span><span class="sxs-lookup"><span data-stu-id="e4a39-111">ObjectName</span></span>  <br/> |<span data-ttu-id="e4a39-112">応答オブジェクトの名前。</span><span class="sxs-lookup"><span data-stu-id="e4a39-112">The name of the response object.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e4a39-113">子要素</span><span class="sxs-lookup"><span data-stu-id="e4a39-113">Child elements</span></span>

<span data-ttu-id="e4a39-114">なし。</span><span class="sxs-lookup"><span data-stu-id="e4a39-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e4a39-115">親要素</span><span class="sxs-lookup"><span data-stu-id="e4a39-115">Parent elements</span></span>

[<span data-ttu-id="e4a39-116">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="e4a39-116">ResponseObjects</span></span>](responseobjects.md)
  
## <a name="remarks"></a><span data-ttu-id="e4a39-117">備考</span><span class="sxs-lookup"><span data-stu-id="e4a39-117">Remarks</span></span>

<span data-ttu-id="e4a39-118">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e4a39-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="e4a39-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e4a39-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e4a39-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="e4a39-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e4a39-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="e4a39-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e4a39-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e4a39-122">Schema Name</span></span>  <br/> |<span data-ttu-id="e4a39-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e4a39-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="e4a39-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e4a39-124">Validation File</span></span>  <br/> |<span data-ttu-id="e4a39-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e4a39-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e4a39-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e4a39-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="e4a39-127">True</span><span class="sxs-lookup"><span data-stu-id="e4a39-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e4a39-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="e4a39-128">See also</span></span>



[<span data-ttu-id="e4a39-129">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="e4a39-129">ResponseObjects</span></span>](responseobjects.md)


- [<span data-ttu-id="e4a39-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e4a39-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

