---
title: PersonaShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 61d87cd5-3270-40d1-bab7-d0d5bf938607
description: PersonaShape 要素は、ペルソナの FindPeople 要求から返されるプロパティのセットを指定します。
ms.openlocfilehash: f974c62c3c255a58d28ec716ffb34dc8964d1cfe
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832743"
---
# <a name="personashape"></a><span data-ttu-id="25096-103">PersonaShape</span><span class="sxs-lookup"><span data-stu-id="25096-103">PersonaShape</span></span>

<span data-ttu-id="25096-104">**PersonaShape**要素は、ペルソナの**FindPeople**要求から返されるプロパティのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="25096-104">The **PersonaShape** element specifies the set of persona properties to be returned from a **FindPeople** request.</span></span> 
  
```XML
<PersonaShape>
   <BaseShape/>
   <AdditionalProperties/>
</PersonaShape>
```

 <span data-ttu-id="25096-105">**PersonaResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="25096-105">**PersonaResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="25096-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="25096-106">Attributes and elements</span></span>

<span data-ttu-id="25096-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="25096-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="25096-108">属性</span><span class="sxs-lookup"><span data-stu-id="25096-108">Attributes</span></span>

<span data-ttu-id="25096-109">なし。</span><span class="sxs-lookup"><span data-stu-id="25096-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="25096-110">子要素</span><span class="sxs-lookup"><span data-stu-id="25096-110">Child elements</span></span>

<span data-ttu-id="25096-111">[BaseShape](baseshape.md) | [AdditionalProperties](additionalproperties.md)</span><span class="sxs-lookup"><span data-stu-id="25096-111">[BaseShape](baseshape.md) | [AdditionalProperties](additionalproperties.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="25096-112">親要素</span><span class="sxs-lookup"><span data-stu-id="25096-112">Parent elements</span></span>

[<span data-ttu-id="25096-113">FindPeople</span><span class="sxs-lookup"><span data-stu-id="25096-113">FindPeople</span></span>](findpeople.md)
  
## <a name="remarks"></a><span data-ttu-id="25096-114">備考</span><span class="sxs-lookup"><span data-stu-id="25096-114">Remarks</span></span>

<span data-ttu-id="25096-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="25096-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="25096-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="25096-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="25096-117">要素情報</span><span class="sxs-lookup"><span data-stu-id="25096-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="25096-118">名前空間</span><span class="sxs-lookup"><span data-stu-id="25096-118">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="25096-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="25096-119">Schema name</span></span>  <br/> |<span data-ttu-id="25096-120">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="25096-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="25096-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="25096-121">Validation file</span></span>  <br/> |<span data-ttu-id="25096-122">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="25096-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="25096-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="25096-123">Can be empty</span></span>  <br/> |<span data-ttu-id="25096-124">false</span><span class="sxs-lookup"><span data-stu-id="25096-124">false</span></span>  <br/> |
   

