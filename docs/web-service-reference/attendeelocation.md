---
title: AttendeeLocation
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1344a087-88ea-472a-bebf-9b45245592fb
description: AttendeeLocation 要素は、予定表アイテムの出席者の場所を指定します。
ms.openlocfilehash: 34a4ee8ea5f4c59cce6eebd8977bd4733f7c7134
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460345"
---
# <a name="attendeelocation"></a><span data-ttu-id="be9ec-103">AttendeeLocation</span><span class="sxs-lookup"><span data-stu-id="be9ec-103">AttendeeLocation</span></span>

<span data-ttu-id="be9ec-104">**AttendeeLocation**要素は、予定表アイテムの出席者の場所を指定します。</span><span class="sxs-lookup"><span data-stu-id="be9ec-104">The **AttendeeLocation** element specifies the location of an attendee for a calendar item.</span></span> 
  
```XML
<AttendeeLocation></AttendeeLocation>
```

 <span data-ttu-id="be9ec-105">**xs: 文字列**</span><span class="sxs-lookup"><span data-stu-id="be9ec-105">**xs:string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="be9ec-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="be9ec-106">Attributes and elements</span></span>

<span data-ttu-id="be9ec-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="be9ec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be9ec-108">属性</span><span class="sxs-lookup"><span data-stu-id="be9ec-108">Attributes</span></span>

<span data-ttu-id="be9ec-109">なし。</span><span class="sxs-lookup"><span data-stu-id="be9ec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="be9ec-110">子要素</span><span class="sxs-lookup"><span data-stu-id="be9ec-110">Child elements</span></span>

<span data-ttu-id="be9ec-111">なし。</span><span class="sxs-lookup"><span data-stu-id="be9ec-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="be9ec-112">親要素</span><span class="sxs-lookup"><span data-stu-id="be9ec-112">Parent elements</span></span>

|<span data-ttu-id="be9ec-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="be9ec-113">**Element**</span></span>|<span data-ttu-id="be9ec-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="be9ec-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be9ec-115">Locationの Statedefinition</span><span class="sxs-lookup"><span data-stu-id="be9ec-115">LocationBasedStateDefinition</span></span>](locationbasedstatedefinition.md) <br/> |<span data-ttu-id="be9ec-116">場所に基づく状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="be9ec-116">Specifies the state when it is based on location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="be9ec-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="be9ec-117">Text value</span></span>

<span data-ttu-id="be9ec-118">AttendeeLocation 要素のテキスト値は、出席者の場所です。</span><span class="sxs-lookup"><span data-stu-id="be9ec-118">The text value of the AttendeeLocation element is the attendess location.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="be9ec-119">注釈</span><span class="sxs-lookup"><span data-stu-id="be9ec-119">Remarks</span></span>

<span data-ttu-id="be9ec-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="be9ec-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="be9ec-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="be9ec-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be9ec-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="be9ec-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be9ec-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="be9ec-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="be9ec-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="be9ec-124">Schema Name</span></span>  <br/> |<span data-ttu-id="be9ec-125">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="be9ec-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="be9ec-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="be9ec-126">Validation File</span></span>  <br/> |<span data-ttu-id="be9ec-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="be9ec-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="be9ec-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="be9ec-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="be9ec-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="be9ec-129">See also</span></span>

- [<span data-ttu-id="be9ec-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="be9ec-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

