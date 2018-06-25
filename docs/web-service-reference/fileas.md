---
title: FileAs
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FileAs
api_type:
- schema
ms.assetid: df50524e-471c-49d2-89fe-b2d0f61a1365
description: 表題の要素は、連絡先フォルダーに連絡先または配布リストを提出する方法を表します。
ms.openlocfilehash: dab9142eebf7691862e7970a7d1e8f5874393b94
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760481"
---
# <a name="fileas"></a><span data-ttu-id="a2018-103">FileAs</span><span class="sxs-lookup"><span data-stu-id="a2018-103">FileAs</span></span>

<span data-ttu-id="a2018-104">**表題**の要素は、連絡先フォルダーに連絡先または配布リストを提出する方法を表します。</span><span class="sxs-lookup"><span data-stu-id="a2018-104">The **FileAs** element represents how a contact or distribution list is filed in the Contacts folder.</span></span> 
  
```xml
<FileAs/>
```

 <span data-ttu-id="a2018-105">**string**</span><span class="sxs-lookup"><span data-stu-id="a2018-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a2018-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a2018-106">Attributes and elements</span></span>

<span data-ttu-id="a2018-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a2018-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a2018-108">属性</span><span class="sxs-lookup"><span data-stu-id="a2018-108">Attributes</span></span>

<span data-ttu-id="a2018-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a2018-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a2018-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a2018-110">Child elements</span></span>

<span data-ttu-id="a2018-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a2018-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a2018-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a2018-112">Parent elements</span></span>

|<span data-ttu-id="a2018-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a2018-113">**Element**</span></span>|<span data-ttu-id="a2018-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a2018-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a2018-115">DistributionList</span><span class="sxs-lookup"><span data-stu-id="a2018-115">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="a2018-116">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="a2018-116">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="a2018-117">Contact</span><span class="sxs-lookup"><span data-stu-id="a2018-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="a2018-118">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="a2018-118">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a2018-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a2018-119">Text value</span></span>

<span data-ttu-id="a2018-120">文字列を表す文字列値は、この要素を使用する場合に必要です。</span><span class="sxs-lookup"><span data-stu-id="a2018-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a2018-121">備考</span><span class="sxs-lookup"><span data-stu-id="a2018-121">Remarks</span></span>

<span data-ttu-id="a2018-122">**表題**要素が完全な名前または会社名以外の名前で連絡先および配布リストを並べ替えるには使用します。</span><span class="sxs-lookup"><span data-stu-id="a2018-122">The **FileAs** element is used to sort contacts and distribution lists by a name other than a full name or company name.</span></span> 
  
<span data-ttu-id="a2018-123">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="a2018-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a2018-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="a2018-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a2018-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="a2018-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a2018-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a2018-126">Schema name</span></span>  <br/> |<span data-ttu-id="a2018-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="a2018-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="a2018-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a2018-128">Validation file</span></span>  <br/> |<span data-ttu-id="a2018-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="a2018-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a2018-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a2018-130">Can be empty</span></span>  <br/> |<span data-ttu-id="a2018-131">False</span><span class="sxs-lookup"><span data-stu-id="a2018-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a2018-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="a2018-132">See also</span></span>



- [<span data-ttu-id="a2018-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a2018-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

