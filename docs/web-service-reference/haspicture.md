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
description: HasPicture 要素は、連絡先アイテムに連絡先の画像を表すファイルの添付ファイルがあるかどうかを示します。
ms.openlocfilehash: 8f6890ec2bcc9a961f69331fb20f5cad8a59bf38
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831806"
---
# <a name="haspicture"></a><span data-ttu-id="04a04-103">HasPicture</span><span class="sxs-lookup"><span data-stu-id="04a04-103">HasPicture</span></span>

<span data-ttu-id="04a04-104">**HasPicture**要素は、連絡先アイテムに連絡先の画像を表すファイルの添付ファイルがあるかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="04a04-104">The **HasPicture** element indicates whether the contact item has a file attachment that represents the contact's picture.</span></span> 
  
[<span data-ttu-id="04a04-105">Contact</span><span class="sxs-lookup"><span data-stu-id="04a04-105">Contact</span></span>](contact.md)
  
[<span data-ttu-id="04a04-106">HasPicture</span><span class="sxs-lookup"><span data-stu-id="04a04-106">HasPicture</span></span>](haspicture.md)
  
```xml
<HasPicture>true or false</HasPicture>
```

 <span data-ttu-id="04a04-107">**boolean**</span><span class="sxs-lookup"><span data-stu-id="04a04-107">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="04a04-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="04a04-108">Attributes and elements</span></span>

<span data-ttu-id="04a04-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="04a04-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="04a04-110">属性</span><span class="sxs-lookup"><span data-stu-id="04a04-110">Attributes</span></span>

<span data-ttu-id="04a04-111">なし。</span><span class="sxs-lookup"><span data-stu-id="04a04-111">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="04a04-112">子要素</span><span class="sxs-lookup"><span data-stu-id="04a04-112">Child elements</span></span>

<span data-ttu-id="04a04-113">なし。</span><span class="sxs-lookup"><span data-stu-id="04a04-113">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="04a04-114">親要素</span><span class="sxs-lookup"><span data-stu-id="04a04-114">Parent elements</span></span>

|<span data-ttu-id="04a04-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="04a04-115">**Element**</span></span>|<span data-ttu-id="04a04-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="04a04-116">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="04a04-117">Contact</span><span class="sxs-lookup"><span data-stu-id="04a04-117">Contact</span></span>](contact.md) <br/> |<span data-ttu-id="04a04-118">Exchange ストア内の連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="04a04-118">Represents a contact item in the Exchange store.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="04a04-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="04a04-119">Text value</span></span>

<span data-ttu-id="04a04-120">**HasPicture**要素のテキスト値には、 **true**または**false**のいずれかを指定できます。</span><span class="sxs-lookup"><span data-stu-id="04a04-120">The text value of the **HasPicture** element can be either **true** or **false**.</span></span> <span data-ttu-id="04a04-121">既定値は、 **false を指定**します。</span><span class="sxs-lookup"><span data-stu-id="04a04-121">The default value is **false**.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="04a04-122">備考</span><span class="sxs-lookup"><span data-stu-id="04a04-122">Remarks</span></span>

<span data-ttu-id="04a04-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="04a04-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="04a04-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="04a04-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="04a04-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="04a04-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="04a04-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="04a04-126">Schema Name</span></span>  <br/> |<span data-ttu-id="04a04-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="04a04-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="04a04-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="04a04-128">Validation File</span></span>  <br/> |<span data-ttu-id="04a04-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="04a04-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="04a04-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="04a04-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="04a04-131">False</span><span class="sxs-lookup"><span data-stu-id="04a04-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="04a04-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="04a04-132">See also</span></span>



- [<span data-ttu-id="04a04-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="04a04-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

