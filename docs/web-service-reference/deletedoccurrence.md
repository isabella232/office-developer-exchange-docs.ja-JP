---
title: DeletedOccurrence
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeletedOccurrence
api_type:
- schema
ms.assetid: ff24ea15-0cd7-407d-a378-73ec16451870
description: DeletedOccurrence 要素は、定期的な予定表アイテムの削除済みアイテムを表します。
ms.openlocfilehash: f12a2ba20f87f7803e492d8422b68c8ecdf9d797
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759968"
---
# <a name="deletedoccurrence"></a><span data-ttu-id="7d26a-103">DeletedOccurrence</span><span class="sxs-lookup"><span data-stu-id="7d26a-103">DeletedOccurrence</span></span>

<span data-ttu-id="7d26a-104">**DeletedOccurrence**要素は、定期的な予定表アイテムの削除済みアイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="7d26a-104">The **DeletedOccurrence** element represents a deleted occurrence of a recurring calendar item.</span></span> 
  
```xml
<DeletedOccurrence>
   <Start/>
</DeletedOccurrence>
```

 <span data-ttu-id="7d26a-105">**DeletedOccurrenceInfoType**</span><span class="sxs-lookup"><span data-stu-id="7d26a-105">**DeletedOccurrenceInfoType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7d26a-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7d26a-106">Attributes and elements</span></span>

<span data-ttu-id="7d26a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7d26a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7d26a-108">属性</span><span class="sxs-lookup"><span data-stu-id="7d26a-108">Attributes</span></span>

<span data-ttu-id="7d26a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7d26a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7d26a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7d26a-110">Child elements</span></span>

|<span data-ttu-id="7d26a-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="7d26a-111">**Element**</span></span>|<span data-ttu-id="7d26a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7d26a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d26a-113">Start</span><span class="sxs-lookup"><span data-stu-id="7d26a-113">Start</span></span>](start.md) <br/> |<span data-ttu-id="7d26a-114">定期的な予定表アイテムの削除済みアイテムの開始時刻を表します。</span><span class="sxs-lookup"><span data-stu-id="7d26a-114">Represents the start time of a deleted occurrence of a recurring calendar item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7d26a-115">親要素</span><span class="sxs-lookup"><span data-stu-id="7d26a-115">Parent elements</span></span>

|<span data-ttu-id="7d26a-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="7d26a-116">**Element**</span></span>|<span data-ttu-id="7d26a-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="7d26a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7d26a-118">DeletedOccurrences</span><span class="sxs-lookup"><span data-stu-id="7d26a-118">DeletedOccurrences</span></span>](deletedoccurrences.md) <br/> |<span data-ttu-id="7d26a-119">定期的な予定表アイテムの削除済みアイテムの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7d26a-119">Contains an array of deleted occurrences of a recurring calendar item.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7d26a-120">備考</span><span class="sxs-lookup"><span data-stu-id="7d26a-120">Remarks</span></span>

<span data-ttu-id="7d26a-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="7d26a-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7d26a-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="7d26a-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7d26a-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="7d26a-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7d26a-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7d26a-124">Schema name</span></span>  <br/> |<span data-ttu-id="7d26a-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7d26a-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="7d26a-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7d26a-126">Validation file</span></span>  <br/> |<span data-ttu-id="7d26a-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7d26a-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7d26a-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7d26a-128">Can be empty</span></span>  <br/> |<span data-ttu-id="7d26a-129">False</span><span class="sxs-lookup"><span data-stu-id="7d26a-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7d26a-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="7d26a-130">See also</span></span>

- [<span data-ttu-id="7d26a-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7d26a-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)  
- <span data-ttu-id="7d26a-132">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="7d26a-132">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>

