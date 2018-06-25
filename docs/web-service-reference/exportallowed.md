---
title: ExportAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dcff5ccc-31dc-4941-9f71-d6519133aebb
description: ExportAllowed 要素は、エクスポートが有効になっているかどうかを指定します。
ms.openlocfilehash: 5c07941e0a79394bbdaa1a1f62b20adedfe7a9bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760378"
---
# <a name="exportallowed"></a><span data-ttu-id="6b691-103">ExportAllowed</span><span class="sxs-lookup"><span data-stu-id="6b691-103">ExportAllowed</span></span>

<span data-ttu-id="6b691-104">**ExportAllowed**要素は、エクスポートが有効になっているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="6b691-104">The **ExportAllowed** element specifies whether exporting is enabled.</span></span> 
  
```XML
<ExportAllowed>true | false</ExportAllowed>
```

 <span data-ttu-id="6b691-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="6b691-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6b691-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6b691-106">Attributes and elements</span></span>

<span data-ttu-id="6b691-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6b691-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6b691-108">属性</span><span class="sxs-lookup"><span data-stu-id="6b691-108">Attributes</span></span>

<span data-ttu-id="6b691-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6b691-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6b691-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6b691-110">Child elements</span></span>

<span data-ttu-id="6b691-111">なし。</span><span class="sxs-lookup"><span data-stu-id="6b691-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="6b691-112">親要素</span><span class="sxs-lookup"><span data-stu-id="6b691-112">Parent elements</span></span>

|<span data-ttu-id="6b691-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="6b691-113">**Element**</span></span>|<span data-ttu-id="6b691-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="6b691-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6b691-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="6b691-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="6b691-116">権限管理のライセンスについての情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="6b691-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6b691-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6b691-117">Text value</span></span>

<span data-ttu-id="6b691-118">の**場合は true** 、 **ExportAllowed**要素のテキスト値は、エクスポートを許可することを示します。</span><span class="sxs-lookup"><span data-stu-id="6b691-118">A text value of **true** for the **ExportAllowed** element indicates that exporting is allowed.</span></span> <span data-ttu-id="6b691-119">**False**の値は、エクスポートすることは許可されていませんを示します。</span><span class="sxs-lookup"><span data-stu-id="6b691-119">A value of **false** indicates that exporting is not allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="6b691-120">備考</span><span class="sxs-lookup"><span data-stu-id="6b691-120">Remarks</span></span>

<span data-ttu-id="6b691-121">この要素はオプションです。</span><span class="sxs-lookup"><span data-stu-id="6b691-121">This element is optional.</span></span>
  
<span data-ttu-id="6b691-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="6b691-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="6b691-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6b691-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6b691-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="6b691-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6b691-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="6b691-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="6b691-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6b691-126">Schema Name</span></span>  <br/> |<span data-ttu-id="6b691-127">型のスキーマ</span><span class="sxs-lookup"><span data-stu-id="6b691-127">Type schema</span></span>  <br/> |
|<span data-ttu-id="6b691-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6b691-128">Validation File</span></span>  <br/> |<span data-ttu-id="6b691-129">types.xsd</span><span class="sxs-lookup"><span data-stu-id="6b691-129">types.xsd</span></span>  <br/> |
|<span data-ttu-id="6b691-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="6b691-130">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="6b691-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="6b691-131">See also</span></span>



- [<span data-ttu-id="6b691-132">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6b691-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

