---
title: SourceId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: fccdedc0-83ed-4bb7-a1d2-623e70d1a7bf
description: SourceId 要素では、ペルソナの属性付きの取引先担当者の識別子を指定します。
ms.openlocfilehash: b08c28f93318a01e45a0d9cb812fef01905694ac
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833521"
---
# <a name="sourceid"></a><span data-ttu-id="42fff-103">SourceId</span><span class="sxs-lookup"><span data-stu-id="42fff-103">SourceId</span></span>

<span data-ttu-id="42fff-104">**SourceId**要素では、ペルソナの属性付きの取引先担当者の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="42fff-104">The **SourceId** element specifies the identifier of the attributed contact in a persona.</span></span> 
  
```XML
<SourceId Id="" ChangeKey=""/>
```

 <span data-ttu-id="42fff-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="42fff-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="42fff-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="42fff-106">Attributes and elements</span></span>

<span data-ttu-id="42fff-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="42fff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="42fff-108">属性</span><span class="sxs-lookup"><span data-stu-id="42fff-108">Attributes</span></span>

|<span data-ttu-id="42fff-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="42fff-109">**Attribute**</span></span>|<span data-ttu-id="42fff-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="42fff-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="42fff-111">ID</span><span class="sxs-lookup"><span data-stu-id="42fff-111">Id</span></span>  <br/> |<span data-ttu-id="42fff-112">**Id**属性のテキスト値は、取引先担当者の識別子です。</span><span class="sxs-lookup"><span data-stu-id="42fff-112">The text value of the **Id** attribute is the identifier of the contact.</span></span>  <br/> |
|<span data-ttu-id="42fff-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="42fff-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="42fff-114">**変更キー**属性のテキスト値は、連絡先の変更キーです。</span><span class="sxs-lookup"><span data-stu-id="42fff-114">The text value of the **ChangeKey** attribute is the change key of the contact.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="42fff-115">子要素</span><span class="sxs-lookup"><span data-stu-id="42fff-115">Child elements</span></span>

<span data-ttu-id="42fff-116">なし。</span><span class="sxs-lookup"><span data-stu-id="42fff-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="42fff-117">親要素</span><span class="sxs-lookup"><span data-stu-id="42fff-117">Parent elements</span></span>

[<span data-ttu-id="42fff-118">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="42fff-118">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
  
## <a name="remarks"></a><span data-ttu-id="42fff-119">備考</span><span class="sxs-lookup"><span data-stu-id="42fff-119">Remarks</span></span>

<span data-ttu-id="42fff-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="42fff-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="42fff-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="42fff-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="42fff-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="42fff-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="42fff-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="42fff-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="42fff-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="42fff-124">Schema name</span></span>  <br/> |<span data-ttu-id="42fff-125">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="42fff-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="42fff-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="42fff-126">Validation file</span></span>  <br/> |<span data-ttu-id="42fff-127">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="42fff-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="42fff-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="42fff-128">Can be empty</span></span>  <br/> ||
   

