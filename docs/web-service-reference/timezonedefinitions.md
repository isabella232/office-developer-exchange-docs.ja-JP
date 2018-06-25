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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839702"
---
# <a name="timezonedefinitions"></a><span data-ttu-id="1b7e8-103">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="1b7e8-103">TimeZoneDefinitions</span></span>

<span data-ttu-id="1b7e8-104">**TimeZoneDefinitions**要素は、タイム ゾーン定義の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="1b7e8-104">The **TimeZoneDefinitions** element represents an array of time zone definitions.</span></span> 
  
```XML
<TimeZoneDefinitions>
   <TimeZoneDefinition/>
</TimeZoneDefinitions>
```

 <span data-ttu-id="1b7e8-105">**ArrayOfTimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="1b7e8-105">**ArrayOfTimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1b7e8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1b7e8-106">Attributes and elements</span></span>

<span data-ttu-id="1b7e8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1b7e8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1b7e8-108">属性</span><span class="sxs-lookup"><span data-stu-id="1b7e8-108">Attributes</span></span>

<span data-ttu-id="1b7e8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="1b7e8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="1b7e8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="1b7e8-110">Child elements</span></span>

|<span data-ttu-id="1b7e8-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="1b7e8-111">**Element**</span></span>|<span data-ttu-id="1b7e8-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="1b7e8-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b7e8-113">タイム</span><span class="sxs-lookup"><span data-stu-id="1b7e8-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="1b7e8-114">期間とタイム ゾーンを定義するための遷移を指定します。</span><span class="sxs-lookup"><span data-stu-id="1b7e8-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1b7e8-115">親要素</span><span class="sxs-lookup"><span data-stu-id="1b7e8-115">Parent elements</span></span>

|<span data-ttu-id="1b7e8-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="1b7e8-116">**Element**</span></span>|<span data-ttu-id="1b7e8-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="1b7e8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1b7e8-118">GetServerTimeZonesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1b7e8-118">GetServerTimeZonesResponseMessage</span></span>](getservertimezonesresponsemessage.md) <br/> |<span data-ttu-id="1b7e8-119">状態と[GetServerTimeZones の操作](getservertimezones-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1b7e8-119">Contains the status and result of a [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1b7e8-120">備考</span><span class="sxs-lookup"><span data-stu-id="1b7e8-120">Remarks</span></span>

<span data-ttu-id="1b7e8-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1b7e8-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1b7e8-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="1b7e8-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1b7e8-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="1b7e8-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1b7e8-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1b7e8-124">Schema Name</span></span>  <br/> |<span data-ttu-id="1b7e8-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="1b7e8-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1b7e8-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1b7e8-126">Validation File</span></span>  <br/> |<span data-ttu-id="1b7e8-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1b7e8-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1b7e8-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1b7e8-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="1b7e8-129">False</span><span class="sxs-lookup"><span data-stu-id="1b7e8-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1b7e8-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="1b7e8-130">See also</span></span>



- [<span data-ttu-id="1b7e8-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1b7e8-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

