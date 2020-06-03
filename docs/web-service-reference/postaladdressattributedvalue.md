---
title: PostalAddressAttributedValue
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0f92aa41-1499-4d96-a973-24529ec64d24
description: PostalAddressAttributedValue 要素は、郵便アドレスの配列のインスタンスと、それに関連付けられている attributions を指定します。
ms.openlocfilehash: bf5becca8ee0f143728010c5d0b1ed5a380838ff
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465381"
---
# <a name="postaladdressattributedvalue"></a><span data-ttu-id="a0f2a-103">PostalAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="a0f2a-103">PostalAddressAttributedValue</span></span>

<span data-ttu-id="a0f2a-104">**PostalAddressAttributedValue**要素は、郵便アドレスの配列のインスタンスと、それに関連付けられている attributions を指定します。</span><span class="sxs-lookup"><span data-stu-id="a0f2a-104">The **PostalAddressAttributedValue** element specifies an instance of an array of postal addresses and their associated attributions.</span></span> 
  
```XML
<PostalAddressAttributedValue>
   <Value/>
   <Attributions/>
</PostalAddressAttributedValue>
```

 <span data-ttu-id="a0f2a-105">**PostalAddressAttributedValueType**</span><span class="sxs-lookup"><span data-stu-id="a0f2a-105">**PostalAddressAttributedValueType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a0f2a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a0f2a-106">Attributes and elements</span></span>

<span data-ttu-id="a0f2a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a0f2a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a0f2a-108">属性</span><span class="sxs-lookup"><span data-stu-id="a0f2a-108">Attributes</span></span>

<span data-ttu-id="a0f2a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a0f2a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a0f2a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a0f2a-110">Child elements</span></span>

<span data-ttu-id="a0f2a-111">[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md)  | [Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md)</span><span class="sxs-lookup"><span data-stu-id="a0f2a-111">[Value (PersonaPostalAddressType)](value-personapostaladdresstype.md) | [Attributions (ArrayOfValueAttributionsType)](attributions-arrayofvalueattributionstype.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a0f2a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a0f2a-112">Parent elements</span></span>

<span data-ttu-id="a0f2a-113">[Businessaddresses](businessaddresses.md)  | [ホームアドレス](homeaddresses.md)  | [Otheraddresses](otheraddresses.md)</span><span class="sxs-lookup"><span data-stu-id="a0f2a-113">[BusinessAddresses](businessaddresses.md) | [HomeAddresses](homeaddresses.md) | [OtherAddresses](otheraddresses.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a0f2a-114">注釈</span><span class="sxs-lookup"><span data-stu-id="a0f2a-114">Remarks</span></span>

<span data-ttu-id="a0f2a-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a0f2a-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="a0f2a-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a0f2a-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a0f2a-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a0f2a-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a0f2a-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="a0f2a-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a0f2a-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a0f2a-119">Schema name</span></span>  <br/> |<span data-ttu-id="a0f2a-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a0f2a-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="a0f2a-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a0f2a-121">Validation file</span></span>  <br/> |<span data-ttu-id="a0f2a-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a0f2a-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a0f2a-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="a0f2a-123">Can be empty</span></span>  <br/> ||
   

