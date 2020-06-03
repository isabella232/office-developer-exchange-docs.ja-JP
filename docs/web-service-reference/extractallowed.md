---
title: ExtractAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bc213f0e-a655-44e9-9ac9-bc1673bae1fe
description: ExtractAllowed 要素は、エンティティ抽出が有効であるかどうかを指定します。
ms.openlocfilehash: f9fcae72d6241e51f549fbf650f5b2aebe019e46
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461983"
---
# <a name="extractallowed"></a><span data-ttu-id="55dff-103">ExtractAllowed</span><span class="sxs-lookup"><span data-stu-id="55dff-103">ExtractAllowed</span></span>

<span data-ttu-id="55dff-104">**ExtractAllowed**要素は、エンティティ抽出が有効であるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="55dff-104">The **ExtractAllowed** element specifies whether entity extraction is enabled.</span></span> 
  
```XML
<ExtractAllowed>true | false</ExtractAllowed
```

 <span data-ttu-id="55dff-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="55dff-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55dff-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="55dff-106">Attributes and elements</span></span>

<span data-ttu-id="55dff-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="55dff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55dff-108">属性</span><span class="sxs-lookup"><span data-stu-id="55dff-108">Attributes</span></span>

<span data-ttu-id="55dff-109">なし。</span><span class="sxs-lookup"><span data-stu-id="55dff-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55dff-110">子要素</span><span class="sxs-lookup"><span data-stu-id="55dff-110">Child elements</span></span>

<span data-ttu-id="55dff-111">なし。</span><span class="sxs-lookup"><span data-stu-id="55dff-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="55dff-112">親要素</span><span class="sxs-lookup"><span data-stu-id="55dff-112">Parent elements</span></span>

|<span data-ttu-id="55dff-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="55dff-113">**Element**</span></span>|<span data-ttu-id="55dff-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="55dff-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55dff-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="55dff-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="55dff-116">Rights management のライセンスに関する情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="55dff-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="55dff-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="55dff-117">Text value</span></span>

<span data-ttu-id="55dff-118">**ExtractAllowed**要素のテキスト値が**true**である場合、エンティティ抽出が有効になっていることを示します。</span><span class="sxs-lookup"><span data-stu-id="55dff-118">A text value of **true** for the **ExtractAllowed** element indicates that entity extraction is enabled.</span></span> <span data-ttu-id="55dff-119">値が**false**の場合、エンティティの抽出が有効になっていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="55dff-119">A value of **false** indicates that entity extraction is not enabled.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="55dff-120">注釈</span><span class="sxs-lookup"><span data-stu-id="55dff-120">Remarks</span></span>

<span data-ttu-id="55dff-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="55dff-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="55dff-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="55dff-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55dff-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="55dff-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55dff-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="55dff-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="55dff-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="55dff-125">Schema Name</span></span>  <br/> |<span data-ttu-id="55dff-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="55dff-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="55dff-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="55dff-127">Validation File</span></span>  <br/> |<span data-ttu-id="55dff-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="55dff-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="55dff-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="55dff-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="55dff-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="55dff-130">See also</span></span>



- [<span data-ttu-id="55dff-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="55dff-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

