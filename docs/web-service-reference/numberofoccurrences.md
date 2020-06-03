---
title: NumberOfOccurrences
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- NumberOfOccurrences
api_type:
- schema
ms.assetid: 9ec86ceb-b271-4718-97ca-b6a532ea7223
description: NumberOfOccurrences 要素は、定期的なアイテムの発生回数を含みます。
ms.openlocfilehash: f9b72611e87c5f2b98deb14c25988e574a324491
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462543"
---
# <a name="numberofoccurrences"></a><span data-ttu-id="84777-103">NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="84777-103">NumberOfOccurrences</span></span>

<span data-ttu-id="84777-104">**Numberofoccurrences**要素は、定期的なアイテムの発生回数を含みます。</span><span class="sxs-lookup"><span data-stu-id="84777-104">The **NumberOfOccurrences** element contains the number of occurrences of a recurring item.</span></span> 
  
```xml
<NumberOfOccurrences/>
```

 <span data-ttu-id="84777-105">**int**</span><span class="sxs-lookup"><span data-stu-id="84777-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="84777-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="84777-106">Attributes and elements</span></span>

<span data-ttu-id="84777-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="84777-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="84777-108">属性</span><span class="sxs-lookup"><span data-stu-id="84777-108">Attributes</span></span>

<span data-ttu-id="84777-109">なし。</span><span class="sxs-lookup"><span data-stu-id="84777-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="84777-110">子要素</span><span class="sxs-lookup"><span data-stu-id="84777-110">Child elements</span></span>

<span data-ttu-id="84777-111">なし。</span><span class="sxs-lookup"><span data-stu-id="84777-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="84777-112">親要素</span><span class="sxs-lookup"><span data-stu-id="84777-112">Parent elements</span></span>

|<span data-ttu-id="84777-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="84777-113">**Element**</span></span>|<span data-ttu-id="84777-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="84777-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="84777-115">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="84777-115">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="84777-116">定期的なアイテムの開始日と発生回数を表します。</span><span class="sxs-lookup"><span data-stu-id="84777-116">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="84777-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="84777-117">Text value</span></span>

<span data-ttu-id="84777-118">テキスト値は、定期的なアイテムの出現回数を表す整数です。</span><span class="sxs-lookup"><span data-stu-id="84777-118">The text value is an integer that represents the number of occurrences of a recurring item.</span></span> <span data-ttu-id="84777-119">この値は、1 ~ 999 の範囲の整数である必要があります。</span><span class="sxs-lookup"><span data-stu-id="84777-119">The value must be an integer in the range of 1 to 999.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="84777-120">注釈</span><span class="sxs-lookup"><span data-stu-id="84777-120">Remarks</span></span>

<span data-ttu-id="84777-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="84777-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="84777-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="84777-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="84777-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="84777-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="84777-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="84777-124">Schema name</span></span>  <br/> |<span data-ttu-id="84777-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="84777-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="84777-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="84777-126">Validation file</span></span>  <br/> |<span data-ttu-id="84777-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="84777-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="84777-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="84777-128">Can be empty</span></span>  <br/> |<span data-ttu-id="84777-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="84777-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="84777-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="84777-130">See also</span></span>



- [<span data-ttu-id="84777-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="84777-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

