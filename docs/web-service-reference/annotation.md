---
title: アノテーションフィーチャー
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e0392635-9d0f-46d5-84ef-0a8a3036479a
description: Annotation 要素には、ユーザーが追加したオプションのメモが含まれています。
ms.openlocfilehash: 291d875085f9bc13e92a14b844b66878f5e6eb2a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466116"
---
# <a name="annotation"></a><span data-ttu-id="20854-103">アノテーションフィーチャー</span><span class="sxs-lookup"><span data-stu-id="20854-103">Annotation</span></span>

<span data-ttu-id="20854-104">**Annotation**要素には、ユーザーが追加したオプションのメモが含まれています。</span><span class="sxs-lookup"><span data-stu-id="20854-104">The **Annotation** element contains optional notes added by a user.</span></span> 
  
```XML
<Annotation></Annotation>
```

 <span data-ttu-id="20854-105">**xs: 文字列**</span><span class="sxs-lookup"><span data-stu-id="20854-105">**xs:string**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="20854-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="20854-106">Attributes and elements</span></span>

<span data-ttu-id="20854-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="20854-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="20854-108">属性</span><span class="sxs-lookup"><span data-stu-id="20854-108">Attributes</span></span>

<span data-ttu-id="20854-109">なし。</span><span class="sxs-lookup"><span data-stu-id="20854-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="20854-110">子要素</span><span class="sxs-lookup"><span data-stu-id="20854-110">Child elements</span></span>

<span data-ttu-id="20854-111">なし。</span><span class="sxs-lookup"><span data-stu-id="20854-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="20854-112">親要素</span><span class="sxs-lookup"><span data-stu-id="20854-112">Parent elements</span></span>

|<span data-ttu-id="20854-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="20854-113">**Element**</span></span>|<span data-ttu-id="20854-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="20854-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="20854-115">EnhancedLocation</span><span class="sxs-lookup"><span data-stu-id="20854-115">EnhancedLocation</span></span>](enhancedlocation.md) <br/> |<span data-ttu-id="20854-116">場所に関する名前、住所、オプションのメモなどの場所情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="20854-116">Specifies location information such as the name, address, and optional notes about a location.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="20854-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="20854-117">Text value</span></span>

<span data-ttu-id="20854-118">Annotation 要素のテキスト値は、ユーザーが場所に関するメモを追加したことを示します。</span><span class="sxs-lookup"><span data-stu-id="20854-118">The text value of the Annotation element is a user added note about a location.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="20854-119">注釈</span><span class="sxs-lookup"><span data-stu-id="20854-119">Remarks</span></span>

<span data-ttu-id="20854-120">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="20854-120">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="20854-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="20854-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="20854-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="20854-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="20854-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="20854-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="20854-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="20854-124">Schema Name</span></span>  <br/> |<span data-ttu-id="20854-125">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="20854-125">Type schema</span></span>  <br/> |
|<span data-ttu-id="20854-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="20854-126">Validation File</span></span>  <br/> |<span data-ttu-id="20854-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="20854-127">types.xsd</span></span>  <br/> |
|<span data-ttu-id="20854-128">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="20854-128">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="20854-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="20854-129">See also</span></span>

- [<span data-ttu-id="20854-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="20854-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

