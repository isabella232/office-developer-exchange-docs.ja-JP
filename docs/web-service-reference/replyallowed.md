---
title: ReplyAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 880af57e-0fa1-473c-b87c-f02f1133ba5e
description: ReplyAllowed 要素は、応答を許可するか権限の管理対象のデータを指定します。
ms.openlocfilehash: c774836ac6e72648d6a6c017d41fcafdb64d116c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833107"
---
# <a name="replyallowed"></a><span data-ttu-id="71974-103">ReplyAllowed</span><span class="sxs-lookup"><span data-stu-id="71974-103">ReplyAllowed</span></span>

<span data-ttu-id="71974-104">**ReplyAllowed**要素は、応答を許可するか権限の管理対象のデータを指定します。</span><span class="sxs-lookup"><span data-stu-id="71974-104">The **ReplyAllowed** element specifies whether a reply is allowed for rights managed data.</span></span> 
  
```XML
<ReplyAllowed> true | false </ReplyAllowed>
```

 <span data-ttu-id="71974-105">**ブール型 (Boolean)**</span><span class="sxs-lookup"><span data-stu-id="71974-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="71974-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="71974-106">Attributes and elements</span></span>

<span data-ttu-id="71974-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="71974-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="71974-108">属性</span><span class="sxs-lookup"><span data-stu-id="71974-108">Attributes</span></span>

<span data-ttu-id="71974-109">なし。</span><span class="sxs-lookup"><span data-stu-id="71974-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="71974-110">子要素</span><span class="sxs-lookup"><span data-stu-id="71974-110">Child elements</span></span>

<span data-ttu-id="71974-111">なし。</span><span class="sxs-lookup"><span data-stu-id="71974-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="71974-112">親要素</span><span class="sxs-lookup"><span data-stu-id="71974-112">Parent elements</span></span>

[<span data-ttu-id="71974-113">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="71974-113">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a><span data-ttu-id="71974-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="71974-114">Text value</span></span>

<span data-ttu-id="71974-115">の**場合は true** 、 **ReplyAllowed**要素のテキスト値は、返信を許可する権限の管理対象のデータを示します。</span><span class="sxs-lookup"><span data-stu-id="71974-115">A text value of **true** for the **ReplyAllowed** element indicates that replies are allowed for the rights managed data.</span></span> <span data-ttu-id="71974-116">**False**の値は、返信が許可されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="71974-116">A value of **false** indicates that replies are not allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="71974-117">備考</span><span class="sxs-lookup"><span data-stu-id="71974-117">Remarks</span></span>

<span data-ttu-id="71974-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="71974-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="71974-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="71974-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="71974-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="71974-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="71974-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="71974-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="71974-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="71974-122">Schema name</span></span>  <br/> |<span data-ttu-id="71974-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="71974-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="71974-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="71974-124">Validation file</span></span>  <br/> |<span data-ttu-id="71974-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="71974-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="71974-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="71974-126">Can be empty</span></span>  <br/> ||
   

