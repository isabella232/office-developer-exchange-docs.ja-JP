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
description: 定数要素は、制限で定数値を識別します。
ms.openlocfilehash: 6cb2eaa4227a8fd0985e8ff5a15d647c3bb1cd6a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461556"
---
# <a name="constant"></a><span data-ttu-id="b6cc8-103">定数</span><span class="sxs-lookup"><span data-stu-id="b6cc8-103">Constant</span></span>

<span data-ttu-id="b6cc8-104">**定数**要素は、制限で定数値を識別します。</span><span class="sxs-lookup"><span data-stu-id="b6cc8-104">The **Constant** element identifies a constant value in a restriction.</span></span> 
  
```xml
<Constant Value="" />
```

 <span data-ttu-id="b6cc8-105">**ConstantValueType**</span><span class="sxs-lookup"><span data-stu-id="b6cc8-105">**ConstantValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b6cc8-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b6cc8-106">Attributes and elements</span></span>

<span data-ttu-id="b6cc8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b6cc8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b6cc8-108">属性</span><span class="sxs-lookup"><span data-stu-id="b6cc8-108">Attributes</span></span>

|<span data-ttu-id="b6cc8-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="b6cc8-109">**Attribute**</span></span>|<span data-ttu-id="b6cc8-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="b6cc8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b6cc8-111">**値**</span><span class="sxs-lookup"><span data-stu-id="b6cc8-111">**Value**</span></span> <br/> |<span data-ttu-id="b6cc8-112">制限で比較する値を指定します。</span><span class="sxs-lookup"><span data-stu-id="b6cc8-112">Specifies the value to compare in the restriction.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b6cc8-113">子要素</span><span class="sxs-lookup"><span data-stu-id="b6cc8-113">Child elements</span></span>

<span data-ttu-id="b6cc8-114">なし。</span><span class="sxs-lookup"><span data-stu-id="b6cc8-114">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b6cc8-115">親要素</span><span class="sxs-lookup"><span data-stu-id="b6cc8-115">Parent elements</span></span>

|<span data-ttu-id="b6cc8-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="b6cc8-116">**Element**</span></span>|<span data-ttu-id="b6cc8-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="b6cc8-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b6cc8-118">内容</span><span class="sxs-lookup"><span data-stu-id="b6cc8-118">Contains</span></span>](contains.md) <br/> |<span data-ttu-id="b6cc8-119">指定したプロパティに指定した定数文字列値が含まれているかどうかを決定する検索式を表します。</span><span class="sxs-lookup"><span data-stu-id="b6cc8-119">Represents a search expression that determines whether a given property contains the supplied constant string value.</span></span>  <br/> |
|[<span data-ttu-id="b6cc8-120">FieldURIOrConstant</span><span class="sxs-lookup"><span data-stu-id="b6cc8-120">FieldURIOrConstant</span></span>](fielduriorconstant.md) <br/> |<span data-ttu-id="b6cc8-121">別のプロパティと比較するときに使用するプロパティまたは定数の値を表します。</span><span class="sxs-lookup"><span data-stu-id="b6cc8-121">Represents either a property or a constant value to be used when comparing with another property.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b6cc8-122">注釈</span><span class="sxs-lookup"><span data-stu-id="b6cc8-122">Remarks</span></span>

<span data-ttu-id="b6cc8-123">**Value**属性の文字列値は、比較しようとしている型に対して強制変換可能である必要があります。</span><span class="sxs-lookup"><span data-stu-id="b6cc8-123">The string value in the **Value** attribute must be coercible into the type you are trying to compare against.</span></span> <span data-ttu-id="b6cc8-124">たとえば、日付/時刻プロパティを定数値と比較する場合、文字列値は日付/時刻を表す必要があります。</span><span class="sxs-lookup"><span data-stu-id="b6cc8-124">For example, if you are comparing a date/time property against a constant value, the string value must represent a date/time.</span></span> 
  
<span data-ttu-id="b6cc8-125">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b6cc8-125">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b6cc8-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b6cc8-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b6cc8-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="b6cc8-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b6cc8-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b6cc8-128">Schema Name</span></span>  <br/> |<span data-ttu-id="b6cc8-129">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="b6cc8-129">Types schema</span></span>  <br/> |
|<span data-ttu-id="b6cc8-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b6cc8-130">Validation File</span></span>  <br/> |<span data-ttu-id="b6cc8-131">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="b6cc8-131">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="b6cc8-132">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b6cc8-132">Can be Empty</span></span>  <br/> |<span data-ttu-id="b6cc8-133">正しくない</span><span class="sxs-lookup"><span data-stu-id="b6cc8-133">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b6cc8-134">関連項目</span><span class="sxs-lookup"><span data-stu-id="b6cc8-134">See also</span></span>



- [<span data-ttu-id="b6cc8-135">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="b6cc8-135">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

