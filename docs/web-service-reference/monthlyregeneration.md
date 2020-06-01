---
title: 月の明示再生
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MonthlyRegeneration
api_type:
- schema
ms.assetid: 9a52ca97-a663-41fe-b61a-61d8c53833ca
description: 月単位の再生要素には、タスクが再生成される頻度 (月数) を指定します。
ms.openlocfilehash: c941bc2606790646d2797df27c854996901c0bc6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462739"
---
# <a name="monthlyregeneration"></a><span data-ttu-id="cf15b-103">月の明示再生</span><span class="sxs-lookup"><span data-stu-id="cf15b-103">MonthlyRegeneration</span></span>

<span data-ttu-id="cf15b-104">月単位の**再生**要素には、タスクが再生成される頻度 (月数) を指定します。</span><span class="sxs-lookup"><span data-stu-id="cf15b-104">The **MonthlyRegeneration** element describes the frequency, in months, of which task is regenerated.</span></span> 
  
```xml
<MonthlyRegeneration>
   <Interval/>
</MonthlyRegeneration>
```

 <span data-ttu-id="cf15b-105">**MonthlyRegeneratingPatternType**</span><span class="sxs-lookup"><span data-stu-id="cf15b-105">**MonthlyRegeneratingPatternType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cf15b-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cf15b-106">Attributes and elements</span></span>

<span data-ttu-id="cf15b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cf15b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cf15b-108">属性</span><span class="sxs-lookup"><span data-stu-id="cf15b-108">Attributes</span></span>

<span data-ttu-id="cf15b-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cf15b-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cf15b-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cf15b-110">Child elements</span></span>

|<span data-ttu-id="cf15b-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="cf15b-111">**Element**</span></span>|<span data-ttu-id="cf15b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="cf15b-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf15b-113">間隔</span><span class="sxs-lookup"><span data-stu-id="cf15b-113">Interval</span></span>](interval.md) <br/> |<span data-ttu-id="cf15b-114">2つの連続する定期的なアイテム間の間隔 (月数) を定義します。</span><span class="sxs-lookup"><span data-stu-id="cf15b-114">Defines the interval, in months, between two consecutive recurring items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cf15b-115">親要素</span><span class="sxs-lookup"><span data-stu-id="cf15b-115">Parent elements</span></span>

|<span data-ttu-id="cf15b-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="cf15b-116">**Element**</span></span>|<span data-ttu-id="cf15b-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="cf15b-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cf15b-118">定期的なアイテム (TaskRecurrenceType)</span><span class="sxs-lookup"><span data-stu-id="cf15b-118">Recurrence (TaskRecurrenceType)</span></span>](recurrence-taskrecurrencetype.md) <br/> |<span data-ttu-id="cf15b-119">定期的なタスクの定期的なアイテムの情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cf15b-119">Contains recurrence information for recurring tasks.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cf15b-120">注釈</span><span class="sxs-lookup"><span data-stu-id="cf15b-120">Remarks</span></span>

<span data-ttu-id="cf15b-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="cf15b-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cf15b-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cf15b-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cf15b-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="cf15b-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cf15b-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cf15b-124">Schema name</span></span>  <br/> |<span data-ttu-id="cf15b-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="cf15b-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="cf15b-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cf15b-126">Validation file</span></span>  <br/> |<span data-ttu-id="cf15b-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="cf15b-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="cf15b-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cf15b-128">Can be empty</span></span>  <br/> |<span data-ttu-id="cf15b-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="cf15b-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cf15b-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="cf15b-130">See also</span></span>



- [<span data-ttu-id="cf15b-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="cf15b-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

