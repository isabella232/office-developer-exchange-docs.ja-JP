---
title: OptedInto
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 083a23d9-acc3-4c15-9d30-c20bf7e6808d
description: OptedInto 要素は、ユーザーがアイテム保持ポリシーをオプトインしているかどうかを示すブール値を指定します。
ms.openlocfilehash: 1095a8c2527546b8c945dd7efb5c0218f9a151c8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468769"
---
# <a name="optedinto"></a><span data-ttu-id="d89ad-103">OptedInto</span><span class="sxs-lookup"><span data-stu-id="d89ad-103">OptedInto</span></span>

<span data-ttu-id="d89ad-104">**Optedinto**要素は、ユーザーがアイテム保持ポリシーをオプトインしているかどうかを示すブール値を指定します。</span><span class="sxs-lookup"><span data-stu-id="d89ad-104">The **OptedInto** element specifies a Boolean value that indicates whether the user opted in to the retention policy.</span></span> 
  
```XML
<OptedInto>true | false</OptedInto>
```

 <span data-ttu-id="d89ad-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="d89ad-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d89ad-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d89ad-106">Attributes and elements</span></span>

<span data-ttu-id="d89ad-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d89ad-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d89ad-108">属性</span><span class="sxs-lookup"><span data-stu-id="d89ad-108">Attributes</span></span>

<span data-ttu-id="d89ad-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d89ad-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d89ad-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d89ad-110">Child elements</span></span>

<span data-ttu-id="d89ad-111">なし。</span><span class="sxs-lookup"><span data-stu-id="d89ad-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="d89ad-112">親要素</span><span class="sxs-lookup"><span data-stu-id="d89ad-112">Parent elements</span></span>

[<span data-ttu-id="d89ad-113">New-retentionpolicytag</span><span class="sxs-lookup"><span data-stu-id="d89ad-113">RetentionPolicyTag</span></span>](retentionpolicytag.md)
  
## <a name="text-value"></a><span data-ttu-id="d89ad-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d89ad-114">Text value</span></span>

<span data-ttu-id="d89ad-115">**Optedinto**要素のテキスト値が**true**である場合は、ユーザーがアイテム保持ポリシーをオプトインしていることを示します。</span><span class="sxs-lookup"><span data-stu-id="d89ad-115">A text value of **true** for the **OptedInto** element indicates that the user opted in to the retention policy.</span></span> <span data-ttu-id="d89ad-116">値が**false**の場合は、ユーザーがアイテム保持ポリシーをオプトインしていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="d89ad-116">A value of **false** indicates that the user did not opt into the retention policy.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="d89ad-117">注釈</span><span class="sxs-lookup"><span data-stu-id="d89ad-117">Remarks</span></span>

<span data-ttu-id="d89ad-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d89ad-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d89ad-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d89ad-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d89ad-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d89ad-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d89ad-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="d89ad-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="d89ad-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d89ad-122">Schema name</span></span>  <br/> |<span data-ttu-id="d89ad-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="d89ad-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="d89ad-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d89ad-124">Validation file</span></span>  <br/> |<span data-ttu-id="d89ad-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="d89ad-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="d89ad-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d89ad-126">Can be empty</span></span>  <br/> ||
   

