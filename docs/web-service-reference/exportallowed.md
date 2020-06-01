---
title: ExportAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: dcff5ccc-31dc-4941-9f71-d6519133aebb
description: ExportAllowed 要素は、エクスポートを有効にするかどうかを指定します。
ms.openlocfilehash: f5a9aa3040c45d535ef338010bb37bcedb797ffc
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460632"
---
# <a name="exportallowed"></a><span data-ttu-id="9da1c-103">ExportAllowed</span><span class="sxs-lookup"><span data-stu-id="9da1c-103">ExportAllowed</span></span>

<span data-ttu-id="9da1c-104">**Exportallowed**要素は、エクスポートを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9da1c-104">The **ExportAllowed** element specifies whether exporting is enabled.</span></span> 
  
```XML
<ExportAllowed>true | false</ExportAllowed>
```

 <span data-ttu-id="9da1c-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="9da1c-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9da1c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="9da1c-106">Attributes and elements</span></span>

<span data-ttu-id="9da1c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9da1c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9da1c-108">属性</span><span class="sxs-lookup"><span data-stu-id="9da1c-108">Attributes</span></span>

<span data-ttu-id="9da1c-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9da1c-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9da1c-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9da1c-110">Child elements</span></span>

<span data-ttu-id="9da1c-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9da1c-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9da1c-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9da1c-112">Parent elements</span></span>

|<span data-ttu-id="9da1c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9da1c-113">**Element**</span></span>|<span data-ttu-id="9da1c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9da1c-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9da1c-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="9da1c-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="9da1c-116">Rights management のライセンスに関する情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="9da1c-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9da1c-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9da1c-117">Text value</span></span>

<span data-ttu-id="9da1c-118">**Exportallowed**要素のテキスト値が**true**の場合は、エクスポートが許可されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="9da1c-118">A text value of **true** for the **ExportAllowed** element indicates that exporting is allowed.</span></span> <span data-ttu-id="9da1c-119">値が**false**の場合、エクスポートが許可されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="9da1c-119">A value of **false** indicates that exporting is not allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9da1c-120">注釈</span><span class="sxs-lookup"><span data-stu-id="9da1c-120">Remarks</span></span>

<span data-ttu-id="9da1c-121">この要素は省略できます。</span><span class="sxs-lookup"><span data-stu-id="9da1c-121">This element is optional.</span></span>
  
<span data-ttu-id="9da1c-122">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9da1c-122">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9da1c-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9da1c-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9da1c-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="9da1c-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9da1c-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="9da1c-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9da1c-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9da1c-126">Schema Name</span></span>  <br/> |<span data-ttu-id="9da1c-127">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="9da1c-127">Type schema</span></span>  <br/> |
|<span data-ttu-id="9da1c-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9da1c-128">Validation File</span></span>  <br/> |<span data-ttu-id="9da1c-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="9da1c-129">types.xsd</span></span>  <br/> |
|<span data-ttu-id="9da1c-130">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9da1c-130">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="9da1c-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="9da1c-131">See also</span></span>



- [<span data-ttu-id="9da1c-132">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="9da1c-132">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

