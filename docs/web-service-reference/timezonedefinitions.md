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
description: TimeZoneDefinitions 要素は、タイムゾーン定義の配列を表します。
ms.openlocfilehash: 16a25eb4fdcad2554ebd19626d0a0bc7f6391ac5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468762"
---
# <a name="timezonedefinitions"></a><span data-ttu-id="df945-103">TimeZoneDefinitions</span><span class="sxs-lookup"><span data-stu-id="df945-103">TimeZoneDefinitions</span></span>

<span data-ttu-id="df945-104">**TimeZoneDefinitions**要素は、タイムゾーン定義の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="df945-104">The **TimeZoneDefinitions** element represents an array of time zone definitions.</span></span> 
  
```XML
<TimeZoneDefinitions>
   <TimeZoneDefinition/>
</TimeZoneDefinitions>
```

 <span data-ttu-id="df945-105">**ArrayOfTimeZoneDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="df945-105">**ArrayOfTimeZoneDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="df945-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="df945-106">Attributes and elements</span></span>

<span data-ttu-id="df945-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="df945-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="df945-108">属性</span><span class="sxs-lookup"><span data-stu-id="df945-108">Attributes</span></span>

<span data-ttu-id="df945-109">なし。</span><span class="sxs-lookup"><span data-stu-id="df945-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="df945-110">子要素</span><span class="sxs-lookup"><span data-stu-id="df945-110">Child elements</span></span>

|<span data-ttu-id="df945-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="df945-111">**Element**</span></span>|<span data-ttu-id="df945-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="df945-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="df945-113">TimeZoneDefinition</span><span class="sxs-lookup"><span data-stu-id="df945-113">TimeZoneDefinition</span></span>](timezonedefinition.md) <br/> |<span data-ttu-id="df945-114">タイムゾーンを定義する期間と切り替えを指定します。</span><span class="sxs-lookup"><span data-stu-id="df945-114">Specifies the periods and transitions that define a time zone.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="df945-115">親要素</span><span class="sxs-lookup"><span data-stu-id="df945-115">Parent elements</span></span>

|<span data-ttu-id="df945-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="df945-116">**Element**</span></span>|<span data-ttu-id="df945-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="df945-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="df945-118">GetServerTimeZonesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="df945-118">GetServerTimeZonesResponseMessage</span></span>](getservertimezonesresponsemessage.md) <br/> |<span data-ttu-id="df945-119">[GetServerTimeZones 操作](getservertimezones-operation.md)要求の状態と結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="df945-119">Contains the status and result of a [GetServerTimeZones operation](getservertimezones-operation.md) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="df945-120">注釈</span><span class="sxs-lookup"><span data-stu-id="df945-120">Remarks</span></span>

<span data-ttu-id="df945-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="df945-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="df945-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="df945-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="df945-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="df945-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="df945-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="df945-124">Schema Name</span></span>  <br/> |<span data-ttu-id="df945-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="df945-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="df945-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="df945-126">Validation File</span></span>  <br/> |<span data-ttu-id="df945-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="df945-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="df945-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="df945-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="df945-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="df945-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="df945-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="df945-130">See also</span></span>



- [<span data-ttu-id="df945-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="df945-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

