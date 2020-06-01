---
title: PrintAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7232505a-bab0-4d78-87bc-6cc4b568937a
description: PrintAllowed 要素は、印刷を有効にするかどうかを指定します。
ms.openlocfilehash: ac38491d563916160b4d00165b743c51cb29fe00
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468748"
---
# <a name="printallowed"></a><span data-ttu-id="d68ab-103">PrintAllowed</span><span class="sxs-lookup"><span data-stu-id="d68ab-103">PrintAllowed</span></span>

<span data-ttu-id="d68ab-104">**Printallowed**要素は、印刷を有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="d68ab-104">The **PrintAllowed** element specifies whether printing is enabled.</span></span> 
  
```XML
<PrintAllowed> true | false </PrintAllowed>
```

 <span data-ttu-id="d68ab-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d68ab-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d68ab-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d68ab-106">Attributes and elements</span></span>

<span data-ttu-id="d68ab-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d68ab-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d68ab-108">属性</span><span class="sxs-lookup"><span data-stu-id="d68ab-108">Attributes</span></span>

<span data-ttu-id="d68ab-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d68ab-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d68ab-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d68ab-110">Child elements</span></span>

<span data-ttu-id="d68ab-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d68ab-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d68ab-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d68ab-112">Parent elements</span></span>

[<span data-ttu-id="d68ab-113">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="d68ab-113">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a><span data-ttu-id="d68ab-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d68ab-114">Text value</span></span>

<span data-ttu-id="d68ab-115">**Printallowed**要素のテキスト値が**true の場合**は、そのコンテンツを印刷する権限が管理されているアイテムであることを示します。</span><span class="sxs-lookup"><span data-stu-id="d68ab-115">A text value of **true** for the **PrintAllowed** element indicates that printing the contents is allowed for a rights managed item.</span></span> <span data-ttu-id="d68ab-116">値が**false**の場合、印刷が許可されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="d68ab-116">A value of **false** indicates that printing is not allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d68ab-117">注釈</span><span class="sxs-lookup"><span data-stu-id="d68ab-117">Remarks</span></span>

<span data-ttu-id="d68ab-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d68ab-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d68ab-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d68ab-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d68ab-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d68ab-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d68ab-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="d68ab-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d68ab-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d68ab-122">Schema name</span></span>  <br/> |<span data-ttu-id="d68ab-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d68ab-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="d68ab-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d68ab-124">Validation file</span></span>  <br/> |<span data-ttu-id="d68ab-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d68ab-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d68ab-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d68ab-126">Can be empty</span></span>  <br/> ||
   

