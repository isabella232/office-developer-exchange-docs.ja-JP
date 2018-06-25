---
title: 注釈
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e0392635-9d0f-46d5-84ef-0a8a3036479a
description: アノテーション要素には、ユーザーによって追加されたメモが含まれています。
ms.openlocfilehash: e0170ef9940b64d4c6a10a08182189571f2beb5a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759320"
---
# <a name="annotation"></a><span data-ttu-id="9fe27-103">注釈</span><span class="sxs-lookup"><span data-stu-id="9fe27-103">Annotation</span></span>

<span data-ttu-id="9fe27-104">**アノテーション**要素には、ユーザーによって追加されたメモが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9fe27-104">The **Annotation** element contains optional notes added by a user.</span></span> 
  
```XML
<Annotation></Annotation>
```

 <span data-ttu-id="9fe27-105">**使用されています**</span><span class="sxs-lookup"><span data-stu-id="9fe27-105">**xs:string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9fe27-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9fe27-106">Attributes and elements</span></span>

<span data-ttu-id="9fe27-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9fe27-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9fe27-108">属性</span><span class="sxs-lookup"><span data-stu-id="9fe27-108">Attributes</span></span>

<span data-ttu-id="9fe27-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9fe27-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9fe27-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9fe27-110">Child elements</span></span>

<span data-ttu-id="9fe27-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9fe27-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9fe27-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9fe27-112">Parent elements</span></span>

|<span data-ttu-id="9fe27-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9fe27-113">**Element**</span></span>|<span data-ttu-id="9fe27-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9fe27-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9fe27-115">EnhancedLocation</span><span class="sxs-lookup"><span data-stu-id="9fe27-115">EnhancedLocation</span></span>](enhancedlocation.md) <br/> |<span data-ttu-id="9fe27-116">場所の名前、住所、メモなどの位置情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="9fe27-116">Specifies location information such as the name, address, and optional notes about a location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9fe27-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9fe27-117">Text value</span></span>

<span data-ttu-id="9fe27-118">アノテーション要素のテキスト値では、ユーザーに関するメモを追加する場所です。</span><span class="sxs-lookup"><span data-stu-id="9fe27-118">The text value of the Annotation element is a user added note about a location.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9fe27-119">備考</span><span class="sxs-lookup"><span data-stu-id="9fe27-119">Remarks</span></span>

<span data-ttu-id="9fe27-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9fe27-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9fe27-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9fe27-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9fe27-122">要素情報</span><span class="sxs-lookup"><span data-stu-id="9fe27-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9fe27-123">名前空間</span><span class="sxs-lookup"><span data-stu-id="9fe27-123">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9fe27-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9fe27-124">Schema Name</span></span>  <br/> |<span data-ttu-id="9fe27-125">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="9fe27-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="9fe27-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9fe27-126">Validation File</span></span>  <br/> |<span data-ttu-id="9fe27-127">types.xsd</span><span class="sxs-lookup"><span data-stu-id="9fe27-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9fe27-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9fe27-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9fe27-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="9fe27-129">See also</span></span>

- [<span data-ttu-id="9fe27-130">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9fe27-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

