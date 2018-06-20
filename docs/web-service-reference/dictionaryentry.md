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
description: DictionaryEntry 要素は、1 つのディクショナリ エントリのプロパティの内容を指定します。
ms.openlocfilehash: 75d7dd1aa82a4cc6c363b9c787cfb15b4d15b656
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760037"
---
# <a name="dictionaryentry"></a><span data-ttu-id="2013d-103">DictionaryEntry</span><span class="sxs-lookup"><span data-stu-id="2013d-103">DictionaryEntry</span></span>

<span data-ttu-id="2013d-104">**DictionaryEntry**要素は、1 つのディクショナリ エントリのプロパティの内容を指定します。</span><span class="sxs-lookup"><span data-stu-id="2013d-104">The **DictionaryEntry** element specifies the contents of a single dictionary entry property.</span></span> 
  
```xml
<DictionaryEntry>
   <DictionaryKey/>
   <DictionaryValue/>
</DictionaryEntry>
```

 <span data-ttu-id="2013d-105">**UserConfigurationDictionaryEntryType**</span><span class="sxs-lookup"><span data-stu-id="2013d-105">**UserConfigurationDictionaryEntryType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2013d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2013d-106">Attributes and elements</span></span>

<span data-ttu-id="2013d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2013d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2013d-108">属性</span><span class="sxs-lookup"><span data-stu-id="2013d-108">Attributes</span></span>

<span data-ttu-id="2013d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2013d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2013d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2013d-110">Child elements</span></span>

|<span data-ttu-id="2013d-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="2013d-111">**Element**</span></span>|<span data-ttu-id="2013d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2013d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2013d-113">DictionaryKey</span><span class="sxs-lookup"><span data-stu-id="2013d-113">DictionaryKey</span></span>](dictionarykey.md) <br/> |<span data-ttu-id="2013d-114">ディクショナリ プロパティのディクショナリのキーを指定します。</span><span class="sxs-lookup"><span data-stu-id="2013d-114">Specifies the dictionary key for a dictionary property.</span></span>  <br/> |
|[<span data-ttu-id="2013d-115">DictionaryValue</span><span class="sxs-lookup"><span data-stu-id="2013d-115">DictionaryValue</span></span>](dictionaryvalue.md) <br/> |<span data-ttu-id="2013d-116">ディクショナリ プロパティのディクショナリの値を指定します。</span><span class="sxs-lookup"><span data-stu-id="2013d-116">Specifies the dictionary value for a dictionary property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2013d-117">親要素</span><span class="sxs-lookup"><span data-stu-id="2013d-117">Parent elements</span></span>

|<span data-ttu-id="2013d-118">**要素**</span><span class="sxs-lookup"><span data-stu-id="2013d-118">**Element**</span></span>|<span data-ttu-id="2013d-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="2013d-119">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2013d-120">辞書</span><span class="sxs-lookup"><span data-stu-id="2013d-120">Dictionary</span></span>](dictionary.md) <br/> |<span data-ttu-id="2013d-121">ユーザーの構成オブジェクトのディクショナリ プロパティのエントリのセットを定義します。</span><span class="sxs-lookup"><span data-stu-id="2013d-121">Defines a set of dictionary property entries for a user configuration object.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="2013d-122">テキスト値</span><span class="sxs-lookup"><span data-stu-id="2013d-122">Text value</span></span>

<span data-ttu-id="2013d-123">なし。</span><span class="sxs-lookup"><span data-stu-id="2013d-123">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="2013d-124">備考</span><span class="sxs-lookup"><span data-stu-id="2013d-124">Remarks</span></span>

<span data-ttu-id="2013d-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="2013d-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2013d-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="2013d-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2013d-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="2013d-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="2013d-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2013d-128">Schema Name</span></span>  <br/> |<span data-ttu-id="2013d-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="2013d-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="2013d-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2013d-130">Validation File</span></span>  <br/> |<span data-ttu-id="2013d-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="2013d-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="2013d-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2013d-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="2013d-133">False</span><span class="sxs-lookup"><span data-stu-id="2013d-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2013d-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="2013d-134">See also</span></span>

- [<span data-ttu-id="2013d-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2013d-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

