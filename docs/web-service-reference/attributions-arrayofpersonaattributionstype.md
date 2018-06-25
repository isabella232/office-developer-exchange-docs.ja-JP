---
title: 帰属 (ArrayOfPersonaAttributionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f61d843c-bca5-4c88-9667-fd03d2a963a1
description: 帰属要素は、1 つまたは複数の連絡先や関連するペルソナに集計される Active Directory の受信者の属性情報の配列を指定します。
ms.openlocfilehash: 52fecb4e4381d5e9dbbaf7134fa18068ba15f6ec
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759464"
---
# <a name="attributions-arrayofpersonaattributionstype"></a><span data-ttu-id="58d90-103">帰属 (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="58d90-103">Attributions (ArrayOfPersonaAttributionsType)</span></span>

<span data-ttu-id="58d90-104">**帰属**要素は、1 つまたは複数の連絡先や関連するペルソナに集計される Active Directory の受信者の属性情報の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="58d90-104">The **Attributions** element specifies an array of attribution information for one or more of the contacts or Active Directory recipients aggregated into the associated persona.</span></span> 
  
```XML
<Attributions>
    <Attribution></Attribution>
</Attributions>
```

 <span data-ttu-id="58d90-105">**ArrayOfPersonaAttributionsType**</span><span class="sxs-lookup"><span data-stu-id="58d90-105">**ArrayOfPersonaAttributionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="58d90-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="58d90-106">Attributes and elements</span></span>

<span data-ttu-id="58d90-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="58d90-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="58d90-108">属性</span><span class="sxs-lookup"><span data-stu-id="58d90-108">Attributes</span></span>

<span data-ttu-id="58d90-109">なし。</span><span class="sxs-lookup"><span data-stu-id="58d90-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="58d90-110">子要素</span><span class="sxs-lookup"><span data-stu-id="58d90-110">Child elements</span></span>

|<span data-ttu-id="58d90-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="58d90-111">**Element**</span></span>|<span data-ttu-id="58d90-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="58d90-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58d90-113">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="58d90-113">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="58d90-114">**PersonaType**要素の属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="58d90-114">Specifies an instance in an array of attributes for a **PersonaType** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="58d90-115">親要素</span><span class="sxs-lookup"><span data-stu-id="58d90-115">Parent elements</span></span>

|<span data-ttu-id="58d90-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="58d90-116">**Element**</span></span>|<span data-ttu-id="58d90-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="58d90-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="58d90-118">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="58d90-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="58d90-119">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="58d90-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="58d90-120">備考</span><span class="sxs-lookup"><span data-stu-id="58d90-120">Remarks</span></span>

<span data-ttu-id="58d90-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="58d90-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="58d90-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="58d90-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="58d90-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="58d90-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="58d90-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="58d90-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="58d90-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="58d90-125">Schema Name</span></span>  <br/> |<span data-ttu-id="58d90-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="58d90-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="58d90-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="58d90-127">Validation File</span></span>  <br/> |<span data-ttu-id="58d90-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="58d90-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="58d90-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="58d90-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="58d90-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="58d90-130">See also</span></span>

- [<span data-ttu-id="58d90-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="58d90-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

