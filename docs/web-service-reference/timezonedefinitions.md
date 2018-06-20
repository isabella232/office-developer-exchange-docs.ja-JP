---
title: TimeZoneDefinitions
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- TimeZoneDefinitions
api_type:
- schema
ms.assetid: 9ca1584e-65b8-49ba-a408-e3e8597e6607
description: TimeZoneDefinitions 要素は、タイム ゾーン定義の配列を表します。
ms.openlocfilehash: 0bc1b69ef564bb4e239d9845a4b1a0133292ff12
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839702"
---
# <a name="timezonedefinitions"></a><span data-ttu-id="e3654-103">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="e3654-103">TimeZoneDefinitions</span></span>

<span data-ttu-id="e3654-104">**TimeZoneDefinitions**要素は、タイム ゾーン定義の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="e3654-104">The **TimeZoneDefinitions** element represents an array of time zone definitions.</span></span> 
  
```XML
<TimeZoneDefinitions>
   <TimeZoneDefinition/>
</TimeZoneDefinitions>
```

 <span data-ttu-id="e3654-105">**ArrayOfTimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="e3654-105">**ArrayOfTimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e3654-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e3654-106">Attributes and elements</span></span>

<span data-ttu-id="e3654-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e3654-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e3654-108">属性</span><span class="sxs-lookup"><span data-stu-id="e3654-108">Attributes</span></span>

<span data-ttu-id="e3654-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e3654-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e3654-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e3654-110">Child elements</span></span>

|<span data-ttu-id="e3654-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="e3654-111">**Element**</span></span>|<span data-ttu-id="e3654-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e3654-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3654-113">タイム</span><span class="sxs-lookup"><span data-stu-id="e3654-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="e3654-114">期間とタイム ゾーンを定義するための遷移を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3654-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e3654-115">親要素</span><span class="sxs-lookup"><span data-stu-id="e3654-115">Parent elements</span></span>

|<span data-ttu-id="e3654-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="e3654-116">**Element**</span></span>|<span data-ttu-id="e3654-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="e3654-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e3654-118">GetServerTimeZonesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e3654-118">GetServerTimeZonesResponseMessage</span></span>](getservertimezonesresponsemessage.md) <br/> |<span data-ttu-id="e3654-119">状態と[GetServerTimeZones の操作](getservertimezones-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e3654-119">Contains the status and result of a [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e3654-120">備考</span><span class="sxs-lookup"><span data-stu-id="e3654-120">Remarks</span></span>

<span data-ttu-id="e3654-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e3654-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e3654-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="e3654-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e3654-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="e3654-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e3654-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e3654-124">Schema Name</span></span>  <br/> |<span data-ttu-id="e3654-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e3654-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e3654-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e3654-126">Validation File</span></span>  <br/> |<span data-ttu-id="e3654-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e3654-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e3654-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e3654-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="e3654-129">False</span><span class="sxs-lookup"><span data-stu-id="e3654-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e3654-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="e3654-130">See also</span></span>



- [<span data-ttu-id="e3654-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e3654-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

