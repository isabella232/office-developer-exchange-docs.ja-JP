---
title: 出現
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Occurrence
api_type:
- schema
ms.assetid: d292b99c-b896-40b7-be5d-2cb314c9481f
description: 見つかった要素では、定期的な予定表アイテムの 1 つの変更されたアイテムを表します。
ms.openlocfilehash: 5a40faa9b885a235d30e7f41830d1eefe2ed23c3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832653"
---
# <a name="occurrence"></a><span data-ttu-id="a20c6-103">出現</span><span class="sxs-lookup"><span data-stu-id="a20c6-103">Occurrence</span></span>

<span data-ttu-id="a20c6-104">**見つかった**要素では、定期的な予定表アイテムの 1 つの変更されたアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="a20c6-104">The **Occurrence** element represents a single modified occurrence of a recurring calendar item.</span></span> 
  
```xml
<Occurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</Occurrence>
```

<span data-ttu-id="a20c6-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="a20c6-105">**OccurrenceInfoType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a20c6-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a20c6-106">Attributes and elements</span></span>

<span data-ttu-id="a20c6-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a20c6-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a20c6-108">属性</span><span class="sxs-lookup"><span data-stu-id="a20c6-108">Attributes</span></span>

<span data-ttu-id="a20c6-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a20c6-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a20c6-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a20c6-110">Child elements</span></span>

|<span data-ttu-id="a20c6-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="a20c6-111">**Element**</span></span>|<span data-ttu-id="a20c6-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="a20c6-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a20c6-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="a20c6-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="a20c6-114">定期的な予定表アイテムに変更されたアイテムの一意の識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a20c6-114">Contains the unique identifier and change key of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="a20c6-115">Start</span><span class="sxs-lookup"><span data-stu-id="a20c6-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="a20c6-116">定期的な予定表アイテムに変更されたアイテムの開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="a20c6-116">Represents the start time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="a20c6-117">終わり</span><span class="sxs-lookup"><span data-stu-id="a20c6-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="a20c6-118">定期的な予定表アイテムに変更されたアイテムの終了時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="a20c6-118">Represents the end time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="a20c6-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="a20c6-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="a20c6-120">定期的な予定表アイテムに変更されたアイテムの元の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="a20c6-120">Represents the original start time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a20c6-121">親要素</span><span class="sxs-lookup"><span data-stu-id="a20c6-121">Parent elements</span></span>

|<span data-ttu-id="a20c6-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="a20c6-122">**Element**</span></span>|<span data-ttu-id="a20c6-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="a20c6-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a20c6-124">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="a20c6-124">ModifiedOccurrences</span></span>](modifiedoccurrences.md) <br/> |<span data-ttu-id="a20c6-125">定期的な予定のマスター アイテムとは異なるものに変更された定期的な予定表アイテム アイテムのコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a20c6-125">Contains a collection of recurring calendar item occurrences that have been modified so that they are different than the recurrence master item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a20c6-126">備考</span><span class="sxs-lookup"><span data-stu-id="a20c6-126">Remarks</span></span>

<span data-ttu-id="a20c6-127">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="a20c6-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a20c6-128">要素情報</span><span class="sxs-lookup"><span data-stu-id="a20c6-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a20c6-129">名前空間</span><span class="sxs-lookup"><span data-stu-id="a20c6-129">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a20c6-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a20c6-130">Schema name</span></span>  <br/> |<span data-ttu-id="a20c6-131">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a20c6-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="a20c6-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a20c6-132">Validation file</span></span>  <br/> |<span data-ttu-id="a20c6-133">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a20c6-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a20c6-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a20c6-134">Can be empty</span></span>  <br/> |<span data-ttu-id="a20c6-135">False</span><span class="sxs-lookup"><span data-stu-id="a20c6-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a20c6-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="a20c6-136">See also</span></span>

- [<span data-ttu-id="a20c6-137">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a20c6-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

