---
title: YomiCompanyNames
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5c414af9-34d0-41ce-bda9-0d4ca3f3be79
description: YomiCompanyNames 要素では、関連付けられているペルソナについて、ふりがな (日本語) の会社名とそのソース attributions の識別子の配列を指定します。
ms.openlocfilehash: 41b97998425926750a3ecc7e17233f2066759689
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457866"
---
# <a name="yomicompanynames"></a><span data-ttu-id="e24fc-103">YomiCompanyNames</span><span class="sxs-lookup"><span data-stu-id="e24fc-103">YomiCompanyNames</span></span>

<span data-ttu-id="e24fc-104">**YomiCompanyNames**要素では、関連付けられているペルソナについて、ふりがな (日本語) の会社名とそのソース attributions の識別子の配列を指定します。</span><span class="sxs-lookup"><span data-stu-id="e24fc-104">The **YomiCompanyNames** element specifies an array of phonetic Japanese company names and the identifiers of their source attributions for the associated persona.</span></span> 
  
```XML
<YomiCompanyNames>
   <StringAttributedValue/>
</YomiCompanyNames>
```

 <span data-ttu-id="e24fc-105">**ArrayOfStringAttributedValuesType**</span><span class="sxs-lookup"><span data-stu-id="e24fc-105">**ArrayOfStringAttributedValuesType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e24fc-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e24fc-106">Attributes and elements</span></span>

<span data-ttu-id="e24fc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e24fc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e24fc-108">属性</span><span class="sxs-lookup"><span data-stu-id="e24fc-108">Attributes</span></span>

<span data-ttu-id="e24fc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e24fc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e24fc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e24fc-110">Child elements</span></span>

[<span data-ttu-id="e24fc-111">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="e24fc-111">StringAttributedValue</span></span>](stringattributedvalue.md)
  
### <a name="parent-elements"></a><span data-ttu-id="e24fc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e24fc-112">Parent elements</span></span>

[<span data-ttu-id="e24fc-113">ユーザー</span><span class="sxs-lookup"><span data-stu-id="e24fc-113">Persona</span></span>](persona.md)
  
## <a name="remarks"></a><span data-ttu-id="e24fc-114">注釈</span><span class="sxs-lookup"><span data-stu-id="e24fc-114">Remarks</span></span>

<span data-ttu-id="e24fc-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e24fc-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e24fc-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e24fc-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e24fc-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e24fc-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e24fc-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="e24fc-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e24fc-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e24fc-119">Schema name</span></span>  <br/> |<span data-ttu-id="e24fc-120">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e24fc-120">Types schema</span></span>  <br/> |
|<span data-ttu-id="e24fc-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e24fc-121">Validation file</span></span>  <br/> |<span data-ttu-id="e24fc-122">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e24fc-122">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e24fc-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e24fc-123">Can be empty</span></span>  <br/> ||
   

