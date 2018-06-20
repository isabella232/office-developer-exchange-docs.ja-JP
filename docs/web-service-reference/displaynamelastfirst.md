---
title: DisplayNameLastFirst
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d392e138-a514-4bce-81b1-1f484e353d1c
description: DisplayNameLastFirst 要素は、形式で、姓、名、姓のペルソナが関連付けられている表示名を指定します。
ms.openlocfilehash: 68ebf0e91e216cffa1ba8db425de248f0d4e77b7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760125"
---
# <a name="displaynamelastfirst"></a><span data-ttu-id="9c7df-103">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="9c7df-103">DisplayNameLastFirst</span></span>

<span data-ttu-id="9c7df-104">**DisplayNameLastFirst**要素は、形式で、「姓」、「氏名」のペルソナが関連付けられている表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="9c7df-104">The **DisplayNameLastFirst** element specifies the display name of the associated persona in the format, "Last Name", "First Name".</span></span> 
  
```XML
<DisplayNameLastFirst></DisplayNameLastFirst>
```

 <span data-ttu-id="9c7df-105">**string**</span><span class="sxs-lookup"><span data-stu-id="9c7df-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9c7df-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9c7df-106">Attributes and elements</span></span>

<span data-ttu-id="9c7df-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9c7df-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9c7df-108">属性</span><span class="sxs-lookup"><span data-stu-id="9c7df-108">Attributes</span></span>

<span data-ttu-id="9c7df-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9c7df-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9c7df-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9c7df-110">Child elements</span></span>

<span data-ttu-id="9c7df-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9c7df-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9c7df-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9c7df-112">Parent elements</span></span>

|<span data-ttu-id="9c7df-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9c7df-113">**Element**</span></span>|<span data-ttu-id="9c7df-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9c7df-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9c7df-115">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="9c7df-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="9c7df-116">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="9c7df-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9c7df-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9c7df-117">Text value</span></span>

<span data-ttu-id="9c7df-118">**DisplayNameLastFirst**要素のテキスト値は、姓を持つ最初の表示名を指定する文字列値です。</span><span class="sxs-lookup"><span data-stu-id="9c7df-118">The text value of the **DisplayNameLastFirst** element is a string value that specifies the display name, with the surname first.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9c7df-119">備考</span><span class="sxs-lookup"><span data-stu-id="9c7df-119">Remarks</span></span>

<span data-ttu-id="9c7df-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9c7df-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9c7df-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9c7df-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9c7df-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="9c7df-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9c7df-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="9c7df-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9c7df-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9c7df-124">Schema Name</span></span>  <br/> |<span data-ttu-id="9c7df-125">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="9c7df-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="9c7df-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9c7df-126">Validation File</span></span>  <br/> |<span data-ttu-id="9c7df-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="9c7df-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9c7df-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9c7df-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9c7df-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="9c7df-129">See also</span></span>

- [<span data-ttu-id="9c7df-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9c7df-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

