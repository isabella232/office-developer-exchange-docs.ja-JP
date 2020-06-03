---
title: CountryOrRegion
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CountryOrRegion
api_type:
- schema
ms.assetid: e978cd19-96ce-4ebf-81df-eadf2d775132
description: Country 要素は、指定された物理的な住所の国または地域を表します。
ms.openlocfilehash: 2e5b8ec40676123c17d6c7f987f139246dbd0493
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44527097"
---
# <a name="countryorregion"></a><span data-ttu-id="08150-103">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="08150-103">CountryOrRegion</span></span>

<span data-ttu-id="08150-104">**Country**要素は、指定された物理的な住所の国または地域を表します。</span><span class="sxs-lookup"><span data-stu-id="08150-104">The **Country** element represents the country or region for a given physical address.</span></span> 
  
```xml
<Country/>
```

 <span data-ttu-id="08150-105">**String**</span><span class="sxs-lookup"><span data-stu-id="08150-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="08150-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="08150-106">Attributes and elements</span></span>

<span data-ttu-id="08150-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="08150-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="08150-108">属性</span><span class="sxs-lookup"><span data-stu-id="08150-108">Attributes</span></span>

<span data-ttu-id="08150-109">なし。</span><span class="sxs-lookup"><span data-stu-id="08150-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="08150-110">子要素</span><span class="sxs-lookup"><span data-stu-id="08150-110">Child elements</span></span>

<span data-ttu-id="08150-111">なし。</span><span class="sxs-lookup"><span data-stu-id="08150-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="08150-112">親要素</span><span class="sxs-lookup"><span data-stu-id="08150-112">Parent elements</span></span>

|<span data-ttu-id="08150-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="08150-113">**Element**</span></span>|<span data-ttu-id="08150-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="08150-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="08150-115">Entry (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="08150-115">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md) <br/> |<span data-ttu-id="08150-116">連絡先アイテムの単一の物理アドレスを記述します。</span><span class="sxs-lookup"><span data-stu-id="08150-116">Describes a single physical address for a contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="08150-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="08150-117">Text value</span></span>

<span data-ttu-id="08150-118">テキスト値は、国の名前を表す文字列型 (string) の値です。</span><span class="sxs-lookup"><span data-stu-id="08150-118">The text value is a string value that represents the name of a country.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="08150-119">注釈</span><span class="sxs-lookup"><span data-stu-id="08150-119">Remarks</span></span>

<span data-ttu-id="08150-120">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="08150-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="08150-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="08150-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="08150-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="08150-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="08150-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="08150-123">Schema name</span></span>  <br/> |<span data-ttu-id="08150-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="08150-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="08150-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="08150-125">Validation file</span></span>  <br/> |<span data-ttu-id="08150-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="08150-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="08150-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="08150-127">Can be empty</span></span>  <br/> |<span data-ttu-id="08150-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="08150-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="08150-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="08150-129">See also</span></span>



- [<span data-ttu-id="08150-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="08150-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

