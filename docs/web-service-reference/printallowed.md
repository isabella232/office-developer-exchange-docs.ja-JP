---
title: PrintAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 7232505a-bab0-4d78-87bc-6cc4b568937a
description: PrintAllowed 要素は、印刷が有効になっているかどうかを指定します。
ms.openlocfilehash: 85c18f3a6bd8f1705d0e21b99bae15484348f777
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832880"
---
# <a name="printallowed"></a><span data-ttu-id="9d7fa-103">PrintAllowed</span><span class="sxs-lookup"><span data-stu-id="9d7fa-103">PrintAllowed</span></span>

<span data-ttu-id="9d7fa-104">**PrintAllowed**要素は、印刷が有効になっているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="9d7fa-104">The **PrintAllowed** element specifies whether printing is enabled.</span></span> 
  
```XML
<PrintAllowed> true | false </PrintAllowed>
```

 <span data-ttu-id="9d7fa-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="9d7fa-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9d7fa-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9d7fa-106">Attributes and elements</span></span>

<span data-ttu-id="9d7fa-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9d7fa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9d7fa-108">属性</span><span class="sxs-lookup"><span data-stu-id="9d7fa-108">Attributes</span></span>

<span data-ttu-id="9d7fa-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9d7fa-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9d7fa-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9d7fa-110">Child elements</span></span>

<span data-ttu-id="9d7fa-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9d7fa-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9d7fa-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9d7fa-112">Parent elements</span></span>

[<span data-ttu-id="9d7fa-113">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="9d7fa-113">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a><span data-ttu-id="9d7fa-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9d7fa-114">Text value</span></span>

<span data-ttu-id="9d7fa-115">の**場合は true** 、 **PrintAllowed**要素のテキスト値は、権限管理の対象項目の内容の印刷を許可することを示します。</span><span class="sxs-lookup"><span data-stu-id="9d7fa-115">A text value of **true** for the **PrintAllowed** element indicates that printing the contents is allowed for a rights managed item.</span></span> <span data-ttu-id="9d7fa-116">**False**の値は、印刷が許可されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="9d7fa-116">A value of **false** indicates that printing is not allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="9d7fa-117">備考</span><span class="sxs-lookup"><span data-stu-id="9d7fa-117">Remarks</span></span>

<span data-ttu-id="9d7fa-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9d7fa-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="9d7fa-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9d7fa-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9d7fa-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="9d7fa-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9d7fa-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="9d7fa-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9d7fa-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9d7fa-122">Schema name</span></span>  <br/> |<span data-ttu-id="9d7fa-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9d7fa-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="9d7fa-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9d7fa-124">Validation file</span></span>  <br/> |<span data-ttu-id="9d7fa-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9d7fa-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9d7fa-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9d7fa-126">Can be empty</span></span>  <br/> ||
   

