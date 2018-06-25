---
title: 属性 (PersonaAttributionType)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dc59e17e-baea-4617-8ca1-4382a89de0d7
description: 属性要素は、PersonaType 要素の属性の配列のインスタンスを指定します。
ms.openlocfilehash: 0e800c92c75bf0c475d4bffd33d6ab49f9ad9a9a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759465"
---
# <a name="attribution-personaattributiontype"></a><span data-ttu-id="d25bf-103">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="d25bf-103">Attribution (PersonaAttributionType)</span></span>

<span data-ttu-id="d25bf-104">**属性**要素は、 **PersonaType**要素の属性の配列のインスタンスを指定します。</span><span class="sxs-lookup"><span data-stu-id="d25bf-104">The **Attribution** element specifies an instance in an array of attributes for a **PersonaType** element.</span></span> 
  
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

 <span data-ttu-id="d25bf-105">**PersonaAttributionType**</span><span class="sxs-lookup"><span data-stu-id="d25bf-105">**PersonaAttributionType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d25bf-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d25bf-106">Attributes and elements</span></span>

<span data-ttu-id="d25bf-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d25bf-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d25bf-108">属性</span><span class="sxs-lookup"><span data-stu-id="d25bf-108">Attributes</span></span>

<span data-ttu-id="d25bf-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d25bf-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d25bf-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d25bf-110">Child elements</span></span>

|<span data-ttu-id="d25bf-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="d25bf-111">**Element**</span></span>|<span data-ttu-id="d25bf-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d25bf-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d25bf-113">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="d25bf-113">ID (String)</span></span>](id-string.md) <br/> |<span data-ttu-id="d25bf-114">アプリケーションか、ペルソナで、属性を一意に識別する文字列を指定します。</span><span class="sxs-lookup"><span data-stu-id="d25bf-114">Specifies a string that uniquely identifies an app or an attribution in a persona.</span></span>  <br/> |
|[<span data-ttu-id="d25bf-115">SourceId</span><span class="sxs-lookup"><span data-stu-id="d25bf-115">SourceId</span></span>](sourceid.md) <br/> |<span data-ttu-id="d25bf-116">連絡先または Active Directory の受信者の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="d25bf-116">Specifies the identifier of the contact or Active Directory recipient.</span></span>  <br/> |
|[<span data-ttu-id="d25bf-117">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="d25bf-117">DisplayName (string)</span></span>](displayname-string.md) <br/> |<span data-ttu-id="d25bf-118">フォルダー、連絡先、配布リスト、ユーザーの代理人、またはルールの表示名を定義します。</span><span class="sxs-lookup"><span data-stu-id="d25bf-118">Defines the display name of a folder, contact, distribution list, delegate user, or rule.</span></span>  <br/> |
|[<span data-ttu-id="d25bf-119">IsWritable</span><span class="sxs-lookup"><span data-stu-id="d25bf-119">IsWritable</span></span>](iswritable.md) <br/> |<span data-ttu-id="d25bf-120">基になっている取引先担当者または Active Directory の受信者に書き込むことがあるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d25bf-120">Specifies whether the underlying contact or Active Directory recipient can be written to.</span></span>  <br/> |
|[<span data-ttu-id="d25bf-121">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="d25bf-121">IsQuickContact</span></span>](isquickcontact.md) <br/> |<span data-ttu-id="d25bf-122">基になっている取引先担当者または Active Directory の受信者は、クイック連絡先かどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="d25bf-122">Specifies a Boolean value that indicates whether the underlying contact or Active Directory recipient is a quick contact.</span></span>  <br/> |
|[<span data-ttu-id="d25bf-123">IsHidden</span><span class="sxs-lookup"><span data-stu-id="d25bf-123">IsHidden</span></span>](ishidden.md) <br/> |<span data-ttu-id="d25bf-124">かどうか、基になっている取引先担当者または Active Directory の受信者する非表示か、ペルソナの一部として表示を示すブール値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d25bf-124">Contains a Boolean value that indicates whether the underlying contact or Active Directory recipient should be hidden or displayed as part of the persona.</span></span>  <br/> |
|[<span data-ttu-id="d25bf-125">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="d25bf-125">FolderId</span></span>](folderid.md) <br/> |<span data-ttu-id="d25bf-126">フォルダーの識別子と変更キーが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d25bf-126">Contains the identifier and change key of a folder.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d25bf-127">親要素</span><span class="sxs-lookup"><span data-stu-id="d25bf-127">Parent elements</span></span>

|<span data-ttu-id="d25bf-128">**要素**</span><span class="sxs-lookup"><span data-stu-id="d25bf-128">**Element**</span></span>|<span data-ttu-id="d25bf-129">**説明**</span><span class="sxs-lookup"><span data-stu-id="d25bf-129">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d25bf-130">帰属 (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="d25bf-130">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md) <br/> |<span data-ttu-id="d25bf-131">1 つまたは複数の連絡先や関連するペルソナに集計される active directory (AD) の受信者の属性情報の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="d25bf-131">Specifies an array of attribution information for one or more of the contacts or active directory (AD) recipients aggregated into the associated persona.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d25bf-132">備考</span><span class="sxs-lookup"><span data-stu-id="d25bf-132">Remarks</span></span>

<span data-ttu-id="d25bf-133">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d25bf-133">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d25bf-134">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d25bf-134">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d25bf-135">要素情報</span><span class="sxs-lookup"><span data-stu-id="d25bf-135">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d25bf-136">名前空間</span><span class="sxs-lookup"><span data-stu-id="d25bf-136">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d25bf-137">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d25bf-137">Schema Name</span></span>  <br/> |<span data-ttu-id="d25bf-138">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="d25bf-138">Type schema</span></span>  <br/> |
|<span data-ttu-id="d25bf-139">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d25bf-139">Validation File</span></span>  <br/> |<span data-ttu-id="d25bf-140">types.xsd</span><span class="sxs-lookup"><span data-stu-id="d25bf-140">types.xsd</span></span>  <br/> |
|<span data-ttu-id="d25bf-141">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d25bf-141">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d25bf-142">関連項目</span><span class="sxs-lookup"><span data-stu-id="d25bf-142">See also</span></span>

- [<span data-ttu-id="d25bf-143">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d25bf-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

