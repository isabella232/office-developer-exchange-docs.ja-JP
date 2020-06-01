---
title: SourceId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fccdedc0-83ed-4bb7-a1d2-623e70d1a7bf
description: SourceId 要素は、ペルソナの属性付き連絡先の識別子を指定します。
ms.openlocfilehash: a795f9fa2cc2084bee34c82b6df9567c79d430eb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465759"
---
# <a name="sourceid"></a><span data-ttu-id="25884-103">SourceId</span><span class="sxs-lookup"><span data-stu-id="25884-103">SourceId</span></span>

<span data-ttu-id="25884-104">**SourceId**要素は、ペルソナの属性付き連絡先の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="25884-104">The **SourceId** element specifies the identifier of the attributed contact in a persona.</span></span> 
  
```XML
<SourceId Id="" ChangeKey=""/>
```

 <span data-ttu-id="25884-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="25884-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="25884-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="25884-106">Attributes and elements</span></span>

<span data-ttu-id="25884-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="25884-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25884-108">属性</span><span class="sxs-lookup"><span data-stu-id="25884-108">Attributes</span></span>

|<span data-ttu-id="25884-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="25884-109">**Attribute**</span></span>|<span data-ttu-id="25884-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="25884-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="25884-111">ID</span><span class="sxs-lookup"><span data-stu-id="25884-111">Id</span></span>  <br/> |<span data-ttu-id="25884-112">**Id**属性のテキスト値は、連絡先の識別子です。</span><span class="sxs-lookup"><span data-stu-id="25884-112">The text value of the **Id** attribute is the identifier of the contact.</span></span>  <br/> |
|<span data-ttu-id="25884-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="25884-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="25884-114">**Changekey**属性のテキスト値は、連絡先の変更キーです。</span><span class="sxs-lookup"><span data-stu-id="25884-114">The text value of the **ChangeKey** attribute is the change key of the contact.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="25884-115">子要素</span><span class="sxs-lookup"><span data-stu-id="25884-115">Child elements</span></span>

<span data-ttu-id="25884-116">なし。</span><span class="sxs-lookup"><span data-stu-id="25884-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="25884-117">親要素</span><span class="sxs-lookup"><span data-stu-id="25884-117">Parent elements</span></span>

[<span data-ttu-id="25884-118">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="25884-118">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
  
## <a name="remarks"></a><span data-ttu-id="25884-119">注釈</span><span class="sxs-lookup"><span data-stu-id="25884-119">Remarks</span></span>

<span data-ttu-id="25884-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="25884-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="25884-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="25884-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25884-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="25884-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25884-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="25884-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="25884-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="25884-124">Schema name</span></span>  <br/> |<span data-ttu-id="25884-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="25884-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="25884-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="25884-126">Validation file</span></span>  <br/> |<span data-ttu-id="25884-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="25884-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="25884-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="25884-128">Can be empty</span></span>  <br/> ||
   

