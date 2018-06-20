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
description: 値の要素には、拡張プロパティの値のコレクションが含まれています。
ms.openlocfilehash: 9c1c07262fa0085487b9a7081c8f72ee55e5ca99
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839988"
---
# <a name="values"></a><span data-ttu-id="7ef71-103">値</span><span class="sxs-lookup"><span data-stu-id="7ef71-103">Values</span></span>

<span data-ttu-id="7ef71-104">**値**の要素には、拡張プロパティの値のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7ef71-104">The **Values** element contains a collection of values for an extended property.</span></span> 
  
```xml
<Values>
   <Value/>
</Values>
```

<span data-ttu-id="7ef71-105">**NonEmptyArrayOfPropertyValuesType**</span><span class="sxs-lookup"><span data-stu-id="7ef71-105">**NonEmptyArrayOfPropertyValuesType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="7ef71-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7ef71-106">Attributes and elements</span></span>

<span data-ttu-id="7ef71-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7ef71-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7ef71-108">属性</span><span class="sxs-lookup"><span data-stu-id="7ef71-108">Attributes</span></span>

<span data-ttu-id="7ef71-109">なし。</span><span class="sxs-lookup"><span data-stu-id="7ef71-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="7ef71-110">子要素</span><span class="sxs-lookup"><span data-stu-id="7ef71-110">Child elements</span></span>

|<span data-ttu-id="7ef71-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="7ef71-111">**Element**</span></span>|<span data-ttu-id="7ef71-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="7ef71-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ef71-113">Value</span><span class="sxs-lookup"><span data-stu-id="7ef71-113">Value</span></span>](value.md) <br/> |<span data-ttu-id="7ef71-114">拡張プロパティの値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7ef71-114">Contains a value of an extended property.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7ef71-115">親要素</span><span class="sxs-lookup"><span data-stu-id="7ef71-115">Parent elements</span></span>

|<span data-ttu-id="7ef71-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="7ef71-116">**Element**</span></span>|<span data-ttu-id="7ef71-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="7ef71-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7ef71-118">ExtendedProperty</span><span class="sxs-lookup"><span data-stu-id="7ef71-118">ExtendedProperty</span></span>](extendedproperty.md) <br/> |<span data-ttu-id="7ef71-119">フォルダーおよびアイテムの拡張プロパティを識別します。</span><span class="sxs-lookup"><span data-stu-id="7ef71-119">Identifies extended properties on folders and items.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7ef71-120">備考</span><span class="sxs-lookup"><span data-stu-id="7ef71-120">Remarks</span></span>

<span data-ttu-id="7ef71-121">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="7ef71-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7ef71-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="7ef71-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7ef71-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="7ef71-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="7ef71-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7ef71-124">Schema name</span></span>  <br/> |<span data-ttu-id="7ef71-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="7ef71-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="7ef71-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7ef71-126">Validation file</span></span>  <br/> |<span data-ttu-id="7ef71-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="7ef71-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="7ef71-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="7ef71-128">Can be empty</span></span>  <br/> |<span data-ttu-id="7ef71-129">False</span><span class="sxs-lookup"><span data-stu-id="7ef71-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7ef71-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="7ef71-130">See also</span></span>

- [<span data-ttu-id="7ef71-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7ef71-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

