---
title: EndTimeZoneId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 02cf4611-affc-48bc-8e37-53d8694eca58
description: EndTimeZoneId 要素は、会議が行われるタイム ゾーンを指定します。
ms.openlocfilehash: 60d28d5ccea1e99cb8f95f52a22b6ba14bf1f349
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760297"
---
# <a name="endtimezoneid"></a><span data-ttu-id="a81bb-103">EndTimeZoneId</span><span class="sxs-lookup"><span data-stu-id="a81bb-103">EndTimeZoneId</span></span>

<span data-ttu-id="a81bb-104">**EndTimeZoneId**要素は、会議が行われるタイム ゾーンを指定します。</span><span class="sxs-lookup"><span data-stu-id="a81bb-104">The **EndTimeZoneId** element specifies the time zone in which a meeting takes place.</span></span> 
  
```XML
<EndTimeZoneId></EndTimeZoneId>
```

 <span data-ttu-id="a81bb-105">**string**</span><span class="sxs-lookup"><span data-stu-id="a81bb-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a81bb-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a81bb-106">Attributes and elements</span></span>

<span data-ttu-id="a81bb-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a81bb-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a81bb-108">属性</span><span class="sxs-lookup"><span data-stu-id="a81bb-108">Attributes</span></span>

<span data-ttu-id="a81bb-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a81bb-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a81bb-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a81bb-110">Child elements</span></span>

<span data-ttu-id="a81bb-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a81bb-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a81bb-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a81bb-112">Parent elements</span></span>

|<span data-ttu-id="a81bb-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a81bb-113">**Element**</span></span>|<span data-ttu-id="a81bb-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a81bb-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a81bb-115">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="a81bb-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="a81bb-116">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="a81bb-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a81bb-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a81bb-117">Text value</span></span>

<span data-ttu-id="a81bb-118">**EndTimeZoneId**要素は、タイム ゾーン id を指定します。</span><span class="sxs-lookup"><span data-stu-id="a81bb-118">The **EndTimeZoneId** element specifies the time zone identifier.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="a81bb-119">備考</span><span class="sxs-lookup"><span data-stu-id="a81bb-119">Remarks</span></span>

<span data-ttu-id="a81bb-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a81bb-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a81bb-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a81bb-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a81bb-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="a81bb-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a81bb-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="a81bb-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a81bb-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a81bb-124">Schema Name</span></span>  <br/> |<span data-ttu-id="a81bb-125">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="a81bb-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="a81bb-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a81bb-126">Validation File</span></span>  <br/> |<span data-ttu-id="a81bb-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="a81bb-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="a81bb-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a81bb-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="a81bb-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="a81bb-129">See also</span></span>



- [<span data-ttu-id="a81bb-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a81bb-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

