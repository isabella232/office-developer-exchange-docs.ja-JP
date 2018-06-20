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
description: NoEndRecurrence 要素は、定義された終了日がない項目の定期的なパターンの開始日について説明します。
ms.openlocfilehash: fc3eae170f5c07e31d7a80b45836efd07d74e543
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832537"
---
# <a name="noendrecurrence"></a><span data-ttu-id="39a05-103">NoEndRecurrence</span><span class="sxs-lookup"><span data-stu-id="39a05-103">NoEndRecurrence</span></span>

<span data-ttu-id="39a05-104">**NoEndRecurrence**要素は、定義された終了日がない項目の定期的なパターンの開始日について説明します。</span><span class="sxs-lookup"><span data-stu-id="39a05-104">The **NoEndRecurrence** element describes the start date of an item recurrence pattern that does not have a defined end date.</span></span> 
  
```xml
<NoEndRecurrence>
   <StartDate/>
</NoEndRecurrence>
```

 <span data-ttu-id="39a05-105">**NoEndRecurrenceRangeType**</span><span class="sxs-lookup"><span data-stu-id="39a05-105">**NoEndRecurrenceRangeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="39a05-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="39a05-106">Attributes and elements</span></span>

<span data-ttu-id="39a05-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="39a05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="39a05-108">属性</span><span class="sxs-lookup"><span data-stu-id="39a05-108">Attributes</span></span>

<span data-ttu-id="39a05-109">なし。</span><span class="sxs-lookup"><span data-stu-id="39a05-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="39a05-110">子要素</span><span class="sxs-lookup"><span data-stu-id="39a05-110">Child elements</span></span>

|<span data-ttu-id="39a05-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="39a05-111">**Element**</span></span>|<span data-ttu-id="39a05-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="39a05-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39a05-113">開始日 (繰り返し)</span><span class="sxs-lookup"><span data-stu-id="39a05-113">StartDate (Recurrence)</span></span>](startdate-recurrence.md) <br/> |<span data-ttu-id="39a05-114">定期的な仕事または予定表アイテムの開始日を表します。</span><span class="sxs-lookup"><span data-stu-id="39a05-114">Represents the start date of a recurring task or calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="39a05-115">親要素</span><span class="sxs-lookup"><span data-stu-id="39a05-115">Parent elements</span></span>

|<span data-ttu-id="39a05-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="39a05-116">**Element**</span></span>|<span data-ttu-id="39a05-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="39a05-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39a05-118">定期的なアイテム (RecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="39a05-118">Recurrence (RecurrenceType)</span></span>](recurrence-recurrencetype.md) <br/> |<span data-ttu-id="39a05-119">予定表アイテムおよび会議出席依頼に定期的なパターンが含まれています。</span><span class="sxs-lookup"><span data-stu-id="39a05-119">Contains the recurrence pattern for calendar items and meeting requests.</span></span>  <br/> |
|[<span data-ttu-id="39a05-120">定期的な予定 (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="39a05-120">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="39a05-121">定期タスクの頻度に関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="39a05-121">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="39a05-122">備考</span><span class="sxs-lookup"><span data-stu-id="39a05-122">Remarks</span></span>

<span data-ttu-id="39a05-123">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="39a05-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="39a05-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="39a05-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="39a05-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="39a05-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="39a05-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="39a05-126">Schema name</span></span>  <br/> |<span data-ttu-id="39a05-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="39a05-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="39a05-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="39a05-128">Validation file</span></span>  <br/> |<span data-ttu-id="39a05-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="39a05-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="39a05-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="39a05-130">Can be empty</span></span>  <br/> |<span data-ttu-id="39a05-131">False</span><span class="sxs-lookup"><span data-stu-id="39a05-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="39a05-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="39a05-132">See also</span></span>



- [<span data-ttu-id="39a05-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="39a05-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

