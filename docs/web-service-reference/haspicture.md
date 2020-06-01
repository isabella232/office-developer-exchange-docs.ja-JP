---
title: HasPicture
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- HasPicture
api_type:
- schema
ms.assetid: 922a43fe-01bd-49f2-9261-e00e4699b8da
description: HasPicture 要素は、連絡先アイテムに連絡先の画像を表す添付ファイルがあるかどうかを示します。
ms.openlocfilehash: 0f0758e38807587d47b9469f40b10bd9c6ea5012
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462438"
---
# <a name="haspicture"></a><span data-ttu-id="167c3-103">HasPicture</span><span class="sxs-lookup"><span data-stu-id="167c3-103">HasPicture</span></span>

<span data-ttu-id="167c3-104">**Haspicture**要素は、連絡先アイテムに連絡先の画像を表す添付ファイルがあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="167c3-104">The **HasPicture** element indicates whether the contact item has a file attachment that represents the contact's picture.</span></span> 
  
[<span data-ttu-id="167c3-105">連絡先</span><span class="sxs-lookup"><span data-stu-id="167c3-105">Contact</span></span>](contact.md)
  
[<span data-ttu-id="167c3-106">HasPicture</span><span class="sxs-lookup"><span data-stu-id="167c3-106">HasPicture</span></span>](haspicture.md)
  
```xml
<HasPicture>true or false</HasPicture>
```

 <span data-ttu-id="167c3-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="167c3-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="167c3-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="167c3-108">Attributes and elements</span></span>

<span data-ttu-id="167c3-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="167c3-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="167c3-110">属性</span><span class="sxs-lookup"><span data-stu-id="167c3-110">Attributes</span></span>

<span data-ttu-id="167c3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="167c3-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="167c3-112">子要素</span><span class="sxs-lookup"><span data-stu-id="167c3-112">Child elements</span></span>

<span data-ttu-id="167c3-113">なし。</span><span class="sxs-lookup"><span data-stu-id="167c3-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="167c3-114">親要素</span><span class="sxs-lookup"><span data-stu-id="167c3-114">Parent elements</span></span>

|<span data-ttu-id="167c3-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="167c3-115">**Element**</span></span>|<span data-ttu-id="167c3-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="167c3-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="167c3-117">連絡先</span><span class="sxs-lookup"><span data-stu-id="167c3-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="167c3-118">Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="167c3-118">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="167c3-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="167c3-119">Text value</span></span>

<span data-ttu-id="167c3-120">**Haspicture**要素のテキスト値には、 **true**または**false**のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="167c3-120">The text value of the **HasPicture** element can be either **true** or **false**.</span></span> <span data-ttu-id="167c3-121">既定値は **false** です。</span><span class="sxs-lookup"><span data-stu-id="167c3-121">The default value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="167c3-122">注釈</span><span class="sxs-lookup"><span data-stu-id="167c3-122">Remarks</span></span>

<span data-ttu-id="167c3-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="167c3-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="167c3-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="167c3-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="167c3-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="167c3-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="167c3-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="167c3-126">Schema Name</span></span>  <br/> |<span data-ttu-id="167c3-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="167c3-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="167c3-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="167c3-128">Validation File</span></span>  <br/> |<span data-ttu-id="167c3-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="167c3-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="167c3-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="167c3-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="167c3-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="167c3-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="167c3-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="167c3-132">See also</span></span>



- [<span data-ttu-id="167c3-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="167c3-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

