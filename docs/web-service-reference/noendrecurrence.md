---
title: NoEndRecurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NoEndRecurrence
api_type:
- schema
ms.assetid: ab2ebd9c-388e-45f1-abf9-56e293ef123b
description: NoEndRecurrence な要素は、定義された終了日を持たないアイテムの定期的なパターンの開始日を示します。
ms.openlocfilehash: 31a3bd6ae2d7ce94debbeebc4fd4f536447433a7
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/01/2020
ms.locfileid: "44466795"
---
# <a name="noendrecurrence"></a><span data-ttu-id="2b384-103">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="2b384-103">NoEndRecurrence</span></span>

<span data-ttu-id="2b384-104">**Noendrecurrence**な要素は、定義された終了日を持たないアイテムの定期的なパターンの開始日を示します。</span><span class="sxs-lookup"><span data-stu-id="2b384-104">The **NoEndRecurrence** element describes the start date of an item recurrence pattern that does not have a defined end date.</span></span> 
  
```xml
<NoEndRecurrence>
   <StartDate/>
</NoEndRecurrence>
```

 <span data-ttu-id="2b384-105">**NoEndRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="2b384-105">**NoEndRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2b384-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2b384-106">Attributes and elements</span></span>

<span data-ttu-id="2b384-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2b384-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2b384-108">属性</span><span class="sxs-lookup"><span data-stu-id="2b384-108">Attributes</span></span>

<span data-ttu-id="2b384-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2b384-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2b384-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2b384-110">Child elements</span></span>

|<span data-ttu-id="2b384-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="2b384-111">**Element**</span></span>|<span data-ttu-id="2b384-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2b384-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b384-113">StartDate (定期的な予定)</span><span class="sxs-lookup"><span data-stu-id="2b384-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="2b384-114">定期的な仕事または予定表アイテムの開始日を表します。</span><span class="sxs-lookup"><span data-stu-id="2b384-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2b384-115">親要素</span><span class="sxs-lookup"><span data-stu-id="2b384-115">Parent elements</span></span>

|<span data-ttu-id="2b384-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="2b384-116">**Element**</span></span>|<span data-ttu-id="2b384-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="2b384-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2b384-118">Recurrence (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="2b384-118">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="2b384-119">予定表アイテムと会議出席依頼の定期的なパターンを含みます。</span><span class="sxs-lookup"><span data-stu-id="2b384-119">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="2b384-120">定期的なアイテム (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="2b384-120">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="2b384-121">定期的なタスクの定期的なアイテムの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2b384-121">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2b384-122">注釈</span><span class="sxs-lookup"><span data-stu-id="2b384-122">Remarks</span></span>

<span data-ttu-id="2b384-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2b384-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2b384-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2b384-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2b384-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="2b384-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2b384-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2b384-126">Schema name</span></span>  <br/> |<span data-ttu-id="2b384-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="2b384-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="2b384-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2b384-128">Validation file</span></span>  <br/> |<span data-ttu-id="2b384-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="2b384-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2b384-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="2b384-130">Can be empty</span></span>  <br/> |<span data-ttu-id="2b384-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="2b384-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2b384-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="2b384-132">See also</span></span>



- [<span data-ttu-id="2b384-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2b384-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

