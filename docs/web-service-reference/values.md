---
title: 値
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Values
api_type:
- schema
ms.assetid: 4b14c714-51fa-4225-82ad-83ba9f611824
description: Values 要素には、拡張プロパティの値のコレクションが含まれています。
ms.openlocfilehash: 2018f7a734725abe8d8e456492862d1142fda205
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465206"
---
# <a name="values"></a><span data-ttu-id="6a254-103">値</span><span class="sxs-lookup"><span data-stu-id="6a254-103">Values</span></span>

<span data-ttu-id="6a254-104">**Values**要素には、拡張プロパティの値のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6a254-104">The **Values** element contains a collection of values for an extended property.</span></span> 
  
```xml
<Values>
   <Value/>
</Values>
```

<span data-ttu-id="6a254-105">**非 Emptyarrayofpropertyvaluest/プロパティ**</span><span class="sxs-lookup"><span data-stu-id="6a254-105">**NonEmptyArrayOfPropertyValuesType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="6a254-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6a254-106">Attributes and elements</span></span>

<span data-ttu-id="6a254-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6a254-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a254-108">属性</span><span class="sxs-lookup"><span data-stu-id="6a254-108">Attributes</span></span>

<span data-ttu-id="6a254-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6a254-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a254-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6a254-110">Child elements</span></span>

|<span data-ttu-id="6a254-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="6a254-111">**Element**</span></span>|<span data-ttu-id="6a254-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6a254-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a254-113">値</span><span class="sxs-lookup"><span data-stu-id="6a254-113">Value</span></span>](value.md) <br/> |<span data-ttu-id="6a254-114">拡張プロパティの値を格納します。</span><span class="sxs-lookup"><span data-stu-id="6a254-114">Contains a value of an extended property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6a254-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6a254-115">Parent elements</span></span>

|<span data-ttu-id="6a254-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="6a254-116">**Element**</span></span>|<span data-ttu-id="6a254-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="6a254-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a254-118">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="6a254-118">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="6a254-119">フォルダーとアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="6a254-119">Identifies extended properties on folders and items.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="6a254-120">注釈</span><span class="sxs-lookup"><span data-stu-id="6a254-120">Remarks</span></span>

<span data-ttu-id="6a254-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="6a254-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a254-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6a254-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a254-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="6a254-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6a254-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6a254-124">Schema name</span></span>  <br/> |<span data-ttu-id="6a254-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="6a254-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="6a254-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6a254-126">Validation file</span></span>  <br/> |<span data-ttu-id="6a254-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="6a254-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="6a254-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6a254-128">Can be empty</span></span>  <br/> |<span data-ttu-id="6a254-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="6a254-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6a254-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="6a254-130">See also</span></span>

- [<span data-ttu-id="6a254-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="6a254-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

