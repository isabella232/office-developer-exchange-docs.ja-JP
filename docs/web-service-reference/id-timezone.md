---
title: Id (TimeZone)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Id
api_type:
- schema
ms.assetid: 4c7350b4-ffa1-4e7d-9433-80b4383bd0d2
description: Id 要素は、1つのタイムゾーン定義を識別します。
ms.openlocfilehash: 18ded1c9c0b6f0219d6256ebe19b9b1f7173da2c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466137"
---
# <a name="id-timezone"></a><span data-ttu-id="e1289-103">Id (TimeZone)</span><span class="sxs-lookup"><span data-stu-id="e1289-103">Id (TimeZone)</span></span>

<span data-ttu-id="e1289-104">**Id**要素は、1つのタイムゾーン定義を識別します。</span><span class="sxs-lookup"><span data-stu-id="e1289-104">The **Id** element identifies a single time zone definition.</span></span> 
  
```xml
<Id>...</Id>
```

 <span data-ttu-id="e1289-105">**string**</span><span class="sxs-lookup"><span data-stu-id="e1289-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e1289-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e1289-106">Attributes and elements</span></span>

<span data-ttu-id="e1289-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e1289-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e1289-108">属性</span><span class="sxs-lookup"><span data-stu-id="e1289-108">Attributes</span></span>

<span data-ttu-id="e1289-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e1289-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e1289-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e1289-110">Child elements</span></span>

<span data-ttu-id="e1289-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e1289-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e1289-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e1289-112">Parent elements</span></span>

|<span data-ttu-id="e1289-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e1289-113">**Element**</span></span>|<span data-ttu-id="e1289-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e1289-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e1289-115">Rid</span><span class="sxs-lookup"><span data-stu-id="e1289-115">Ids</span></span>](ids.md) <br/> |<span data-ttu-id="e1289-116">タイムゾーン定義識別子の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="e1289-116">Contains an array of time zone definition identifiers.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e1289-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e1289-117">Text value</span></span>

<span data-ttu-id="e1289-118">テキスト値は必須です。</span><span class="sxs-lookup"><span data-stu-id="e1289-118">A text value is required.</span></span> <span data-ttu-id="e1289-119">テキスト値は、タイムゾーン定義の一意識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="e1289-119">The text value represents the unique identifier for time zone definition.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e1289-120">注釈</span><span class="sxs-lookup"><span data-stu-id="e1289-120">Remarks</span></span>

<span data-ttu-id="e1289-121">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e1289-121">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e1289-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e1289-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e1289-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="e1289-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e1289-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e1289-124">Schema Name</span></span>  <br/> |<span data-ttu-id="e1289-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e1289-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="e1289-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e1289-126">Validation File</span></span>  <br/> |<span data-ttu-id="e1289-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e1289-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e1289-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e1289-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="e1289-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="e1289-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e1289-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="e1289-130">See also</span></span>



- [<span data-ttu-id="e1289-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e1289-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

