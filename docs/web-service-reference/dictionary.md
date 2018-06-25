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
description: ユーザーの構成オブジェクトのプロパティのエントリをディクショナリのディクショナリの要素を定義します。
ms.openlocfilehash: 151abfe7a9a9ae05b8b61af87c33675e025920ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760035"
---
# <a name="dictionary"></a><span data-ttu-id="9d819-103">Dictionary</span><span class="sxs-lookup"><span data-stu-id="9d819-103">Dictionary</span></span>

<span data-ttu-id="9d819-104">ユーザーの構成オブジェクトのプロパティのエントリをディクショナリの**ディクショナリ**の要素を定義します。</span><span class="sxs-lookup"><span data-stu-id="9d819-104">The **Dictionary** element defines a set of dictionary property entries for a user configuration object.</span></span> 
  
```xml
<Dictionary>
   <DictionaryEntry/>
</Dictionary>
```

 <span data-ttu-id="9d819-105">**UserConfigurationDictionaryType**</span><span class="sxs-lookup"><span data-stu-id="9d819-105">**UserConfigurationDictionaryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d819-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9d819-106">Attributes and elements</span></span>

<span data-ttu-id="9d819-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9d819-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d819-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d819-108">Attributes</span></span>

<span data-ttu-id="9d819-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9d819-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d819-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9d819-110">Child elements</span></span>

|<span data-ttu-id="9d819-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="9d819-111">**Element**</span></span>|<span data-ttu-id="9d819-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="9d819-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d819-113">DictionaryEntry</span><span class="sxs-lookup"><span data-stu-id="9d819-113">DictionaryEntry</span></span>](dictionaryentry.md) <br/> |<span data-ttu-id="9d819-114">1 つのディクショナリ エントリのプロパティの内容を指定します。</span><span class="sxs-lookup"><span data-stu-id="9d819-114">Specifies the contents of a single dictionary entry property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9d819-115">親要素</span><span class="sxs-lookup"><span data-stu-id="9d819-115">Parent elements</span></span>

|<span data-ttu-id="9d819-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="9d819-116">**Element**</span></span>|<span data-ttu-id="9d819-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="9d819-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9d819-118">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="9d819-118">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="9d819-119">1 人のユーザーの構成オブジェクトを定義します。</span><span class="sxs-lookup"><span data-stu-id="9d819-119">Defines a single user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9d819-120">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9d819-120">Text value</span></span>

<span data-ttu-id="9d819-121">なし。</span><span class="sxs-lookup"><span data-stu-id="9d819-121">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9d819-122">備考</span><span class="sxs-lookup"><span data-stu-id="9d819-122">Remarks</span></span>

<span data-ttu-id="9d819-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9d819-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d819-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="9d819-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d819-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="9d819-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9d819-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9d819-126">Schema Name</span></span>  <br/> |<span data-ttu-id="9d819-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9d819-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="9d819-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9d819-128">Validation File</span></span>  <br/> |<span data-ttu-id="9d819-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9d819-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9d819-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9d819-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="9d819-131">False</span><span class="sxs-lookup"><span data-stu-id="9d819-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9d819-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="9d819-132">See also</span></span>

- [<span data-ttu-id="9d819-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9d819-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

