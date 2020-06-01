---
title: DictionaryEntry
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DictionaryEntry
api_type:
- schema
ms.assetid: 531ea96a-d411-43e6-9fec-11fa2c959a30
description: DictionaryEntry 要素は、単一の dictionary entry プロパティの内容を指定します。
ms.openlocfilehash: 4c5d4c037f0c97b26d518d2f1386f71b31fa2d1f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455661"
---
# <a name="dictionaryentry"></a><span data-ttu-id="ebc55-103">DictionaryEntry</span><span class="sxs-lookup"><span data-stu-id="ebc55-103">DictionaryEntry</span></span>

<span data-ttu-id="ebc55-104">**Dictionaryentry**要素は、単一の dictionary entry プロパティの内容を指定します。</span><span class="sxs-lookup"><span data-stu-id="ebc55-104">The **DictionaryEntry** element specifies the contents of a single dictionary entry property.</span></span> 
  
```xml
<DictionaryEntry>
   <DictionaryKey/>
   <DictionaryValue/>
</DictionaryEntry>
```

 <span data-ttu-id="ebc55-105">**UserConfigurationDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="ebc55-105">**UserConfigurationDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ebc55-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ebc55-106">Attributes and elements</span></span>

<span data-ttu-id="ebc55-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ebc55-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ebc55-108">属性</span><span class="sxs-lookup"><span data-stu-id="ebc55-108">Attributes</span></span>

<span data-ttu-id="ebc55-109">なし。</span><span class="sxs-lookup"><span data-stu-id="ebc55-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="ebc55-110">子要素</span><span class="sxs-lookup"><span data-stu-id="ebc55-110">Child elements</span></span>

|<span data-ttu-id="ebc55-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="ebc55-111">**Element**</span></span>|<span data-ttu-id="ebc55-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="ebc55-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ebc55-113">DictionaryKey</span><span class="sxs-lookup"><span data-stu-id="ebc55-113">DictionaryKey</span></span>](dictionarykey.md) <br/> |<span data-ttu-id="ebc55-114">Dictionary プロパティの辞書キーを指定します。</span><span class="sxs-lookup"><span data-stu-id="ebc55-114">Specifies the dictionary key for a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="ebc55-115">DictionaryValue</span><span class="sxs-lookup"><span data-stu-id="ebc55-115">DictionaryValue</span></span>](dictionaryvalue.md) <br/> |<span data-ttu-id="ebc55-116">Dictionary プロパティの辞書値を指定します。</span><span class="sxs-lookup"><span data-stu-id="ebc55-116">Specifies the dictionary value for a dictionary property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ebc55-117">親要素</span><span class="sxs-lookup"><span data-stu-id="ebc55-117">Parent elements</span></span>

|<span data-ttu-id="ebc55-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="ebc55-118">**Element**</span></span>|<span data-ttu-id="ebc55-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="ebc55-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ebc55-120">辞書</span><span class="sxs-lookup"><span data-stu-id="ebc55-120">Dictionary</span></span>](dictionary.md) <br/> |<span data-ttu-id="ebc55-121">ユーザー構成オブジェクトの辞書のプロパティエントリのセットを定義します。</span><span class="sxs-lookup"><span data-stu-id="ebc55-121">Defines a set of dictionary property entries for a user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="ebc55-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="ebc55-122">Text value</span></span>

<span data-ttu-id="ebc55-123">なし。</span><span class="sxs-lookup"><span data-stu-id="ebc55-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="ebc55-124">注釈</span><span class="sxs-lookup"><span data-stu-id="ebc55-124">Remarks</span></span>

<span data-ttu-id="ebc55-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="ebc55-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ebc55-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ebc55-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ebc55-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="ebc55-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="ebc55-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ebc55-128">Schema Name</span></span>  <br/> |<span data-ttu-id="ebc55-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="ebc55-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="ebc55-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ebc55-130">Validation File</span></span>  <br/> |<span data-ttu-id="ebc55-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="ebc55-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="ebc55-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ebc55-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="ebc55-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="ebc55-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ebc55-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="ebc55-134">See also</span></span>

- [<span data-ttu-id="ebc55-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="ebc55-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

