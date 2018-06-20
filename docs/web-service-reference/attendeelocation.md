---
title: AttendeeLocation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1344a087-88ea-472a-bebf-9b45245592fb
description: AttendeeLocation 要素は、出席者の予定表アイテムの場所を指定します。
ms.openlocfilehash: 4670f1fa59fec4cf1e2b35a1380f6205677ce5af
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759458"
---
# <a name="attendeelocation"></a><span data-ttu-id="4e8d4-103">AttendeeLocation</span><span class="sxs-lookup"><span data-stu-id="4e8d4-103">AttendeeLocation</span></span>

<span data-ttu-id="4e8d4-104">**AttendeeLocation**要素は、出席者の予定表アイテムの場所を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e8d4-104">The **AttendeeLocation** element specifies the location of an attendee for a calendar item.</span></span> 
  
```XML
<AttendeeLocation></AttendeeLocation>
```

 <span data-ttu-id="4e8d4-105">**使用されています**</span><span class="sxs-lookup"><span data-stu-id="4e8d4-105">**xs:string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4e8d4-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4e8d4-106">Attributes and elements</span></span>

<span data-ttu-id="4e8d4-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4e8d4-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4e8d4-108">属性</span><span class="sxs-lookup"><span data-stu-id="4e8d4-108">Attributes</span></span>

<span data-ttu-id="4e8d4-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4e8d4-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4e8d4-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4e8d4-110">Child elements</span></span>

<span data-ttu-id="4e8d4-111">なし。</span><span class="sxs-lookup"><span data-stu-id="4e8d4-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="4e8d4-112">親要素</span><span class="sxs-lookup"><span data-stu-id="4e8d4-112">Parent elements</span></span>

|<span data-ttu-id="4e8d4-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="4e8d4-113">**Element**</span></span>|<span data-ttu-id="4e8d4-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="4e8d4-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e8d4-115">LocationBasedStateDefinition</span><span class="sxs-lookup"><span data-stu-id="4e8d4-115">LocationBasedStateDefinition</span></span>](locationbasedstatedefinition.md) <br/> |<span data-ttu-id="4e8d4-116">場所に基づいて、状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="4e8d4-116">Specifies the state when it is based on location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4e8d4-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4e8d4-117">Text value</span></span>

<span data-ttu-id="4e8d4-118">AttendeeLocation 要素のテキスト値は、attendess 場所です。</span><span class="sxs-lookup"><span data-stu-id="4e8d4-118">The text value of the AttendeeLocation element is the attendess location.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4e8d4-119">備考</span><span class="sxs-lookup"><span data-stu-id="4e8d4-119">Remarks</span></span>

<span data-ttu-id="4e8d4-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4e8d4-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="4e8d4-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4e8d4-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4e8d4-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="4e8d4-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4e8d4-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="4e8d4-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="4e8d4-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4e8d4-124">Schema Name</span></span>  <br/> |<span data-ttu-id="4e8d4-125">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="4e8d4-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="4e8d4-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4e8d4-126">Validation File</span></span>  <br/> |<span data-ttu-id="4e8d4-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="4e8d4-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="4e8d4-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4e8d4-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="4e8d4-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="4e8d4-129">See also</span></span>

- [<span data-ttu-id="4e8d4-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4e8d4-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

