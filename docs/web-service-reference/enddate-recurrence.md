---
title: 終了日 (繰り返し)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndDate
api_type:
- schema
ms.assetid: 16026595-26f8-4770-8a6d-0d3e4157effd
description: 終了要素では、定期的な仕事または EndDateRecurrence パターンの種類のある予定表アイテムの終了日を表します。
ms.openlocfilehash: b8570a069fc0a2d05044a9c85ab2d5c39d70ccdf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760279"
---
# <a name="enddate-recurrence"></a><span data-ttu-id="d2107-103">終了日 (繰り返し)</span><span class="sxs-lookup"><span data-stu-id="d2107-103">EndDate (Recurrence)</span></span>

<span data-ttu-id="d2107-104">**終了**要素では、定期的な仕事または EndDateRecurrence パターンの種類のある予定表アイテムの終了日を表します。</span><span class="sxs-lookup"><span data-stu-id="d2107-104">The **EndDate** element represents the end date of a recurring task or a calendar item that has the EndDateRecurrence pattern type.</span></span> 
  
```xml
<EndDate/>
```

 <span data-ttu-id="d2107-105">**date**</span><span class="sxs-lookup"><span data-stu-id="d2107-105">**date**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2107-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d2107-106">Attributes and elements</span></span>

<span data-ttu-id="d2107-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d2107-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2107-108">属性</span><span class="sxs-lookup"><span data-stu-id="d2107-108">Attributes</span></span>

<span data-ttu-id="d2107-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d2107-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2107-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d2107-110">Child elements</span></span>

<span data-ttu-id="d2107-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d2107-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d2107-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d2107-112">Parent elements</span></span>

|<span data-ttu-id="d2107-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="d2107-113">**Element**</span></span>|<span data-ttu-id="d2107-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2107-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2107-115">EndDateRecurrence</span><span class="sxs-lookup"><span data-stu-id="d2107-115">EndDateRecurrence</span></span>](enddaterecurrence.md) <br/> |<span data-ttu-id="d2107-116">開始日と終了日の項目の定期的なパターンについて説明します。</span><span class="sxs-lookup"><span data-stu-id="d2107-116">Describes the start date and the end date of an item recurrence pattern.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d2107-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d2107-117">Text value</span></span>

<span data-ttu-id="d2107-118">日付を表すテキスト値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="d2107-118">A text value that represents a date is required if this element is used.</span></span> <span data-ttu-id="d2107-119">値が 4500 年 9 月 1 日より大きくすることはできません 00時 00分: 00 です。</span><span class="sxs-lookup"><span data-stu-id="d2107-119">The value cannot be larger than September 1, 4500 00:00:00.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d2107-120">備考</span><span class="sxs-lookup"><span data-stu-id="d2107-120">Remarks</span></span>

<span data-ttu-id="d2107-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="d2107-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2107-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="d2107-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2107-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="d2107-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d2107-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d2107-124">Schema name</span></span>  <br/> |<span data-ttu-id="d2107-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d2107-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="d2107-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d2107-126">Validation file</span></span>  <br/> |<span data-ttu-id="d2107-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d2107-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d2107-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d2107-128">Can be empty</span></span>  <br/> |<span data-ttu-id="d2107-129">False</span><span class="sxs-lookup"><span data-stu-id="d2107-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2107-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="d2107-130">See also</span></span>



- [<span data-ttu-id="d2107-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d2107-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

