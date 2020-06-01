---
title: 発生
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
description: オカレンスリンク要素は、定期的な予定表アイテムの1つの変更されたオカレンスを表します。
ms.openlocfilehash: c3a6bcce23f0bb1125dbd2a5bb86e9b20039a4e1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466319"
---
# <a name="occurrence"></a><span data-ttu-id="55df2-103">発生</span><span class="sxs-lookup"><span data-stu-id="55df2-103">Occurrence</span></span>

<span data-ttu-id="55df2-104">**オカレンスリンク**要素は、定期的な予定表アイテムの1つの変更されたオカレンスを表します。</span><span class="sxs-lookup"><span data-stu-id="55df2-104">The **Occurrence** element represents a single modified occurrence of a recurring calendar item.</span></span> 
  
```xml
<Occurrence>
   <ItemId/>
   <Start/>
   <End/>
   <OriginalStart/>
</Occurrence>
```

<span data-ttu-id="55df2-105">**OccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="55df2-105">**OccurrenceInfoType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="55df2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="55df2-106">Attributes and elements</span></span>

<span data-ttu-id="55df2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="55df2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55df2-108">属性</span><span class="sxs-lookup"><span data-stu-id="55df2-108">Attributes</span></span>

<span data-ttu-id="55df2-109">なし。</span><span class="sxs-lookup"><span data-stu-id="55df2-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55df2-110">子要素</span><span class="sxs-lookup"><span data-stu-id="55df2-110">Child elements</span></span>

|<span data-ttu-id="55df2-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="55df2-111">**Element**</span></span>|<span data-ttu-id="55df2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="55df2-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55df2-113">ItemId</span><span class="sxs-lookup"><span data-stu-id="55df2-113">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="55df2-114">定期的な予定表アイテムの変更されたアイテムの一意識別子および変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="55df2-114">Contains the unique identifier and change key of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="55df2-115">開始</span><span class="sxs-lookup"><span data-stu-id="55df2-115">Start</span></span>](start.md) <br/> |<span data-ttu-id="55df2-116">定期的な予定表アイテムの変更された発生の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="55df2-116">Represents the start time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="55df2-117">終わり</span><span class="sxs-lookup"><span data-stu-id="55df2-117">End </span></span>](end-ex15websvcsotherref.md) <br/> |<span data-ttu-id="55df2-118">定期的な予定表アイテムの変更された発生の終了時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="55df2-118">Represents the end time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
|[<span data-ttu-id="55df2-119">OriginalStart</span><span class="sxs-lookup"><span data-stu-id="55df2-119">OriginalStart</span></span>](originalstart.md) <br/> |<span data-ttu-id="55df2-120">定期的な予定表アイテムの変更された発生の元の開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="55df2-120">Represents the original start time of a modified occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="55df2-121">親要素</span><span class="sxs-lookup"><span data-stu-id="55df2-121">Parent elements</span></span>

|<span data-ttu-id="55df2-122">**要素**</span><span class="sxs-lookup"><span data-stu-id="55df2-122">**Element**</span></span>|<span data-ttu-id="55df2-123">**説明**</span><span class="sxs-lookup"><span data-stu-id="55df2-123">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55df2-124">ModifiedOccurrences</span><span class="sxs-lookup"><span data-stu-id="55df2-124">ModifiedOccurrences</span></span>](modifiedoccurrences.md) <br/> |<span data-ttu-id="55df2-125">定期的な予定表アイテムのコレクションが含まれています。これは、定期的なアイテムのマスターアイテムとは異なるように変更されています。</span><span class="sxs-lookup"><span data-stu-id="55df2-125">Contains a collection of recurring calendar item occurrences that have been modified so that they are different than the recurrence master item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="55df2-126">注釈</span><span class="sxs-lookup"><span data-stu-id="55df2-126">Remarks</span></span>

<span data-ttu-id="55df2-127">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="55df2-127">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55df2-128">要素の情報</span><span class="sxs-lookup"><span data-stu-id="55df2-128">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55df2-129">Namespace</span><span class="sxs-lookup"><span data-stu-id="55df2-129">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="55df2-130">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="55df2-130">Schema name</span></span>  <br/> |<span data-ttu-id="55df2-131">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="55df2-131">Types schema</span></span>  <br/> |
|<span data-ttu-id="55df2-132">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="55df2-132">Validation file</span></span>  <br/> |<span data-ttu-id="55df2-133">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="55df2-133">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="55df2-134">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="55df2-134">Can be empty</span></span>  <br/> |<span data-ttu-id="55df2-135">正しくない</span><span class="sxs-lookup"><span data-stu-id="55df2-135">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55df2-136">関連項目</span><span class="sxs-lookup"><span data-stu-id="55df2-136">See also</span></span>

- [<span data-ttu-id="55df2-137">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="55df2-137">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

