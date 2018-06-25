---
title: DeleteFromFolderStateDefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3aba59a0-f12a-48b5-842b-11cf4530dd51
description: DeleteFromFolderStateDefinition 要素は、フォルダーからアイテムが削除されたときの状態を指定します。
ms.openlocfilehash: 7b6374b9fa55d3b08569e8ac9e247dd6e5bebc24
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759981"
---
# <a name="deletefromfolderstatedefinition"></a><span data-ttu-id="5cfdd-103">DeleteFromFolderStateDefinition</span><span class="sxs-lookup"><span data-stu-id="5cfdd-103">DeleteFromFolderStateDefinition</span></span>

<span data-ttu-id="5cfdd-104">**DeleteFromFolderStateDefinition**要素は、フォルダーからアイテムが削除されたときの状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="5cfdd-104">The **DeleteFromFolderStateDefinition** element specifies the state when an item is deleted from a folder.</span></span> 
  
```XML
<DeleteFromFolderStateDefinition>
    <OccurrenceDate></OccurrenceDate>
    <IsOccurrencePresent></IsOccurrencePresent>
</DeleteFromFolderStateDefinition>
```

 <span data-ttu-id="5cfdd-105">**DeleteFromFolderStateDefinitionType**</span><span class="sxs-lookup"><span data-stu-id="5cfdd-105">**DeleteFromFolderStateDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5cfdd-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5cfdd-106">Attributes and elements</span></span>

<span data-ttu-id="5cfdd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5cfdd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5cfdd-108">属性</span><span class="sxs-lookup"><span data-stu-id="5cfdd-108">Attributes</span></span>

<span data-ttu-id="5cfdd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="5cfdd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="5cfdd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="5cfdd-110">Child elements</span></span>

|<span data-ttu-id="5cfdd-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="5cfdd-111">**Element**</span></span>|<span data-ttu-id="5cfdd-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="5cfdd-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5cfdd-113">発生 (タイム ゾーンの切り替え)</span><span class="sxs-lookup"><span data-stu-id="5cfdd-113">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="5cfdd-114">予定表アイテムが発生した日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="5cfdd-114">Specifies the date of the occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="5cfdd-115">IsOccurrencePresent</span><span class="sxs-lookup"><span data-stu-id="5cfdd-115">IsOccurrencePresent</span></span>](isoccurrencepresent.md) <br/> |<span data-ttu-id="5cfdd-116">予定表アイテムの出現箇所が存在するかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="5cfdd-116">Specifies a Boolean value that indicates whether an occurrence of the calendar item is present.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5cfdd-117">親要素</span><span class="sxs-lookup"><span data-stu-id="5cfdd-117">Parent elements</span></span>

|<span data-ttu-id="5cfdd-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="5cfdd-118">**Element**</span></span>|<span data-ttu-id="5cfdd-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="5cfdd-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5cfdd-120">StateDefinition</span><span class="sxs-lookup"><span data-stu-id="5cfdd-120">StateDefinition</span></span>](statedefinition.md) <br/> |<span data-ttu-id="5cfdd-121">状態の定義を指定します。</span><span class="sxs-lookup"><span data-stu-id="5cfdd-121">Specifies a state definition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5cfdd-122">備考</span><span class="sxs-lookup"><span data-stu-id="5cfdd-122">Remarks</span></span>

<span data-ttu-id="5cfdd-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="5cfdd-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="5cfdd-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="5cfdd-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5cfdd-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="5cfdd-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5cfdd-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="5cfdd-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5cfdd-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5cfdd-127">Schema Name</span></span>  <br/> |<span data-ttu-id="5cfdd-128">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="5cfdd-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="5cfdd-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5cfdd-129">Validation File</span></span>  <br/> |<span data-ttu-id="5cfdd-130">types.xsd</span><span class="sxs-lookup"><span data-stu-id="5cfdd-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="5cfdd-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="5cfdd-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="5cfdd-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="5cfdd-132">See also</span></span>

- [<span data-ttu-id="5cfdd-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5cfdd-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

