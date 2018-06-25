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
description: 国の要素では、国または地域の特定の物理アドレスを表します。
ms.openlocfilehash: 84a8cc4c76af616f116f35b733a645a6a0e4640c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759793"
---
# <a name="countryorregion"></a><span data-ttu-id="fa718-103">CountryOrRegion</span><span class="sxs-lookup"><span data-stu-id="fa718-103">CountryOrRegion</span></span>

<span data-ttu-id="fa718-104">**国**の要素では、国または地域の特定の物理アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="fa718-104">The **Country** element represents the country or region for a given physical address.</span></span> 
  
```xml
<Country/>
```

 <span data-ttu-id="fa718-105">**文字列型 (String)**</span><span class="sxs-lookup"><span data-stu-id="fa718-105">**String**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa718-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fa718-106">Attributes and elements</span></span>

<span data-ttu-id="fa718-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fa718-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa718-108">属性</span><span class="sxs-lookup"><span data-stu-id="fa718-108">Attributes</span></span>

<span data-ttu-id="fa718-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fa718-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fa718-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fa718-110">Child elements</span></span>

<span data-ttu-id="fa718-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fa718-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fa718-112">親要素</span><span class="sxs-lookup"><span data-stu-id="fa718-112">Parent elements</span></span>

|<span data-ttu-id="fa718-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="fa718-113">**Element**</span></span>|<span data-ttu-id="fa718-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="fa718-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa718-115">エントリ (PhysicalAddress)</span><span class="sxs-lookup"><span data-stu-id="fa718-115">Entry (PhysicalAddress)</span></span>](entry-physicaladdress.md) <br/> |<span data-ttu-id="fa718-116">連絡先アイテムの 1 つの物理アドレスをについて説明します。</span><span class="sxs-lookup"><span data-stu-id="fa718-116">Describes a single physical address for a contact item.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="fa718-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fa718-117">Text value</span></span>

<span data-ttu-id="fa718-118">テキスト値は、国の名前を表す文字列値です。</span><span class="sxs-lookup"><span data-stu-id="fa718-118">The text value is a string value that represents the name of a country.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="fa718-119">備考</span><span class="sxs-lookup"><span data-stu-id="fa718-119">Remarks</span></span>

<span data-ttu-id="fa718-120">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="fa718-120">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fa718-121">要素情報</span><span class="sxs-lookup"><span data-stu-id="fa718-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa718-122">名前空間</span><span class="sxs-lookup"><span data-stu-id="fa718-122">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fa718-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fa718-123">Schema name</span></span>  <br/> |<span data-ttu-id="fa718-124">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="fa718-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="fa718-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fa718-125">Validation file</span></span>  <br/> |<span data-ttu-id="fa718-126">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="fa718-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fa718-127">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fa718-127">Can be empty</span></span>  <br/> |<span data-ttu-id="fa718-128">False</span><span class="sxs-lookup"><span data-stu-id="fa718-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="fa718-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="fa718-129">See also</span></span>



- [<span data-ttu-id="fa718-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="fa718-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

