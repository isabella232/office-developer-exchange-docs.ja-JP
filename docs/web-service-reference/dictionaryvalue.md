---
title: DictionaryValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DictionaryValue
api_type:
- schema
ms.assetid: f4089381-826f-4f6a-8c6d-e51b910cbe6d
description: DictionaryValue 要素は、dictionary プロパティの辞書値を指定します。
ms.openlocfilehash: 9bad9b8cc7aa80aa071c89a1c22609dc8d44f2b6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462144"
---
# <a name="dictionaryvalue"></a><span data-ttu-id="edc12-103">DictionaryValue</span><span class="sxs-lookup"><span data-stu-id="edc12-103">DictionaryValue</span></span>

<span data-ttu-id="edc12-104">**Dictionaryvalue**要素は、dictionary プロパティの辞書値を指定します。</span><span class="sxs-lookup"><span data-stu-id="edc12-104">The **DictionaryValue** element specifies the dictionary value for a dictionary property.</span></span> 
  
```xml
<DictionaryValue>
   <Type/>
   <Value/>
</DictionaryValue>
```

 <span data-ttu-id="edc12-105">**UserConfigurationDictionaryObjectType**</span><span class="sxs-lookup"><span data-stu-id="edc12-105">**UserConfigurationDictionaryObjectType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="edc12-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="edc12-106">Attributes and elements</span></span>

<span data-ttu-id="edc12-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="edc12-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="edc12-108">属性</span><span class="sxs-lookup"><span data-stu-id="edc12-108">Attributes</span></span>

<span data-ttu-id="edc12-109">なし。</span><span class="sxs-lookup"><span data-stu-id="edc12-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="edc12-110">子要素</span><span class="sxs-lookup"><span data-stu-id="edc12-110">Child elements</span></span>

|<span data-ttu-id="edc12-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="edc12-111">**Element**</span></span>|<span data-ttu-id="edc12-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="edc12-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="edc12-113">Type (UserConfiguration)</span><span class="sxs-lookup"><span data-stu-id="edc12-113">Type (UserConfiguration)</span></span>](type-userconfiguration.md) <br/> |<span data-ttu-id="edc12-114">Dictionary オブジェクトの種類を指定します。</span><span class="sxs-lookup"><span data-stu-id="edc12-114">Specifies the dictionary object type.</span></span>  <br/> |
|[<span data-ttu-id="edc12-115">Value (UserConfiguration)</span><span class="sxs-lookup"><span data-stu-id="edc12-115">Value (UserConfiguration)</span></span>](value-userconfiguration.md) <br/> |<span data-ttu-id="edc12-116">Dictionary オブジェクトの値を文字列として指定します。</span><span class="sxs-lookup"><span data-stu-id="edc12-116">Specifies the dictionary object value as a string.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="edc12-117">親要素</span><span class="sxs-lookup"><span data-stu-id="edc12-117">Parent elements</span></span>

|<span data-ttu-id="edc12-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="edc12-118">**Element**</span></span>|<span data-ttu-id="edc12-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="edc12-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="edc12-120">DictionaryEntry</span><span class="sxs-lookup"><span data-stu-id="edc12-120">DictionaryEntry</span></span>](dictionaryentry.md) <br/> |<span data-ttu-id="edc12-121">単一の辞書エントリプロパティの内容を指定します。</span><span class="sxs-lookup"><span data-stu-id="edc12-121">Specifies the contents of a single dictionary entry property.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="edc12-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="edc12-122">Text value</span></span>

<span data-ttu-id="edc12-123">なし。</span><span class="sxs-lookup"><span data-stu-id="edc12-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="edc12-124">注釈</span><span class="sxs-lookup"><span data-stu-id="edc12-124">Remarks</span></span>

<span data-ttu-id="edc12-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="edc12-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="edc12-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="edc12-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="edc12-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="edc12-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="edc12-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="edc12-128">Schema Name</span></span>  <br/> |<span data-ttu-id="edc12-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="edc12-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="edc12-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="edc12-130">Validation File</span></span>  <br/> |<span data-ttu-id="edc12-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="edc12-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="edc12-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="edc12-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="edc12-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="edc12-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="edc12-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="edc12-134">See also</span></span>

- [<span data-ttu-id="edc12-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="edc12-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

