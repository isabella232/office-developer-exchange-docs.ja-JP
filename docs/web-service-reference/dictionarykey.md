---
title: DictionaryKey
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DictionaryKey
api_type:
- schema
ms.assetid: f331c8ac-f1c7-4248-a570-97701969d5bf
description: DictionaryKey 要素は、ディクショナリ プロパティのディクショナリのキーを指定します。
ms.openlocfilehash: 7e706f16fe155278ea56f303ffbb5971c1779879
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760039"
---
# <a name="dictionarykey"></a><span data-ttu-id="d3ffc-103">DictionaryKey</span><span class="sxs-lookup"><span data-stu-id="d3ffc-103">DictionaryKey</span></span>

<span data-ttu-id="d3ffc-104">**DictionaryKey**要素は、ディクショナリ プロパティのディクショナリのキーを指定します。</span><span class="sxs-lookup"><span data-stu-id="d3ffc-104">The **DictionaryKey** element specifies the dictionary key for a dictionary property.</span></span> 
  
```xml
<DictionaryKey>
   <Type/>
   <Value/>
</DictionaryKey>
```

 <span data-ttu-id="d3ffc-105">**UserConfigurationDictionaryObjectType**</span><span class="sxs-lookup"><span data-stu-id="d3ffc-105">**UserConfigurationDictionaryObjectType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d3ffc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d3ffc-106">Attributes and elements</span></span>

<span data-ttu-id="d3ffc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d3ffc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d3ffc-108">属性</span><span class="sxs-lookup"><span data-stu-id="d3ffc-108">Attributes</span></span>

<span data-ttu-id="d3ffc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d3ffc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d3ffc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d3ffc-110">Child elements</span></span>

|<span data-ttu-id="d3ffc-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d3ffc-111">**Element**</span></span>|<span data-ttu-id="d3ffc-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d3ffc-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3ffc-113">型 (UserConfiguration)</span><span class="sxs-lookup"><span data-stu-id="d3ffc-113">Type (UserConfiguration)</span></span>](type-userconfiguration.md) <br/> | <span data-ttu-id="d3ffc-114">ディクショナリ オブジェクトの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="d3ffc-114">Specifies a dictionary object type.</span></span><br/><br/><span data-ttu-id="d3ffc-115">型には、次の文字列値のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="d3ffc-115">The type can be one of the following string values:</span></span><br/><br/><span data-ttu-id="d3ffc-116">-日時</span><span class="sxs-lookup"><span data-stu-id="d3ffc-116">-  DateTime</span></span>  <br/><span data-ttu-id="d3ffc-117">-ブール値</span><span class="sxs-lookup"><span data-stu-id="d3ffc-117">-  Boolean</span></span>  <br/><span data-ttu-id="d3ffc-118">バイト</span><span class="sxs-lookup"><span data-stu-id="d3ffc-118">-  Byte</span></span>  <br/><span data-ttu-id="d3ffc-119">文字列</span><span class="sxs-lookup"><span data-stu-id="d3ffc-119">-  String</span></span>  <br/><span data-ttu-id="d3ffc-120">-Integer32</span><span class="sxs-lookup"><span data-stu-id="d3ffc-120">-  Integer32</span></span>  <br/><span data-ttu-id="d3ffc-121">-UnsignedInteger32</span><span class="sxs-lookup"><span data-stu-id="d3ffc-121">-  UnsignedInteger32</span></span>  <br/><span data-ttu-id="d3ffc-122">-Integer64</span><span class="sxs-lookup"><span data-stu-id="d3ffc-122">-  Integer64</span></span>  <br/><span data-ttu-id="d3ffc-123">-UnsignedInteger64</span><span class="sxs-lookup"><span data-stu-id="d3ffc-123">-  UnsignedInteger64</span></span>  <br/><span data-ttu-id="d3ffc-124">-自己責任で使用</span><span class="sxs-lookup"><span data-stu-id="d3ffc-124">-  StringArray</span></span>  <br/><span data-ttu-id="d3ffc-125">-ByteArray</span><span class="sxs-lookup"><span data-stu-id="d3ffc-125">-  ByteArray</span></span>  <br/> |
|[<span data-ttu-id="d3ffc-126">値 (UserConfiguration)</span><span class="sxs-lookup"><span data-stu-id="d3ffc-126">Value (UserConfiguration)</span></span>](value-userconfiguration.md) <br/> |<span data-ttu-id="d3ffc-127">ディクショナリ オブジェクトの値を文字列として指定します。</span><span class="sxs-lookup"><span data-stu-id="d3ffc-127">Specifies the dictionary object value as a string.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d3ffc-128">親要素</span><span class="sxs-lookup"><span data-stu-id="d3ffc-128">Parent elements</span></span>

|<span data-ttu-id="d3ffc-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="d3ffc-129">**Element**</span></span>|<span data-ttu-id="d3ffc-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="d3ffc-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d3ffc-131">DictionaryEntry</span><span class="sxs-lookup"><span data-stu-id="d3ffc-131">DictionaryEntry</span></span>](dictionaryentry.md) <br/> |<span data-ttu-id="d3ffc-132">1 つのディクショナリ エントリのプロパティの内容を指定します。</span><span class="sxs-lookup"><span data-stu-id="d3ffc-132">Specifies the contents of a single dictionary entry property.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="d3ffc-133">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d3ffc-133">Text value</span></span>

<span data-ttu-id="d3ffc-134">なし。</span><span class="sxs-lookup"><span data-stu-id="d3ffc-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d3ffc-135">備考</span><span class="sxs-lookup"><span data-stu-id="d3ffc-135">Remarks</span></span>

<span data-ttu-id="d3ffc-136">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d3ffc-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d3ffc-137">要素情報</span><span class="sxs-lookup"><span data-stu-id="d3ffc-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d3ffc-138">名前空間</span><span class="sxs-lookup"><span data-stu-id="d3ffc-138">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d3ffc-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d3ffc-139">Schema Name</span></span>  <br/> |<span data-ttu-id="d3ffc-140">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="d3ffc-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="d3ffc-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d3ffc-141">Validation File</span></span>  <br/> |<span data-ttu-id="d3ffc-142">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="d3ffc-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d3ffc-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d3ffc-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="d3ffc-144">False</span><span class="sxs-lookup"><span data-stu-id="d3ffc-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d3ffc-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="d3ffc-145">See also</span></span>

- [<span data-ttu-id="d3ffc-146">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d3ffc-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

