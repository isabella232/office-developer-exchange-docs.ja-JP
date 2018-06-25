---
title: 定数
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Constant
api_type:
- schema
ms.assetid: 340af0cd-9f12-44ab-b8f1-21d107c8d0c9
description: 定数の要素は、制限の中で定数値を識別します。
ms.openlocfilehash: 73912bc1981c5d54040f7c4a563ad805916fe721
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759663"
---
# <a name="constant"></a><span data-ttu-id="5e778-103">定数</span><span class="sxs-lookup"><span data-stu-id="5e778-103">Constant</span></span>

<span data-ttu-id="5e778-104">**定数**の要素は、制限の中で定数値を識別します。</span><span class="sxs-lookup"><span data-stu-id="5e778-104">The **Constant** element identifies a constant value in a restriction.</span></span> 
  
```xml
<Constant Value="" />
```

 <span data-ttu-id="5e778-105">**ConstantValueType**</span><span class="sxs-lookup"><span data-stu-id="5e778-105">**ConstantValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5e778-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5e778-106">Attributes and elements</span></span>

<span data-ttu-id="5e778-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5e778-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5e778-108">属性</span><span class="sxs-lookup"><span data-stu-id="5e778-108">Attributes</span></span>

|<span data-ttu-id="5e778-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="5e778-109">**Attribute**</span></span>|<span data-ttu-id="5e778-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="5e778-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5e778-111">**Value**</span><span class="sxs-lookup"><span data-stu-id="5e778-111">**Value**</span></span> <br/> |<span data-ttu-id="5e778-112">制限における比較値を指定します。</span><span class="sxs-lookup"><span data-stu-id="5e778-112">Specifies the value to compare in the restriction.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5e778-113">子要素</span><span class="sxs-lookup"><span data-stu-id="5e778-113">Child elements</span></span>

<span data-ttu-id="5e778-114">なし。</span><span class="sxs-lookup"><span data-stu-id="5e778-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="5e778-115">親要素</span><span class="sxs-lookup"><span data-stu-id="5e778-115">Parent elements</span></span>

|<span data-ttu-id="5e778-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="5e778-116">**Element**</span></span>|<span data-ttu-id="5e778-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="5e778-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5e778-118">内容</span><span class="sxs-lookup"><span data-stu-id="5e778-118">Contains</span></span>](contains.md) <br/> |<span data-ttu-id="5e778-119">指定したプロパティに指定された文字列定数の値が含まれているかどうかを判断する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="5e778-119">Represents a search expression that determines whether a given property contains the supplied constant string value.</span></span>  <br/> |
|[<span data-ttu-id="5e778-120">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="5e778-120">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="5e778-121">プロパティまたは別のプロパティを比較するときに使用する定数値のいずれかを表します。</span><span class="sxs-lookup"><span data-stu-id="5e778-121">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5e778-122">備考</span><span class="sxs-lookup"><span data-stu-id="5e778-122">Remarks</span></span>

<span data-ttu-id="5e778-123">**Value**属性の文字列値と比較しようとしている型に強制変換できる必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e778-123">The string value in the **Value** attribute must be coercible into the type you are trying to compare against.</span></span> <span data-ttu-id="5e778-124">たとえば、日付/時刻プロパティを定数値を比較する場合は、文字列値は日付/時刻を表す必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e778-124">For example, if you are comparing a date/time property against a constant value, the string value must represent a date/time.</span></span> 
  
<span data-ttu-id="5e778-125">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="5e778-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5e778-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="5e778-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5e778-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="5e778-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="5e778-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5e778-128">Schema Name</span></span>  <br/> |<span data-ttu-id="5e778-129">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="5e778-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="5e778-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5e778-130">Validation File</span></span>  <br/> |<span data-ttu-id="5e778-131">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="5e778-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="5e778-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5e778-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="5e778-133">False</span><span class="sxs-lookup"><span data-stu-id="5e778-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5e778-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="5e778-134">See also</span></span>



- [<span data-ttu-id="5e778-135">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="5e778-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

