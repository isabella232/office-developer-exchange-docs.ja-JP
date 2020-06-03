---
title: Dictionary
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Dictionary
api_type:
- schema
ms.assetid: 8309e468-115b-4d6e-b33c-c4719dcecc4c
description: Dictionary 要素は、ユーザー構成オブジェクトの辞書のプロパティエントリのセットを定義します。
ms.openlocfilehash: 8e5267717aab2317b2bc1581a775ead81025a08a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455668"
---
# <a name="dictionary"></a><span data-ttu-id="7c8a3-103">Dictionary</span><span class="sxs-lookup"><span data-stu-id="7c8a3-103">Dictionary</span></span>

<span data-ttu-id="7c8a3-104">**Dictionary**要素は、ユーザー構成オブジェクトの辞書のプロパティエントリのセットを定義します。</span><span class="sxs-lookup"><span data-stu-id="7c8a3-104">The **Dictionary** element defines a set of dictionary property entries for a user configuration object.</span></span> 
  
```xml
<Dictionary>
   <DictionaryEntry/>
</Dictionary>
```

 <span data-ttu-id="7c8a3-105">**UserConfigurationDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="7c8a3-105">**UserConfigurationDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7c8a3-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7c8a3-106">Attributes and elements</span></span>

<span data-ttu-id="7c8a3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7c8a3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7c8a3-108">属性</span><span class="sxs-lookup"><span data-stu-id="7c8a3-108">Attributes</span></span>

<span data-ttu-id="7c8a3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7c8a3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7c8a3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7c8a3-110">Child elements</span></span>

|<span data-ttu-id="7c8a3-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="7c8a3-111">**Element**</span></span>|<span data-ttu-id="7c8a3-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7c8a3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c8a3-113">DictionaryEntry</span><span class="sxs-lookup"><span data-stu-id="7c8a3-113">DictionaryEntry</span></span>](dictionaryentry.md) <br/> |<span data-ttu-id="7c8a3-114">単一の辞書エントリプロパティの内容を指定します。</span><span class="sxs-lookup"><span data-stu-id="7c8a3-114">Specifies the contents of a single dictionary entry property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7c8a3-115">親要素</span><span class="sxs-lookup"><span data-stu-id="7c8a3-115">Parent elements</span></span>

|<span data-ttu-id="7c8a3-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="7c8a3-116">**Element**</span></span>|<span data-ttu-id="7c8a3-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="7c8a3-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7c8a3-118">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="7c8a3-118">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="7c8a3-119">1つのユーザー構成オブジェクトを定義します。</span><span class="sxs-lookup"><span data-stu-id="7c8a3-119">Defines a single user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="7c8a3-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="7c8a3-120">Text value</span></span>

<span data-ttu-id="7c8a3-121">なし。</span><span class="sxs-lookup"><span data-stu-id="7c8a3-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="7c8a3-122">注釈</span><span class="sxs-lookup"><span data-stu-id="7c8a3-122">Remarks</span></span>

<span data-ttu-id="7c8a3-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="7c8a3-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7c8a3-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7c8a3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7c8a3-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="7c8a3-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7c8a3-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7c8a3-126">Schema Name</span></span>  <br/> |<span data-ttu-id="7c8a3-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="7c8a3-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="7c8a3-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7c8a3-128">Validation File</span></span>  <br/> |<span data-ttu-id="7c8a3-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="7c8a3-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7c8a3-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7c8a3-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="7c8a3-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="7c8a3-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7c8a3-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="7c8a3-132">See also</span></span>

- [<span data-ttu-id="7c8a3-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7c8a3-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

