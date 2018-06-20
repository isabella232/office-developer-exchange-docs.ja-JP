---
title: DisplayNameFirstLast
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 013c17c9-cb37-4028-9fe6-c3f47441d0f7
description: DisplayNameFirstLast 要素は、形式で、名、姓、名のペルソナが関連付けられている表示名を指定します。
ms.openlocfilehash: 7a8c269c7e1b03448d176a630fbcae979926bdf4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760114"
---
# <a name="displaynamefirstlast"></a><span data-ttu-id="cad32-103">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="cad32-103">DisplayNameFirstLast</span></span>

<span data-ttu-id="cad32-104">**DisplayNameFirstLast**要素は、形式、「氏名」、"Last Name"に関連付けられているペルソナの表示名を指定します。</span><span class="sxs-lookup"><span data-stu-id="cad32-104">The **DisplayNameFirstLast** element specifies the display name of the associated persona in the format, "First Name", "Last Name".</span></span> 
  
```XML
<DisplayNameFirstLast>
```

 <span data-ttu-id="cad32-105">**string**</span><span class="sxs-lookup"><span data-stu-id="cad32-105">**string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cad32-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cad32-106">Attributes and elements</span></span>

<span data-ttu-id="cad32-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cad32-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cad32-108">属性</span><span class="sxs-lookup"><span data-stu-id="cad32-108">Attributes</span></span>

<span data-ttu-id="cad32-109">なし。</span><span class="sxs-lookup"><span data-stu-id="cad32-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="cad32-110">子要素</span><span class="sxs-lookup"><span data-stu-id="cad32-110">Child elements</span></span>

<span data-ttu-id="cad32-111">なし。</span><span class="sxs-lookup"><span data-stu-id="cad32-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="cad32-112">親要素</span><span class="sxs-lookup"><span data-stu-id="cad32-112">Parent elements</span></span>

|<span data-ttu-id="cad32-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="cad32-113">**Element**</span></span>|<span data-ttu-id="cad32-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="cad32-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cad32-115">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="cad32-115">Persona</span></span>](persona.md) <br/> |<span data-ttu-id="cad32-116">**GetPersona**の要求によって返されるペルソナ データのセットを指定します。</span><span class="sxs-lookup"><span data-stu-id="cad32-116">Specifies a set of persona data returned by a **GetPersona** request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cad32-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cad32-117">Text value</span></span>

<span data-ttu-id="cad32-118">**DisplayNameFirstLast**要素のテキスト値は、最初に指定した名前の表示名を含む文字列値です。</span><span class="sxs-lookup"><span data-stu-id="cad32-118">The text value of the **DisplayNameFirstLast** element is a string value containing the display name, with the given name first.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="cad32-119">備考</span><span class="sxs-lookup"><span data-stu-id="cad32-119">Remarks</span></span>

<span data-ttu-id="cad32-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="cad32-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="cad32-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cad32-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cad32-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="cad32-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cad32-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="cad32-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="cad32-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cad32-124">Schema Name</span></span>  <br/> |<span data-ttu-id="cad32-125">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="cad32-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="cad32-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cad32-126">Validation File</span></span>  <br/> |<span data-ttu-id="cad32-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="cad32-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="cad32-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cad32-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="cad32-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="cad32-129">See also</span></span>

- [<span data-ttu-id="cad32-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="cad32-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

