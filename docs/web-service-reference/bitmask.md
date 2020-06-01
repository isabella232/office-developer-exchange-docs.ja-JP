---
title: 示す
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
description: ビットマスク要素は、除外制限操作の間に使用される16進数または10進数のマスクを表します。
ms.openlocfilehash: f05be466d05b13f8f362afb5fc0552653a532475
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458811"
---
# <a name="bitmask"></a><span data-ttu-id="7ce86-103">示す</span><span class="sxs-lookup"><span data-stu-id="7ce86-103">Bitmask</span></span>

<span data-ttu-id="7ce86-104">**ビットマスク**要素は、[除外](excludes.md)制限操作の間に使用される16進数または10進数のマスクを表します。</span><span class="sxs-lookup"><span data-stu-id="7ce86-104">The **Bitmask** element represents a hexadecimal or decimal mask to be used during an [Excludes](excludes.md) restriction operation.</span></span> 
  
```xml
<Bitmask Value="" />
```

<span data-ttu-id="7ce86-105">**ExcludesValueType**</span><span class="sxs-lookup"><span data-stu-id="7ce86-105">**ExcludesValueType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7ce86-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7ce86-106">Attributes and elements</span></span>

<span data-ttu-id="7ce86-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7ce86-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ce86-108">属性</span><span class="sxs-lookup"><span data-stu-id="7ce86-108">Attributes</span></span>

|<span data-ttu-id="7ce86-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="7ce86-109">**Attribute**</span></span>|<span data-ttu-id="7ce86-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="7ce86-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7ce86-111">**値**</span><span class="sxs-lookup"><span data-stu-id="7ce86-111">**Value**</span></span> | <span data-ttu-id="7ce86-112">10進数または16進数のビットマスクを表します。</span><span class="sxs-lookup"><span data-stu-id="7ce86-112">Represents a decimal or hexadecimal bitmask.</span></span> <span data-ttu-id="7ce86-113">この値は、次の正規表現で表されます。</span><span class="sxs-lookup"><span data-stu-id="7ce86-113">The value is represented by the following regular expression:</span></span><br/><span data-ttu-id="7ce86-114">`((0x|0X)[0-9A-Fa-f]*)|([0-9]*)`.</span><span class="sxs-lookup"><span data-stu-id="7ce86-114">`((0x|0X)[0-9A-Fa-f]*)|([0-9]*)`.</span></span><br/><br/><span data-ttu-id="7ce86-115">この属性の16進値の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ce86-115">The following are examples of hexadecimal values for this attribute:</span></span><br/><span data-ttu-id="7ce86-116">- 0x12AF</span><span class="sxs-lookup"><span data-stu-id="7ce86-116">- 0x12AF</span></span><br/><span data-ttu-id="7ce86-117">- 0X334AE</span><span class="sxs-lookup"><span data-stu-id="7ce86-117">- 0X334AE</span></span><br/><br/><span data-ttu-id="7ce86-118">この属性の10進値の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ce86-118">The following are examples of decimal values for this attribute:</span></span><br/><span data-ttu-id="7ce86-119">-10</span><span class="sxs-lookup"><span data-stu-id="7ce86-119">- 10</span></span><br/><span data-ttu-id="7ce86-120">-255</span><span class="sxs-lookup"><span data-stu-id="7ce86-120">- 255</span></span><br/><span data-ttu-id="7ce86-121">-4562</span><span class="sxs-lookup"><span data-stu-id="7ce86-121">- 4562</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="7ce86-122">子要素</span><span class="sxs-lookup"><span data-stu-id="7ce86-122">Child elements</span></span>

<span data-ttu-id="7ce86-123">なし。</span><span class="sxs-lookup"><span data-stu-id="7ce86-123">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="7ce86-124">親要素</span><span class="sxs-lookup"><span data-stu-id="7ce86-124">Parent elements</span></span>

|<span data-ttu-id="7ce86-125">**要素**</span><span class="sxs-lookup"><span data-stu-id="7ce86-125">**Element**</span></span>|<span data-ttu-id="7ce86-126">**説明**</span><span class="sxs-lookup"><span data-stu-id="7ce86-126">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ce86-127">Excludes</span><span class="sxs-lookup"><span data-stu-id="7ce86-127">Excludes</span></span>](excludes.md) <br/> |<span data-ttu-id="7ce86-128">プロパティのビット単位のマスクを実行します。</span><span class="sxs-lookup"><span data-stu-id="7ce86-128">Performs a bitwise mask of the properties.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7ce86-129">注釈</span><span class="sxs-lookup"><span data-stu-id="7ce86-129">Remarks</span></span>

<span data-ttu-id="7ce86-130">16進数の値のプレフィックスは、0x または0X である必要があります。</span><span class="sxs-lookup"><span data-stu-id="7ce86-130">Hexadecimal values must have a prefix of either 0x or 0X.</span></span> <span data-ttu-id="7ce86-131">このプレフィックスが存在しない場合、値は10進数値と見なされます。</span><span class="sxs-lookup"><span data-stu-id="7ce86-131">If this prefix does not exist, the value is assumed to be a decimal number.</span></span>
  
<span data-ttu-id="7ce86-132">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7ce86-132">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ce86-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7ce86-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ce86-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="7ce86-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7ce86-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7ce86-135">Schema name</span></span>  <br/> |<span data-ttu-id="7ce86-136">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7ce86-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="7ce86-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7ce86-137">Validation file</span></span>  <br/> |<span data-ttu-id="7ce86-138">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7ce86-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7ce86-139">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7ce86-139">Can be empty</span></span>  <br/> |<span data-ttu-id="7ce86-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="7ce86-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ce86-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="7ce86-141">See also</span></span>

- [<span data-ttu-id="7ce86-142">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7ce86-142">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

