---
title: ビットマスク
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Bitmask
api_type:
- schema
ms.assetid: fc7eeac2-555f-4cbc-8b48-26d9ed67748a
description: Excludes 制限操作時に使用する 16 進数または 10 進数のマスクを表すビットマスク要素。
ms.openlocfilehash: 86c8c61f22d8d620a9139280b2a43ed7fec4727d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759517"
---
# <a name="bitmask"></a><span data-ttu-id="d4fb1-103">ビットマスク</span><span class="sxs-lookup"><span data-stu-id="d4fb1-103">Bitmask</span></span>

<span data-ttu-id="d4fb1-104">[Excludes](excludes.md)制限操作時に使用する 16 進数または 10 進数のマスクを表す**ビットマスク**要素。</span><span class="sxs-lookup"><span data-stu-id="d4fb1-104">The **Bitmask** element represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> 
  
```xml
<Bitmask Value="" />
```

<span data-ttu-id="d4fb1-105">**ExcludesValueType**</span><span class="sxs-lookup"><span data-stu-id="d4fb1-105">**ExcludesValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="d4fb1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d4fb1-106">Attributes and elements</span></span>

<span data-ttu-id="d4fb1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d4fb1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d4fb1-108">属性</span><span class="sxs-lookup"><span data-stu-id="d4fb1-108">Attributes</span></span>

|<span data-ttu-id="d4fb1-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="d4fb1-109">**Attribute**</span></span>|<span data-ttu-id="d4fb1-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="d4fb1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d4fb1-111">**Value**</span><span class="sxs-lookup"><span data-stu-id="d4fb1-111">**Value**</span></span> | <span data-ttu-id="d4fb1-112">10 進または 16 進数のビットマスクを表します。</span><span class="sxs-lookup"><span data-stu-id="d4fb1-112">Represents a decimal or hexadecimal bitmask.</span></span> <span data-ttu-id="d4fb1-113">値は、次の正規表現で表されます。</span><span class="sxs-lookup"><span data-stu-id="d4fb1-113">The value is represented by the following regular expression:</span></span><br/><span data-ttu-id="d4fb1-114">' ((0 x</span><span class="sxs-lookup"><span data-stu-id="d4fb1-114">\`((0x</span></span>|<span data-ttu-id="d4fb1-115">0X)[0-9A-Fa-f]\*)</span><span class="sxs-lookup"><span data-stu-id="d4fb1-115">0X)[0-9A-Fa-f]\*)</span></span>|<span data-ttu-id="d4fb1-116">([0-9] \*)'。</span><span class="sxs-lookup"><span data-stu-id="d4fb1-116">([0-9]\*)\`.</span></span><br/><br/><span data-ttu-id="d4fb1-117">次に、この属性の値を 16 進数の例を示します。</span><span class="sxs-lookup"><span data-stu-id="d4fb1-117">The following are examples of hexadecimal values for this attribute:</span></span><br/><span data-ttu-id="d4fb1-118">-0x12AF</span><span class="sxs-lookup"><span data-stu-id="d4fb1-118">- 0x12AF</span></span><br/><span data-ttu-id="d4fb1-119">-0X334AE</span><span class="sxs-lookup"><span data-stu-id="d4fb1-119">- 0X334AE</span></span><br/><br/><span data-ttu-id="d4fb1-120">次に、この属性の値を 10 進数の例を示します。</span><span class="sxs-lookup"><span data-stu-id="d4fb1-120">The following are examples of decimal values for this attribute:</span></span><br/><span data-ttu-id="d4fb1-121">-10</span><span class="sxs-lookup"><span data-stu-id="d4fb1-121">- 10</span></span><br/><span data-ttu-id="d4fb1-122">-255</span><span class="sxs-lookup"><span data-stu-id="d4fb1-122">- 255</span></span><br/><span data-ttu-id="d4fb1-123">-4562</span><span class="sxs-lookup"><span data-stu-id="d4fb1-123">- 4562</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="d4fb1-124">子要素</span><span class="sxs-lookup"><span data-stu-id="d4fb1-124">Child elements</span></span>

<span data-ttu-id="d4fb1-125">なし。</span><span class="sxs-lookup"><span data-stu-id="d4fb1-125">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d4fb1-126">親要素</span><span class="sxs-lookup"><span data-stu-id="d4fb1-126">Parent elements</span></span>

|<span data-ttu-id="d4fb1-127">**要素**</span><span class="sxs-lookup"><span data-stu-id="d4fb1-127">**Element**</span></span>|<span data-ttu-id="d4fb1-128">**説明**</span><span class="sxs-lookup"><span data-stu-id="d4fb1-128">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d4fb1-129">除外</span><span class="sxs-lookup"><span data-stu-id="d4fb1-129">Excludes</span></span>](excludes.md) <br/> |<span data-ttu-id="d4fb1-130">プロパティのビットごとのマスクを実行します。</span><span class="sxs-lookup"><span data-stu-id="d4fb1-130">Performs a bitwise mask of the properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d4fb1-131">備考</span><span class="sxs-lookup"><span data-stu-id="d4fb1-131">Remarks</span></span>

<span data-ttu-id="d4fb1-132">16 進数の値には、プレフィックス 0x または 0x が必要です。</span><span class="sxs-lookup"><span data-stu-id="d4fb1-132">Hexadecimal values must have a prefix of either 0x or 0X.</span></span> <span data-ttu-id="d4fb1-133">このプレフィックスが存在しない場合、値は 10 進数と見なされます。</span><span class="sxs-lookup"><span data-stu-id="d4fb1-133">If this prefix does not exist, the value is assumed to be a decimal number.</span></span>
  
<span data-ttu-id="d4fb1-134">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="d4fb1-134">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d4fb1-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="d4fb1-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d4fb1-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="d4fb1-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d4fb1-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d4fb1-137">Schema name</span></span>  <br/> |<span data-ttu-id="d4fb1-138">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d4fb1-138">Types schema</span></span>  <br/> |
|<span data-ttu-id="d4fb1-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d4fb1-139">Validation file</span></span>  <br/> |<span data-ttu-id="d4fb1-140">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d4fb1-140">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d4fb1-141">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d4fb1-141">Can be empty</span></span>  <br/> |<span data-ttu-id="d4fb1-142">False</span><span class="sxs-lookup"><span data-stu-id="d4fb1-142">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d4fb1-143">関連項目</span><span class="sxs-lookup"><span data-stu-id="d4fb1-143">See also</span></span>

- [<span data-ttu-id="d4fb1-144">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d4fb1-144">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

