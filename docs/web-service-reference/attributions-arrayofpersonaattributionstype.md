---
title: Attributions (ArrayOfPersonaAttributionsType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: f61d843c-bca5-4c88-9667-fd03d2a963a1
description: Attributions 要素は、関連付けられたペルソナに集約された1つ以上の連絡先または Active Directory 受信者の属性情報の配列を指定します。
ms.openlocfilehash: a9883e06a8adbd5c9d3bc7e1edd28c62418df653
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460324"
---
# <a name="attributions-arrayofpersonaattributionstype"></a><span data-ttu-id="86d82-103">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="86d82-103">Attributions (ArrayOfPersonaAttributionsType)</span></span>

<span data-ttu-id="86d82-104">**Attributions**要素は、関連付けられたペルソナに集約された1つ以上の連絡先または Active Directory 受信者の属性情報の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="86d82-104">The **Attributions** element specifies an array of attribution information for one or more of the contacts or Active Directory recipients aggregated into the associated persona.</span></span> 
  
```XML
<Attributions>
    <Attribution></Attribution>
</Attributions>
```

 <span data-ttu-id="86d82-105">**ArrayOfPersonaAttributionsType**</span><span class="sxs-lookup"><span data-stu-id="86d82-105">**ArrayOfPersonaAttributionsType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="86d82-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="86d82-106">Attributes and elements</span></span>

<span data-ttu-id="86d82-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="86d82-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="86d82-108">属性</span><span class="sxs-lookup"><span data-stu-id="86d82-108">Attributes</span></span>

<span data-ttu-id="86d82-109">なし。</span><span class="sxs-lookup"><span data-stu-id="86d82-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="86d82-110">子要素</span><span class="sxs-lookup"><span data-stu-id="86d82-110">Child elements</span></span>

|<span data-ttu-id="86d82-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="86d82-111">**Element**</span></span>|<span data-ttu-id="86d82-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="86d82-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86d82-113">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="86d82-113">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md) <br/> |<span data-ttu-id="86d82-114">**個人の atype**要素の属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="86d82-114">Specifies an instance in an array of attributes for a **PersonaType** element.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="86d82-115">親要素</span><span class="sxs-lookup"><span data-stu-id="86d82-115">Parent elements</span></span>

|<span data-ttu-id="86d82-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="86d82-116">**Element**</span></span>|<span data-ttu-id="86d82-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="86d82-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="86d82-118">ユーザー</span><span class="sxs-lookup"><span data-stu-id="86d82-118">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="86d82-119">**Getpersona**要求によって返される一連のペルソナデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="86d82-119">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="86d82-120">注釈</span><span class="sxs-lookup"><span data-stu-id="86d82-120">Remarks</span></span>

<span data-ttu-id="86d82-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="86d82-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="86d82-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="86d82-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="86d82-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="86d82-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="86d82-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="86d82-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="86d82-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="86d82-125">Schema Name</span></span>  <br/> |<span data-ttu-id="86d82-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="86d82-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="86d82-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="86d82-127">Validation File</span></span>  <br/> |<span data-ttu-id="86d82-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="86d82-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="86d82-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="86d82-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="86d82-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="86d82-130">See also</span></span>

- [<span data-ttu-id="86d82-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="86d82-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

