---
title: OptedInto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 083a23d9-acc3-4c15-9d30-c20bf7e6808d
description: OptedInto 要素は、リテンション ・ ポリシーをユーザーが有効にするかどうかを示すブール値を指定します。
ms.openlocfilehash: 0d8fb2b07c6c98ba6973ab6efabe9c35d2d1ac12
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832657"
---
# <a name="optedinto"></a><span data-ttu-id="e2324-103">OptedInto</span><span class="sxs-lookup"><span data-stu-id="e2324-103">OptedInto</span></span>

<span data-ttu-id="e2324-104">**OptedInto**要素は、リテンション ・ ポリシーをユーザーが有効にするかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="e2324-104">The **OptedInto** element specifies a Boolean value that indicates whether the user opted in to the retention policy.</span></span> 
  
```XML
<OptedInto>true | false</OptedInto>
```

 <span data-ttu-id="e2324-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="e2324-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e2324-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e2324-106">Attributes and elements</span></span>

<span data-ttu-id="e2324-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e2324-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2324-108">属性</span><span class="sxs-lookup"><span data-stu-id="e2324-108">Attributes</span></span>

<span data-ttu-id="e2324-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e2324-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e2324-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e2324-110">Child elements</span></span>

<span data-ttu-id="e2324-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e2324-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e2324-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e2324-112">Parent elements</span></span>

[<span data-ttu-id="e2324-113">RetentionPolicyTag</span><span class="sxs-lookup"><span data-stu-id="e2324-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="e2324-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e2324-114">Text value</span></span>

<span data-ttu-id="e2324-115">の**場合は true** 、 **OptedInto**要素のテキスト値は、保持ポリシーにユーザーが有効にことを示します。</span><span class="sxs-lookup"><span data-stu-id="e2324-115">A text value of **true** for the **OptedInto** element indicates that the user opted in to the retention policy.</span></span> <span data-ttu-id="e2324-116">**False**の値は、リテンション ・ ポリシーに、ユーザーを選択しなかったことを示します。</span><span class="sxs-lookup"><span data-stu-id="e2324-116">A value of **false** indicates that the user did not opt into the retention policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e2324-117">備考</span><span class="sxs-lookup"><span data-stu-id="e2324-117">Remarks</span></span>

<span data-ttu-id="e2324-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e2324-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e2324-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e2324-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2324-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="e2324-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2324-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="e2324-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e2324-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e2324-122">Schema name</span></span>  <br/> |<span data-ttu-id="e2324-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="e2324-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="e2324-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e2324-124">Validation file</span></span>  <br/> |<span data-ttu-id="e2324-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="e2324-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e2324-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e2324-126">Can be empty</span></span>  <br/> ||
   

