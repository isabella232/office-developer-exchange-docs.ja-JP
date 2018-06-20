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
description: NumberOfOccurrences 要素には、定期的なアイテムの出現回数が含まれています。
ms.openlocfilehash: c18a20f14395aead304bd0158ff64c70e51ec165
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832656"
---
# <a name="numberofoccurrences"></a><span data-ttu-id="e7531-103">NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="e7531-103">NumberOfOccurrences</span></span>

<span data-ttu-id="e7531-104">**NumberOfOccurrences**要素には、定期的なアイテムの出現回数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e7531-104">The **NumberOfOccurrences** element contains the number of occurrences of a recurring item.</span></span> 
  
```xml
<NumberOfOccurrences/>
```

 <span data-ttu-id="e7531-105">**int**</span><span class="sxs-lookup"><span data-stu-id="e7531-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e7531-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e7531-106">Attributes and elements</span></span>

<span data-ttu-id="e7531-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e7531-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e7531-108">属性</span><span class="sxs-lookup"><span data-stu-id="e7531-108">Attributes</span></span>

<span data-ttu-id="e7531-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e7531-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e7531-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e7531-110">Child elements</span></span>

<span data-ttu-id="e7531-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e7531-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e7531-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e7531-112">Parent elements</span></span>

|<span data-ttu-id="e7531-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e7531-113">**Element**</span></span>|<span data-ttu-id="e7531-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e7531-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e7531-115">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="e7531-115">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="e7531-116">開始日と定期的なアイテムの出現回数を説明します。</span><span class="sxs-lookup"><span data-stu-id="e7531-116">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e7531-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e7531-117">Text value</span></span>

<span data-ttu-id="e7531-118">テキスト値は、定期的なアイテムの出現回数を表す整数です。</span><span class="sxs-lookup"><span data-stu-id="e7531-118">The text value is an integer that represents the number of occurrences of a recurring item.</span></span> <span data-ttu-id="e7531-119">値は 1 ~ 999 の範囲の整数である必要があります。</span><span class="sxs-lookup"><span data-stu-id="e7531-119">The value must be an integer in the range of 1 to 999.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e7531-120">備考</span><span class="sxs-lookup"><span data-stu-id="e7531-120">Remarks</span></span>

<span data-ttu-id="e7531-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="e7531-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e7531-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="e7531-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e7531-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="e7531-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e7531-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e7531-124">Schema name</span></span>  <br/> |<span data-ttu-id="e7531-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e7531-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="e7531-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e7531-126">Validation file</span></span>  <br/> |<span data-ttu-id="e7531-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e7531-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e7531-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e7531-128">Can be empty</span></span>  <br/> |<span data-ttu-id="e7531-129">False</span><span class="sxs-lookup"><span data-stu-id="e7531-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e7531-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="e7531-130">See also</span></span>



- [<span data-ttu-id="e7531-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e7531-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

