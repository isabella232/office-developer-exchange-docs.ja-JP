---
title: PostalAddressAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0f92aa41-1499-4d96-a973-24529ec64d24
description: PostalAddressAttributedValue 要素は、アドレスの郵便番号の配列と、関連付けられている帰属のインスタンスを指定します。
ms.openlocfilehash: f2b8b9818e39780b934522910d016875dbe5af2e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832854"
---
# <a name="postaladdressattributedvalue"></a><span data-ttu-id="8bba8-103">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="8bba8-103">PostalAddressAttributedValue</span></span>

<span data-ttu-id="8bba8-104">**PostalAddressAttributedValue**要素は、アドレスの郵便番号の配列と、関連付けられている帰属のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="8bba8-104">The **PostalAddressAttributedValue** element specifies an instance of an array of postal addresses and their associated attributions.</span></span> 
  
```XML
<PostalAddressAttributedValue>
   <Value/>
   <Attributions/>
</PostalAddressAttributedValue>
```

 <span data-ttu-id="8bba8-105">**PostalAddressAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="8bba8-105">**PostalAddressAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8bba8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8bba8-106">Attributes and elements</span></span>

<span data-ttu-id="8bba8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8bba8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8bba8-108">属性</span><span class="sxs-lookup"><span data-stu-id="8bba8-108">Attributes</span></span>

<span data-ttu-id="8bba8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8bba8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8bba8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8bba8-110">Child elements</span></span>

<span data-ttu-id="8bba8-111">[値 (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [(ArrayOfValueAttributionsType) の帰属](attributions-arrayofvalueattributionstype.md)</span><span class="sxs-lookup"><span data-stu-id="8bba8-111">[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8bba8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8bba8-112">Parent elements</span></span>

<span data-ttu-id="8bba8-113">[BusinessAddresses](businessaddresses.md) | [HomeAddresses](homeaddresses.md) | [OtherAddresses](otheraddresses.md)</span><span class="sxs-lookup"><span data-stu-id="8bba8-113">[BusinessAddresses](businessaddresses.md) | [HomeAddresses](homeaddresses.md) | [OtherAddresses](otheraddresses.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8bba8-114">備考</span><span class="sxs-lookup"><span data-stu-id="8bba8-114">Remarks</span></span>

<span data-ttu-id="8bba8-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="8bba8-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="8bba8-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8bba8-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8bba8-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="8bba8-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8bba8-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="8bba8-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8bba8-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8bba8-119">Schema name</span></span>  <br/> |<span data-ttu-id="8bba8-120">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="8bba8-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="8bba8-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8bba8-121">Validation file</span></span>  <br/> |<span data-ttu-id="8bba8-122">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="8bba8-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8bba8-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8bba8-123">Can be empty</span></span>  <br/> ||
   

