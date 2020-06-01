---
title: Deletedocの Enceencestatedefinition
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: a9c01c64-e76c-4adc-8b04-88af97bd0cc8
description: Deletedoc状態 Encestatedefinition は、予定表アイテムの削除されたアイテムの状態を指定します。
ms.openlocfilehash: ff8ad1d9c35d7bab3f6fe2cd1896bb16384c18e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458797"
---
# <a name="deletedoccurrencestatedefinition"></a><span data-ttu-id="eecd1-103">Deletedocの Enceencestatedefinition</span><span class="sxs-lookup"><span data-stu-id="eecd1-103">DeletedOccurrenceStateDefinition</span></span>

<span data-ttu-id="eecd1-104">**Deletedoc状態 Encestatedefinition**は、予定表アイテムの削除されたアイテムの状態を指定します。</span><span class="sxs-lookup"><span data-stu-id="eecd1-104">The **DeletedOccurrenceStateDefinition** specifies the state for a deleted occurrence of a calendar item.</span></span> 
  
```XML
<DeletedOccurrenceStateDefinition>
    <OccurrenceDate></OccurrenceDate>
    <IsOccurrencePresent></IsOccurrencePresent>
</DeletedOccurrenceStateDefinition>
```

 <span data-ttu-id="eecd1-105">**Deletedocの Enceencestatedefinitiontype**</span><span class="sxs-lookup"><span data-stu-id="eecd1-105">**DeletedOccurrenceStateDefinitionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eecd1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="eecd1-106">Attributes and elements</span></span>

<span data-ttu-id="eecd1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="eecd1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eecd1-108">属性</span><span class="sxs-lookup"><span data-stu-id="eecd1-108">Attributes</span></span>

<span data-ttu-id="eecd1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="eecd1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="eecd1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="eecd1-110">Child elements</span></span>

|<span data-ttu-id="eecd1-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="eecd1-111">**Element**</span></span>|<span data-ttu-id="eecd1-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="eecd1-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eecd1-113">発生 (タイムゾーンの切り替え)</span><span class="sxs-lookup"><span data-stu-id="eecd1-113">Occurrence (Time Zone Transition)</span></span>](occurrence-time-zone-transition.md) <br/> |<span data-ttu-id="eecd1-114">予定表アイテムが発生する日付を指定します。</span><span class="sxs-lookup"><span data-stu-id="eecd1-114">Specifies the date of the occurrence of a calendar item.</span></span>  <br/> |
|[<span data-ttu-id="eecd1-115">Iソケットの現在の表示</span><span class="sxs-lookup"><span data-stu-id="eecd1-115">IsOccurrencePresent</span></span>](isoccurrencepresent.md) <br/> |<span data-ttu-id="eecd1-116">予定表アイテムの発生が存在するかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="eecd1-116">Specifies a Boolean value that indicates whether an occurrence of the calendar item is present.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eecd1-117">親要素</span><span class="sxs-lookup"><span data-stu-id="eecd1-117">Parent elements</span></span>

|<span data-ttu-id="eecd1-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="eecd1-118">**Element**</span></span>|<span data-ttu-id="eecd1-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="eecd1-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eecd1-120">StateDefinition</span><span class="sxs-lookup"><span data-stu-id="eecd1-120">StateDefinition</span></span>](statedefinition.md) <br/> |<span data-ttu-id="eecd1-121">状態定義を指定します。</span><span class="sxs-lookup"><span data-stu-id="eecd1-121">Specifies a state definition.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="eecd1-122">注釈</span><span class="sxs-lookup"><span data-stu-id="eecd1-122">Remarks</span></span>

<span data-ttu-id="eecd1-123">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="eecd1-123">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="eecd1-124">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="eecd1-124">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eecd1-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="eecd1-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eecd1-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="eecd1-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="eecd1-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="eecd1-127">Schema Name</span></span>  <br/> |<span data-ttu-id="eecd1-128">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="eecd1-128">Type schema</span></span>  <br/> |
|<span data-ttu-id="eecd1-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="eecd1-129">Validation File</span></span>  <br/> |<span data-ttu-id="eecd1-130">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="eecd1-130">types.xsd</span></span>  <br/> |
|<span data-ttu-id="eecd1-131">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="eecd1-131">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="eecd1-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="eecd1-132">See also</span></span>

- [<span data-ttu-id="eecd1-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="eecd1-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

