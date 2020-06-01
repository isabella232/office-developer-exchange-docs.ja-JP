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
description: FileAs 要素は、連絡先フォルダーで連絡先または配布リストがどのようにファイリングされるかを表します。
ms.openlocfilehash: be756d86d7608fcb758dd54f2ada9f03a04343e2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461199"
---
# <a name="fileas"></a><span data-ttu-id="f0200-103">FileAs</span><span class="sxs-lookup"><span data-stu-id="f0200-103">FileAs</span></span>

<span data-ttu-id="f0200-104">**FileAs**要素は、連絡先フォルダーで連絡先または配布リストがどのようにファイリングされるかを表します。</span><span class="sxs-lookup"><span data-stu-id="f0200-104">The **FileAs** element represents how a contact or distribution list is filed in the Contacts folder.</span></span> 
  
```xml
<FileAs/>
```

 <span data-ttu-id="f0200-105">**string**</span><span class="sxs-lookup"><span data-stu-id="f0200-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f0200-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f0200-106">Attributes and elements</span></span>

<span data-ttu-id="f0200-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f0200-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f0200-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0200-108">Attributes</span></span>

<span data-ttu-id="f0200-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f0200-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f0200-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f0200-110">Child elements</span></span>

<span data-ttu-id="f0200-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f0200-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f0200-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f0200-112">Parent elements</span></span>

|<span data-ttu-id="f0200-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f0200-113">**Element**</span></span>|<span data-ttu-id="f0200-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f0200-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f0200-115">DistributionList</span><span class="sxs-lookup"><span data-stu-id="f0200-115">DistributionList</span></span>](distributionlist.md) <br/> |<span data-ttu-id="f0200-116">配布リストを表します。</span><span class="sxs-lookup"><span data-stu-id="f0200-116">Represents a distribution list.</span></span>  <br/> |
|[<span data-ttu-id="f0200-117">連絡先</span><span class="sxs-lookup"><span data-stu-id="f0200-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="f0200-118">Exchange の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="f0200-118">Represents an Exchange contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f0200-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f0200-119">Text value</span></span>

<span data-ttu-id="f0200-120">この要素を使用する場合は、文字列を表すテキスト値が必要です。</span><span class="sxs-lookup"><span data-stu-id="f0200-120">A text value that represents a string is required if this element is used.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f0200-121">注釈</span><span class="sxs-lookup"><span data-stu-id="f0200-121">Remarks</span></span>

<span data-ttu-id="f0200-122">**FileAs**要素は、連絡先および配布リストを、氏名または会社名以外の名前で並べ替えるために使用されます。</span><span class="sxs-lookup"><span data-stu-id="f0200-122">The **FileAs** element is used to sort contacts and distribution lists by a name other than a full name or company name.</span></span> 
  
<span data-ttu-id="f0200-123">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="f0200-123">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f0200-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f0200-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f0200-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="f0200-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f0200-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f0200-126">Schema name</span></span>  <br/> |<span data-ttu-id="f0200-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="f0200-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="f0200-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f0200-128">Validation file</span></span>  <br/> |<span data-ttu-id="f0200-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f0200-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="f0200-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f0200-130">Can be empty</span></span>  <br/> |<span data-ttu-id="f0200-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="f0200-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f0200-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="f0200-132">See also</span></span>



- [<span data-ttu-id="f0200-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f0200-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

