---
title: ReplyAllAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: d22f68cf-b18b-45d0-a9ff-414b7db0e67e
description: ReplyAllAllowed 要素は、権限の許可は、すべての応答でデータを管理するかどうかを指定します。
ms.openlocfilehash: cf814e6f27a734afc51b633bf832126a57d7ca5f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833105"
---
# <a name="replyallallowed"></a><span data-ttu-id="c8061-103">ReplyAllAllowed</span><span class="sxs-lookup"><span data-stu-id="c8061-103">ReplyAllAllowed</span></span>

<span data-ttu-id="c8061-104">**ReplyAllAllowed**要素は、権限の許可は、すべての応答でデータを管理するかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="c8061-104">The **ReplyAllAllowed** element specifies whether a reply all is allowed for rights managed data.</span></span> 
  
```XML
<ReplyAllAllowed> true | false </ReplyAllAllowed>
```

 <span data-ttu-id="c8061-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="c8061-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c8061-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c8061-106">Attributes and elements</span></span>

<span data-ttu-id="c8061-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c8061-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c8061-108">属性</span><span class="sxs-lookup"><span data-stu-id="c8061-108">Attributes</span></span>

<span data-ttu-id="c8061-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c8061-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c8061-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c8061-110">Child elements</span></span>

<span data-ttu-id="c8061-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c8061-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c8061-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c8061-112">Parent elements</span></span>

[<span data-ttu-id="c8061-113">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="c8061-113">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a><span data-ttu-id="c8061-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c8061-114">Text value</span></span>

<span data-ttu-id="c8061-115">の**場合は true** 、 **ReplyAllAllowed**要素のテキスト値は、権限の許可は、すべての応答にデータが管理されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="c8061-115">A text value of **true** for the **ReplyAllAllowed** element indicates that a reply all is allowed for the rights managed data.</span></span> <span data-ttu-id="c8061-116">**False**の値は、すべての返信が許可されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="c8061-116">A value of **false** indicates that a reply all is not allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="c8061-117">備考</span><span class="sxs-lookup"><span data-stu-id="c8061-117">Remarks</span></span>

<span data-ttu-id="c8061-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c8061-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="c8061-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c8061-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c8061-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="c8061-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c8061-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="c8061-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c8061-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c8061-122">Schema name</span></span>  <br/> |<span data-ttu-id="c8061-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="c8061-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="c8061-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c8061-124">Validation file</span></span>  <br/> |<span data-ttu-id="c8061-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="c8061-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c8061-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c8061-126">Can be empty</span></span>  <br/> ||
   

