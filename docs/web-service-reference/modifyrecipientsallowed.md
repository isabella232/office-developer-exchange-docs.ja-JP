---
title: ModifyRecipientsAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f25e673-0df0-4285-bf03-a083a395cdab
description: ModifyRecipientsAllowed 要素は、受信者の変更が有効になっているかどうかを指定します。
ms.openlocfilehash: 2b07c7fa8e6b5872621c8b019b60584abbf98e3c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832473"
---
# <a name="modifyrecipientsallowed"></a><span data-ttu-id="59910-103">ModifyRecipientsAllowed</span><span class="sxs-lookup"><span data-stu-id="59910-103">ModifyRecipientsAllowed</span></span>

<span data-ttu-id="59910-104">**ModifyRecipientsAllowed**要素は、受信者の変更が有効になっているかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="59910-104">The **ModifyRecipientsAllowed** element specifies whether modification of the recipients is enabled.</span></span> 
  
```XML
<ModifyRecipientsAllowed> true | false </ModifyRecipientsAllowed>
```

 <span data-ttu-id="59910-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="59910-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59910-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="59910-106">Attributes and elements</span></span>

<span data-ttu-id="59910-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="59910-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59910-108">属性</span><span class="sxs-lookup"><span data-stu-id="59910-108">Attributes</span></span>

<span data-ttu-id="59910-109">なし。</span><span class="sxs-lookup"><span data-stu-id="59910-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="59910-110">子要素</span><span class="sxs-lookup"><span data-stu-id="59910-110">Child elements</span></span>

<span data-ttu-id="59910-111">なし。</span><span class="sxs-lookup"><span data-stu-id="59910-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="59910-112">親要素</span><span class="sxs-lookup"><span data-stu-id="59910-112">Parent elements</span></span>

[<span data-ttu-id="59910-113">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="59910-113">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a><span data-ttu-id="59910-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="59910-114">Text value</span></span>

<span data-ttu-id="59910-115">の**場合は true** 、 **ModifyRecipientsAllowed**要素のテキスト値は、項目の受信者リストが権限管理を有効にするとアイテムを変更できることを示します。</span><span class="sxs-lookup"><span data-stu-id="59910-115">A text value of **true** for the **ModifyRecipientsAllowed** element indicates that the item recipient list is modifiable for an item with rights management enabled on it.</span></span> <span data-ttu-id="59910-116">**False**の値は、受信者の一覧が変更可能ではないことを示します。</span><span class="sxs-lookup"><span data-stu-id="59910-116">A value of **false** indicates that the recipient list is not modifiable.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="59910-117">備考</span><span class="sxs-lookup"><span data-stu-id="59910-117">Remarks</span></span>

<span data-ttu-id="59910-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="59910-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="59910-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="59910-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59910-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="59910-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59910-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="59910-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="59910-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="59910-122">Schema name</span></span>  <br/> |<span data-ttu-id="59910-123">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="59910-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="59910-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="59910-124">Validation file</span></span>  <br/> |<span data-ttu-id="59910-125">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="59910-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="59910-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="59910-126">Can be empty</span></span>  <br/> ||
   

