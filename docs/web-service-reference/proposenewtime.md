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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832904"
---
# <a name="proposenewtime"></a><span data-ttu-id="6075c-103">ProposeNewTime</span><span class="sxs-lookup"><span data-stu-id="6075c-103">ProposeNewTime</span></span>

<span data-ttu-id="6075c-104">**ProposeNewTime**要素は、会議の出席者が会議の新しい日時を提案できることを示す応答オブジェクトを指定します。</span><span class="sxs-lookup"><span data-stu-id="6075c-104">The **ProposeNewTime** element specifies a response object that indicates that the meeting attendee can propose a new meeting time.</span></span> 
  
```XML
<ProposeNewTime ObjectName=""></ProposeNewTime>
```

 <span data-ttu-id="6075c-105">**ProposeNewTimeType**</span><span class="sxs-lookup"><span data-stu-id="6075c-105">**ProposeNewTimeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6075c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6075c-106">Attributes and elements</span></span>

<span data-ttu-id="6075c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6075c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6075c-108">属性</span><span class="sxs-lookup"><span data-stu-id="6075c-108">Attributes</span></span>

****

|<span data-ttu-id="6075c-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="6075c-109">**Attribute**</span></span>|<span data-ttu-id="6075c-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="6075c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6075c-111">オブジェクト名</span><span class="sxs-lookup"><span data-stu-id="6075c-111">ObjectName</span></span>  <br/> |<span data-ttu-id="6075c-112">応答オブジェクトの名前。</span><span class="sxs-lookup"><span data-stu-id="6075c-112">The name of the response object.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6075c-113">子要素</span><span class="sxs-lookup"><span data-stu-id="6075c-113">Child elements</span></span>

<span data-ttu-id="6075c-114">なし。</span><span class="sxs-lookup"><span data-stu-id="6075c-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6075c-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6075c-115">Parent elements</span></span>

[<span data-ttu-id="6075c-116">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="6075c-116">ResponseObjects</span></span>](responseobjects.md)
  
## <a name="remarks"></a><span data-ttu-id="6075c-117">備考</span><span class="sxs-lookup"><span data-stu-id="6075c-117">Remarks</span></span>

<span data-ttu-id="6075c-118">この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6075c-118">This element was introduced in Exchange Server 2013 Service Pack 1 (SP1).</span></span>
  
<span data-ttu-id="6075c-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6075c-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6075c-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="6075c-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6075c-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="6075c-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6075c-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6075c-122">Schema Name</span></span>  <br/> |<span data-ttu-id="6075c-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="6075c-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="6075c-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6075c-124">Validation File</span></span>  <br/> |<span data-ttu-id="6075c-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="6075c-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6075c-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6075c-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="6075c-127">True</span><span class="sxs-lookup"><span data-stu-id="6075c-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6075c-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="6075c-128">See also</span></span>



[<span data-ttu-id="6075c-129">ResponseObjects</span><span class="sxs-lookup"><span data-stu-id="6075c-129">ResponseObjects</span></span>](responseobjects.md)


- [<span data-ttu-id="6075c-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6075c-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

