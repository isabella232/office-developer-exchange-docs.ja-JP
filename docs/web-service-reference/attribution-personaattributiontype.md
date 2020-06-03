---
title: 属性 (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: 属性要素は、個人の Atype 要素の属性の配列のインスタンスを指定します。
ms.openlocfilehash: 05b0d41c116f2ed7b8dbb3ac44108bb879256b5c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464176"
---
# <a name="attribution-personaattributiontype"></a><span data-ttu-id="e83be-103">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="e83be-103">Attribution (PersonaAttributionType)</span></span>

<span data-ttu-id="e83be-104">属性**要素は、** **個人の atype**要素の属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="e83be-104">The **Attribution** element specifies an instance in an array of attributes for a **PersonaType** element.</span></span> 
  
```XML
<Attribution>
    <Id></Id>
    <SourceId></SourceId>
    <DisplayName></DisplayName>
    <IsWritable></IsWritable>
    <IsQuickContact></IsQuickContact>
    <IsHidden></IsHidden>
    <FolderId></FolderId>
</Attribution>
```

 <span data-ttu-id="e83be-105">**PersonaAttributionType**</span><span class="sxs-lookup"><span data-stu-id="e83be-105">**PersonaAttributionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e83be-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e83be-106">Attributes and elements</span></span>

<span data-ttu-id="e83be-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e83be-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e83be-108">属性</span><span class="sxs-lookup"><span data-stu-id="e83be-108">Attributes</span></span>

<span data-ttu-id="e83be-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e83be-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e83be-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e83be-110">Child elements</span></span>

|<span data-ttu-id="e83be-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="e83be-111">**Element**</span></span>|<span data-ttu-id="e83be-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="e83be-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e83be-113">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="e83be-113">ID (String)</span></span>](id-string.md) <br/> |<span data-ttu-id="e83be-114">アプリを一意に識別する文字列を指定します。または、ペルソナの属性を指定します。</span><span class="sxs-lookup"><span data-stu-id="e83be-114">Specifies a string that uniquely identifies an app or an attribution in a persona.</span></span>  <br/> |
|[<span data-ttu-id="e83be-115">SourceId</span><span class="sxs-lookup"><span data-stu-id="e83be-115">SourceId</span></span>](sourceid.md) <br/> |<span data-ttu-id="e83be-116">連絡先または Active Directory 受信者の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="e83be-116">Specifies the identifier of the contact or Active Directory recipient.</span></span>  <br/> |
|[<span data-ttu-id="e83be-117">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="e83be-117">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="e83be-118">フォルダー、連絡先、配布リスト、代理人のユーザー、またはルールの表示名を定義します。</span><span class="sxs-lookup"><span data-stu-id="e83be-118">Defines the display name of a folder, contact, distribution list, delegate user, or rule.</span></span>  <br/> |
|[<span data-ttu-id="e83be-119">IsWritable 可能</span><span class="sxs-lookup"><span data-stu-id="e83be-119">IsWritable</span></span>](iswritable.md) <br/> |<span data-ttu-id="e83be-120">基になる連絡先または Active Directory 受信者に書き込むことができるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e83be-120">Specifies whether the underlying contact or Active Directory recipient can be written to.</span></span>  <br/> |
|[<span data-ttu-id="e83be-121">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="e83be-121">IsQuickContact</span></span>](isquickcontact.md) <br/> |<span data-ttu-id="e83be-122">基になる連絡先または Active Directory 受信者がクイック連絡先であるかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e83be-122">Specifies a Boolean value that indicates whether the underlying contact or Active Directory recipient is a quick contact.</span></span>  <br/> |
|[<span data-ttu-id="e83be-123">IsHidden</span><span class="sxs-lookup"><span data-stu-id="e83be-123">IsHidden</span></span>](ishidden.md) <br/> |<span data-ttu-id="e83be-124">基になる連絡先または Active Directory 受信者を表示するか、ペルソナの一部として表示するかを示すブール値を格納します。</span><span class="sxs-lookup"><span data-stu-id="e83be-124">Contains a Boolean value that indicates whether the underlying contact or Active Directory recipient should be hidden or displayed as part of the persona.</span></span>  <br/> |
|[<span data-ttu-id="e83be-125">FolderId</span><span class="sxs-lookup"><span data-stu-id="e83be-125">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="e83be-126">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e83be-126">Contains the identifier and change key of a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e83be-127">親要素</span><span class="sxs-lookup"><span data-stu-id="e83be-127">Parent elements</span></span>

|<span data-ttu-id="e83be-128">**要素**</span><span class="sxs-lookup"><span data-stu-id="e83be-128">**Element**</span></span>|<span data-ttu-id="e83be-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="e83be-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e83be-130">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="e83be-130">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md) <br/> |<span data-ttu-id="e83be-131">関連付けられたペルソナに集約された1つ以上の連絡先または active directory (AD) 受信者の属性情報の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="e83be-131">Specifies an array of attribution information for one or more of the contacts or active directory (AD) recipients aggregated into the associated persona.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="e83be-132">注釈</span><span class="sxs-lookup"><span data-stu-id="e83be-132">Remarks</span></span>

<span data-ttu-id="e83be-133">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e83be-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e83be-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e83be-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e83be-135">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e83be-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e83be-136">Namespace</span><span class="sxs-lookup"><span data-stu-id="e83be-136">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e83be-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e83be-137">Schema Name</span></span>  <br/> |<span data-ttu-id="e83be-138">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="e83be-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="e83be-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e83be-139">Validation File</span></span>  <br/> |<span data-ttu-id="e83be-140">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e83be-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e83be-141">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e83be-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e83be-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="e83be-142">See also</span></span>

- [<span data-ttu-id="e83be-143">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e83be-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

