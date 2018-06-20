---
title: DeletedOccurrenceStateDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a9c01c64-e76c-4adc-8b04-88af97bd0cc8
description: DeletedOccurrenceStateDefinition では、予定表アイテムの削除済みアイテムの状態を指定します。
ms.openlocfilehash: ad0434d604ee78ebf1905b60857929e1af4d45f6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759970"
---
# <a name="deletedoccurrencestatedefinition"></a><span data-ttu-id="8f832-103">DeletedOccurrenceStateDefinition</span><span class="sxs-lookup"><span data-stu-id="8f832-103">DeletedOccurrenceStateDefinition</span></span>

<span data-ttu-id="8f832-104">**DeletedOccurrenceStateDefinition**は、予定表アイテムの削除済みアイテムの状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="8f832-104">The **DeletedOccurrenceStateDefinition** specifies the state for a deleted occurrence of a calendar item.</span></span> 
  
```XML
<DeletedOccurrenceStateDefinition>
    <OccurrenceDate></OccurrenceDate>
    <IsOccurrencePresent></IsOccurrencePresent>
</DeletedOccurrenceStateDefinition>
```

 <span data-ttu-id="8f832-105">**DeletedOccurrenceStateDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="8f832-105">**DeletedOccurrenceStateDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8f832-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8f832-106">Attributes and elements</span></span>

<span data-ttu-id="8f832-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8f832-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8f832-108">属性</span><span class="sxs-lookup"><span data-stu-id="8f832-108">Attributes</span></span>

<span data-ttu-id="8f832-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8f832-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8f832-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8f832-110">Child elements</span></span>

|<span data-ttu-id="8f832-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="8f832-111">**Element**</span></span>|<span data-ttu-id="8f832-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="8f832-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f832-113">発生 (タイム ゾーンの切り替え)</span><span class="sxs-lookup"><span data-stu-id="8f832-113">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="8f832-114">予定表アイテムが発生した日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="8f832-114">Specifies the date of the occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="8f832-115">IsOccurrencePresent</span><span class="sxs-lookup"><span data-stu-id="8f832-115">IsOccurrencePresent</span></span>](isoccurrencepresent.md) <br/> |<span data-ttu-id="8f832-116">予定表アイテムの出現箇所が存在するかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="8f832-116">Specifies a Boolean value that indicates whether an occurrence of the calendar item is present.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8f832-117">親要素</span><span class="sxs-lookup"><span data-stu-id="8f832-117">Parent elements</span></span>

|<span data-ttu-id="8f832-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="8f832-118">**Element**</span></span>|<span data-ttu-id="8f832-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="8f832-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f832-120">StateDefinition</span><span class="sxs-lookup"><span data-stu-id="8f832-120">StateDefinition</span></span>](statedefinition.md) <br/> |<span data-ttu-id="8f832-121">状態の定義を指定します。</span><span class="sxs-lookup"><span data-stu-id="8f832-121">Specifies a state definition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8f832-122">備考</span><span class="sxs-lookup"><span data-stu-id="8f832-122">Remarks</span></span>

<span data-ttu-id="8f832-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8f832-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8f832-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8f832-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8f832-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="8f832-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8f832-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="8f832-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8f832-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8f832-127">Schema Name</span></span>  <br/> |<span data-ttu-id="8f832-128">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="8f832-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="8f832-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8f832-129">Validation File</span></span>  <br/> |<span data-ttu-id="8f832-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="8f832-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="8f832-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8f832-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="8f832-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="8f832-132">See also</span></span>

- [<span data-ttu-id="8f832-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8f832-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

