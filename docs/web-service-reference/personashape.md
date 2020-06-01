---
title: PersonaShape
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 61d87cd5-3270-40d1-bab7-d0d5bf938607
description: PersonaShape 要素は、FindPeople 要求から返される一連のペルソナプロパティを指定します。
ms.openlocfilehash: 49cbae714a3b854496dc91ea6102f4b676623690
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457572"
---
# <a name="personashape"></a><span data-ttu-id="c52bd-103">PersonaShape</span><span class="sxs-lookup"><span data-stu-id="c52bd-103">PersonaShape</span></span>

<span data-ttu-id="c52bd-104">**PersonaShape**要素は、 **findpeople**要求から返される一連のペルソナプロパティを指定します。</span><span class="sxs-lookup"><span data-stu-id="c52bd-104">The **PersonaShape** element specifies the set of persona properties to be returned from a **FindPeople** request.</span></span> 
  
```XML
<PersonaShape>
   <BaseShape/>
   <AdditionalProperties/>
</PersonaShape>
```

 <span data-ttu-id="c52bd-105">**PersonaResponseShapeType**</span><span class="sxs-lookup"><span data-stu-id="c52bd-105">**PersonaResponseShapeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c52bd-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c52bd-106">Attributes and elements</span></span>

<span data-ttu-id="c52bd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c52bd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c52bd-108">属性</span><span class="sxs-lookup"><span data-stu-id="c52bd-108">Attributes</span></span>

<span data-ttu-id="c52bd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c52bd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c52bd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c52bd-110">Child elements</span></span>

<span data-ttu-id="c52bd-111">[Baseshape](baseshape.md)  | [Additionalproperties](additionalproperties.md)</span><span class="sxs-lookup"><span data-stu-id="c52bd-111">[BaseShape](baseshape.md) | [AdditionalProperties](additionalproperties.md)</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c52bd-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c52bd-112">Parent elements</span></span>

[<span data-ttu-id="c52bd-113">FindPeople</span><span class="sxs-lookup"><span data-stu-id="c52bd-113">FindPeople</span></span>](findpeople.md)
  
## <a name="remarks"></a><span data-ttu-id="c52bd-114">注釈</span><span class="sxs-lookup"><span data-stu-id="c52bd-114">Remarks</span></span>

<span data-ttu-id="c52bd-115">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c52bd-115">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c52bd-116">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c52bd-116">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c52bd-117">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c52bd-117">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c52bd-118">Namespace</span><span class="sxs-lookup"><span data-stu-id="c52bd-118">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c52bd-119">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c52bd-119">Schema name</span></span>  <br/> |<span data-ttu-id="c52bd-120">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="c52bd-120">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c52bd-121">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c52bd-121">Validation file</span></span>  <br/> |<span data-ttu-id="c52bd-122">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c52bd-122">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c52bd-123">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c52bd-123">Can be empty</span></span>  <br/> |<span data-ttu-id="c52bd-124">false</span><span class="sxs-lookup"><span data-stu-id="c52bd-124">false</span></span>  <br/> |
   

