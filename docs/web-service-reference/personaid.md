---
title: PersonaId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: eec3a468-afd5-4d72-a61e-cd1964fb686c
description: PersonaId 要素では、関連付けられているペルソナのペルソナの識別子を指定します。
ms.openlocfilehash: 77668a1b32a97eef08b3316c7d4d7c8e6494c7bb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832738"
---
# <a name="personaid"></a><span data-ttu-id="e86ea-103">PersonaId</span><span class="sxs-lookup"><span data-stu-id="e86ea-103">PersonaId</span></span>

<span data-ttu-id="e86ea-104">**PersonaId**要素では、関連付けられているペルソナのペルソナの識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="e86ea-104">The **PersonaId** element specifies the persona identifier for the associated persona.</span></span> 
  
```XML
<PersonaId Id="" ChangeKey=""/>
```

 <span data-ttu-id="e86ea-105">**ItemIdType**</span><span class="sxs-lookup"><span data-stu-id="e86ea-105">**ItemIdType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e86ea-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e86ea-106">Attributes and elements</span></span>

<span data-ttu-id="e86ea-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e86ea-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e86ea-108">属性</span><span class="sxs-lookup"><span data-stu-id="e86ea-108">Attributes</span></span>

|<span data-ttu-id="e86ea-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="e86ea-109">**Attribute**</span></span>|<span data-ttu-id="e86ea-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="e86ea-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e86ea-111">ID</span><span class="sxs-lookup"><span data-stu-id="e86ea-111">Id</span></span>  <br/> |<span data-ttu-id="e86ea-112">**Id**属性のテキスト値は、ペルソナの識別子です。</span><span class="sxs-lookup"><span data-stu-id="e86ea-112">The text value of the **Id** attribute is the identifier of the persona.</span></span>  <br/> |
|<span data-ttu-id="e86ea-113">ChangeKey</span><span class="sxs-lookup"><span data-stu-id="e86ea-113">ChangeKey</span></span>  <br/> |<span data-ttu-id="e86ea-114">**変更キー**属性のテキスト値は、ペルソナの変更キーです。</span><span class="sxs-lookup"><span data-stu-id="e86ea-114">The text value of the **ChangeKey** attribute is the change key of the persona.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e86ea-115">子要素</span><span class="sxs-lookup"><span data-stu-id="e86ea-115">Child elements</span></span>

<span data-ttu-id="e86ea-116">なし。</span><span class="sxs-lookup"><span data-stu-id="e86ea-116">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e86ea-117">親要素</span><span class="sxs-lookup"><span data-stu-id="e86ea-117">Parent elements</span></span>

<span data-ttu-id="e86ea-118">[GetPersona](getpersona.md) | [ペルソナ](persona.md)</span><span class="sxs-lookup"><span data-stu-id="e86ea-118">[GetPersona](getpersona.md) | [Persona](persona.md)</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e86ea-119">備考</span><span class="sxs-lookup"><span data-stu-id="e86ea-119">Remarks</span></span>

<span data-ttu-id="e86ea-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e86ea-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e86ea-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e86ea-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e86ea-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="e86ea-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e86ea-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="e86ea-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e86ea-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e86ea-124">Schema name</span></span>  <br/> |<span data-ttu-id="e86ea-125">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e86ea-125">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e86ea-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e86ea-126">Validation file</span></span>  <br/> |<span data-ttu-id="e86ea-127">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e86ea-127">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e86ea-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e86ea-128">Can be empty</span></span>  <br/> ||
   

