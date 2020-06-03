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
description: DictionaryKey 要素は、dictionary プロパティの辞書キーを指定します。
ms.openlocfilehash: 8d9d897c86eb5048068936433c6c0d77917ff777
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462151"
---
# <a name="dictionarykey"></a><span data-ttu-id="8d9c3-103">DictionaryKey</span><span class="sxs-lookup"><span data-stu-id="8d9c3-103">DictionaryKey</span></span>

<span data-ttu-id="8d9c3-104">**Dictionarykey**要素は、dictionary プロパティの辞書キーを指定します。</span><span class="sxs-lookup"><span data-stu-id="8d9c3-104">The **DictionaryKey** element specifies the dictionary key for a dictionary property.</span></span> 
  
```xml
<DictionaryKey>
   <Type/>
   <Value/>
</DictionaryKey>
```

 <span data-ttu-id="8d9c3-105">**UserConfigurationDictionaryObjectType**</span><span class="sxs-lookup"><span data-stu-id="8d9c3-105">**UserConfigurationDictionaryObjectType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8d9c3-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8d9c3-106">Attributes and elements</span></span>

<span data-ttu-id="8d9c3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8d9c3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8d9c3-108">属性</span><span class="sxs-lookup"><span data-stu-id="8d9c3-108">Attributes</span></span>

<span data-ttu-id="8d9c3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8d9c3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8d9c3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8d9c3-110">Child elements</span></span>

|<span data-ttu-id="8d9c3-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="8d9c3-111">**Element**</span></span>|<span data-ttu-id="8d9c3-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="8d9c3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d9c3-113">Type (UserConfiguration)</span><span class="sxs-lookup"><span data-stu-id="8d9c3-113">Type (UserConfiguration)</span></span>](type-userconfiguration.md) <br/> | <span data-ttu-id="8d9c3-114">Dictionary オブジェクトの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d9c3-114">Specifies a dictionary object type.</span></span><br/><br/><span data-ttu-id="8d9c3-115">この型には、次のいずれかの文字列値を指定できます。</span><span class="sxs-lookup"><span data-stu-id="8d9c3-115">The type can be one of the following string values:</span></span><br/><br/><span data-ttu-id="8d9c3-116">-DateTime</span><span class="sxs-lookup"><span data-stu-id="8d9c3-116">-  DateTime</span></span>  <br/><span data-ttu-id="8d9c3-117">-Boolean</span><span class="sxs-lookup"><span data-stu-id="8d9c3-117">-  Boolean</span></span>  <br/><span data-ttu-id="8d9c3-118">バイト</span><span class="sxs-lookup"><span data-stu-id="8d9c3-118">-  Byte</span></span>  <br/><span data-ttu-id="8d9c3-119">文字列</span><span class="sxs-lookup"><span data-stu-id="8d9c3-119">-  String</span></span>  <br/><span data-ttu-id="8d9c3-120">- Integer32</span><span class="sxs-lookup"><span data-stu-id="8d9c3-120">-  Integer32</span></span>  <br/><span data-ttu-id="8d9c3-121">- UnsignedInteger32</span><span class="sxs-lookup"><span data-stu-id="8d9c3-121">-  UnsignedInteger32</span></span>  <br/><span data-ttu-id="8d9c3-122">- Integer64</span><span class="sxs-lookup"><span data-stu-id="8d9c3-122">-  Integer64</span></span>  <br/><span data-ttu-id="8d9c3-123">- UnsignedInteger64</span><span class="sxs-lookup"><span data-stu-id="8d9c3-123">-  UnsignedInteger64</span></span>  <br/><span data-ttu-id="8d9c3-124">-StringArray</span><span class="sxs-lookup"><span data-stu-id="8d9c3-124">-  StringArray</span></span>  <br/><span data-ttu-id="8d9c3-125">- ByteArray</span><span class="sxs-lookup"><span data-stu-id="8d9c3-125">-  ByteArray</span></span>  <br/> |
|[<span data-ttu-id="8d9c3-126">Value (UserConfiguration)</span><span class="sxs-lookup"><span data-stu-id="8d9c3-126">Value (UserConfiguration)</span></span>](value-userconfiguration.md) <br/> |<span data-ttu-id="8d9c3-127">Dictionary オブジェクトの値を文字列として指定します。</span><span class="sxs-lookup"><span data-stu-id="8d9c3-127">Specifies the dictionary object value as a string.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8d9c3-128">親要素</span><span class="sxs-lookup"><span data-stu-id="8d9c3-128">Parent elements</span></span>

|<span data-ttu-id="8d9c3-129">**要素**</span><span class="sxs-lookup"><span data-stu-id="8d9c3-129">**Element**</span></span>|<span data-ttu-id="8d9c3-130">**説明**</span><span class="sxs-lookup"><span data-stu-id="8d9c3-130">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8d9c3-131">DictionaryEntry</span><span class="sxs-lookup"><span data-stu-id="8d9c3-131">DictionaryEntry</span></span>](dictionaryentry.md) <br/> |<span data-ttu-id="8d9c3-132">単一の辞書エントリプロパティの内容を指定します。</span><span class="sxs-lookup"><span data-stu-id="8d9c3-132">Specifies the contents of a single dictionary entry property.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8d9c3-133">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8d9c3-133">Text value</span></span>

<span data-ttu-id="8d9c3-134">なし。</span><span class="sxs-lookup"><span data-stu-id="8d9c3-134">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8d9c3-135">注釈</span><span class="sxs-lookup"><span data-stu-id="8d9c3-135">Remarks</span></span>

<span data-ttu-id="8d9c3-136">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8d9c3-136">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8d9c3-137">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8d9c3-137">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8d9c3-138">Namespace</span><span class="sxs-lookup"><span data-stu-id="8d9c3-138">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8d9c3-139">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8d9c3-139">Schema Name</span></span>  <br/> |<span data-ttu-id="8d9c3-140">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8d9c3-140">Types schema</span></span>  <br/> |
|<span data-ttu-id="8d9c3-141">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8d9c3-141">Validation File</span></span>  <br/> |<span data-ttu-id="8d9c3-142">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8d9c3-142">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8d9c3-143">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8d9c3-143">Can be Empty</span></span>  <br/> |<span data-ttu-id="8d9c3-144">正しくない</span><span class="sxs-lookup"><span data-stu-id="8d9c3-144">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8d9c3-145">関連項目</span><span class="sxs-lookup"><span data-stu-id="8d9c3-145">See also</span></span>

- [<span data-ttu-id="8d9c3-146">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8d9c3-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

