---
title: EditAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e63c4f7e-77c0-4826-b4e2-43b795d03914
description: EditAllowed 要素は、情報権利の管理を編集できるかどうかを指定します。
ms.openlocfilehash: 48c7d751c018bf5702b05b41eeaa7ad350189e3a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760192"
---
# <a name="editallowed"></a><span data-ttu-id="b19ed-103">EditAllowed</span><span class="sxs-lookup"><span data-stu-id="b19ed-103">EditAllowed</span></span>

<span data-ttu-id="b19ed-104">**EditAllowed**要素は、情報権利の管理を編集できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="b19ed-104">The **EditAllowed** element specifies whether Information Rights Management can be edited.</span></span> 
  
```XML
<EditAllowed> true | false </EditAllowed>
```

 <span data-ttu-id="b19ed-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="b19ed-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b19ed-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b19ed-106">Attributes and elements</span></span>

<span data-ttu-id="b19ed-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b19ed-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b19ed-108">属性</span><span class="sxs-lookup"><span data-stu-id="b19ed-108">Attributes</span></span>

<span data-ttu-id="b19ed-109">なし。</span><span class="sxs-lookup"><span data-stu-id="b19ed-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="b19ed-110">子要素</span><span class="sxs-lookup"><span data-stu-id="b19ed-110">Child elements</span></span>

<span data-ttu-id="b19ed-111">なし。</span><span class="sxs-lookup"><span data-stu-id="b19ed-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="b19ed-112">親要素</span><span class="sxs-lookup"><span data-stu-id="b19ed-112">Parent elements</span></span>

|<span data-ttu-id="b19ed-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="b19ed-113">**Element**</span></span>|<span data-ttu-id="b19ed-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="b19ed-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b19ed-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="b19ed-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="b19ed-116">権限管理のライセンスについての情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="b19ed-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="b19ed-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b19ed-117">Text value</span></span>

<span data-ttu-id="b19ed-118">の**場合は true** 、 **EditAllowed**要素のテキスト値は、情報権利管理 (IRM) を編集できることを示します。</span><span class="sxs-lookup"><span data-stu-id="b19ed-118">A text value of **true** for the **EditAllowed** element indicates that Information Rights Management (IRM) can be edited.</span></span> <span data-ttu-id="b19ed-119">**False**の値は、IRM を編集できないことを示します。</span><span class="sxs-lookup"><span data-stu-id="b19ed-119">A value of **false** indicates that IRM cannot be edited.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="b19ed-120">備考</span><span class="sxs-lookup"><span data-stu-id="b19ed-120">Remarks</span></span>

<span data-ttu-id="b19ed-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="b19ed-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="b19ed-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b19ed-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b19ed-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="b19ed-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b19ed-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="b19ed-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="b19ed-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b19ed-125">Schema Name</span></span>  <br/> |<span data-ttu-id="b19ed-126">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="b19ed-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="b19ed-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b19ed-127">Validation File</span></span>  <br/> |<span data-ttu-id="b19ed-128">types.xsd</span><span class="sxs-lookup"><span data-stu-id="b19ed-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="b19ed-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b19ed-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="b19ed-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="b19ed-130">See also</span></span>



- [<span data-ttu-id="b19ed-131">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b19ed-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

