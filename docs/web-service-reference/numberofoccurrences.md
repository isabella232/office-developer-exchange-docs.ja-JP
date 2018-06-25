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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832656"
---
# <a name="numberofoccurrences"></a><span data-ttu-id="82c07-103">NumberOfOccurrences</span><span class="sxs-lookup"><span data-stu-id="82c07-103">NumberOfOccurrences</span></span>

<span data-ttu-id="82c07-104">**NumberOfOccurrences**要素には、定期的なアイテムの出現回数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="82c07-104">The **NumberOfOccurrences** element contains the number of occurrences of a recurring item.</span></span> 
  
```xml
<NumberOfOccurrences/>
```

 <span data-ttu-id="82c07-105">**int**</span><span class="sxs-lookup"><span data-stu-id="82c07-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="82c07-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="82c07-106">Attributes and elements</span></span>

<span data-ttu-id="82c07-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="82c07-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="82c07-108">属性</span><span class="sxs-lookup"><span data-stu-id="82c07-108">Attributes</span></span>

<span data-ttu-id="82c07-109">なし。</span><span class="sxs-lookup"><span data-stu-id="82c07-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="82c07-110">子要素</span><span class="sxs-lookup"><span data-stu-id="82c07-110">Child elements</span></span>

<span data-ttu-id="82c07-111">なし。</span><span class="sxs-lookup"><span data-stu-id="82c07-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="82c07-112">親要素</span><span class="sxs-lookup"><span data-stu-id="82c07-112">Parent elements</span></span>

|<span data-ttu-id="82c07-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="82c07-113">**Element**</span></span>|<span data-ttu-id="82c07-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="82c07-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="82c07-115">NumberedRecurrence</span><span class="sxs-lookup"><span data-stu-id="82c07-115">NumberedRecurrence</span></span>](numberedrecurrence.md) <br/> |<span data-ttu-id="82c07-116">開始日と定期的なアイテムの出現回数を説明します。</span><span class="sxs-lookup"><span data-stu-id="82c07-116">Describes the start date and the number of occurrences of a recurring item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="82c07-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="82c07-117">Text value</span></span>

<span data-ttu-id="82c07-118">テキスト値は、定期的なアイテムの出現回数を表す整数です。</span><span class="sxs-lookup"><span data-stu-id="82c07-118">The text value is an integer that represents the number of occurrences of a recurring item.</span></span> <span data-ttu-id="82c07-119">値は 1 ~ 999 の範囲の整数である必要があります。</span><span class="sxs-lookup"><span data-stu-id="82c07-119">The value must be an integer in the range of 1 to 999.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="82c07-120">備考</span><span class="sxs-lookup"><span data-stu-id="82c07-120">Remarks</span></span>

<span data-ttu-id="82c07-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="82c07-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="82c07-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="82c07-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="82c07-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="82c07-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="82c07-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="82c07-124">Schema name</span></span>  <br/> |<span data-ttu-id="82c07-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="82c07-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="82c07-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="82c07-126">Validation file</span></span>  <br/> |<span data-ttu-id="82c07-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="82c07-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="82c07-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="82c07-128">Can be empty</span></span>  <br/> |<span data-ttu-id="82c07-129">False</span><span class="sxs-lookup"><span data-stu-id="82c07-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="82c07-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="82c07-130">See also</span></span>



- [<span data-ttu-id="82c07-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="82c07-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

