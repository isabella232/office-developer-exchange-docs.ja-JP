---
title: PersonaId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: eec3a468-afd5-4d72-a61e-cd1964fb686c
description: 個人情報要素は、関連付けられたペルソナのペルソナ識別子を指定します。
ms.openlocfilehash: 3d7315097a14fb1eed5f378422cba80414601675
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457243"
---
# <a name="personaid"></a><span data-ttu-id="70903-103">PersonaId</span><span class="sxs-lookup"><span data-stu-id="70903-103">PersonaId</span></span>

<span data-ttu-id="70903-104">**個人**情報要素は、関連付けられたペルソナのペルソナ識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="70903-104">The **PersonaId** element specifies the persona identifier for the associated persona.</span></span> 
  
```XML
<PersonaId Id="" ChangeKey=""/>
```

 <span data-ttu-id="70903-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="70903-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70903-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="70903-106">Attributes and elements</span></span>

<span data-ttu-id="70903-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="70903-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70903-108">属性</span><span class="sxs-lookup"><span data-stu-id="70903-108">Attributes</span></span>

|<span data-ttu-id="70903-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="70903-109">**Attribute**</span></span>|<span data-ttu-id="70903-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="70903-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="70903-111">ID</span><span class="sxs-lookup"><span data-stu-id="70903-111">Id</span></span>  <br/> |<span data-ttu-id="70903-112">**Id**属性のテキスト値は、ペルソナの識別子です。</span><span class="sxs-lookup"><span data-stu-id="70903-112">The text value of the **Id** attribute is the identifier of the persona.</span></span>  <br/> |
|<span data-ttu-id="70903-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="70903-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="70903-114">**Changekey**属性のテキスト値は、ペルソナの変更キーです。</span><span class="sxs-lookup"><span data-stu-id="70903-114">The text value of the **ChangeKey** attribute is the change key of the persona.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="70903-115">子要素</span><span class="sxs-lookup"><span data-stu-id="70903-115">Child elements</span></span>

<span data-ttu-id="70903-116">なし。</span><span class="sxs-lookup"><span data-stu-id="70903-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="70903-117">親要素</span><span class="sxs-lookup"><span data-stu-id="70903-117">Parent elements</span></span>

<span data-ttu-id="70903-118">[Getpersona](getpersona.md)  | [Persona](persona.md)</span><span class="sxs-lookup"><span data-stu-id="70903-118">[GetPersona](getpersona.md) | [Persona](persona.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="70903-119">注釈</span><span class="sxs-lookup"><span data-stu-id="70903-119">Remarks</span></span>

<span data-ttu-id="70903-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="70903-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="70903-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="70903-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70903-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="70903-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70903-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="70903-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="70903-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="70903-124">Schema name</span></span>  <br/> |<span data-ttu-id="70903-125">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="70903-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="70903-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="70903-126">Validation file</span></span>  <br/> |<span data-ttu-id="70903-127">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="70903-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="70903-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="70903-128">Can be empty</span></span>  <br/> ||
   

