---
title: Modify受信者の許可
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3f25e673-0df0-4285-bf03-a083a395cdab
description: Modify受信者 Sallowed 要素は、受信者の変更を有効にするかどうかを指定します。
ms.openlocfilehash: 3154ec3aceb2da7911002d505e0c452bf920d71f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44465696"
---
# <a name="modifyrecipientsallowed"></a><span data-ttu-id="fb145-103">Modify受信者の許可</span><span class="sxs-lookup"><span data-stu-id="fb145-103">ModifyRecipientsAllowed</span></span>

<span data-ttu-id="fb145-104">**Modify受信者 Sallowed**要素は、受信者の変更を有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="fb145-104">The **ModifyRecipientsAllowed** element specifies whether modification of the recipients is enabled.</span></span> 
  
```XML
<ModifyRecipientsAllowed> true | false </ModifyRecipientsAllowed>
```

 <span data-ttu-id="fb145-105">**boolean**</span><span class="sxs-lookup"><span data-stu-id="fb145-105">**boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fb145-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="fb145-106">Attributes and elements</span></span>

<span data-ttu-id="fb145-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fb145-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fb145-108">属性</span><span class="sxs-lookup"><span data-stu-id="fb145-108">Attributes</span></span>

<span data-ttu-id="fb145-109">なし。</span><span class="sxs-lookup"><span data-stu-id="fb145-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="fb145-110">子要素</span><span class="sxs-lookup"><span data-stu-id="fb145-110">Child elements</span></span>

<span data-ttu-id="fb145-111">なし。</span><span class="sxs-lookup"><span data-stu-id="fb145-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="fb145-112">親要素</span><span class="sxs-lookup"><span data-stu-id="fb145-112">Parent elements</span></span>

[<span data-ttu-id="fb145-113">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="fb145-113">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md)
  
## <a name="text-value"></a><span data-ttu-id="fb145-114">テキスト値</span><span class="sxs-lookup"><span data-stu-id="fb145-114">Text value</span></span>

<span data-ttu-id="fb145-115">**Modifyrecipient Sallowed**要素のテキスト値が**true**になっている場合は、そのアイテムで権限管理が有効になっているアイテムに対してアイテム受信者リストが変更可能であることを示します。</span><span class="sxs-lookup"><span data-stu-id="fb145-115">A text value of **true** for the **ModifyRecipientsAllowed** element indicates that the item recipient list is modifiable for an item with rights management enabled on it.</span></span> <span data-ttu-id="fb145-116">値が**false**の場合、受信者の一覧は変更できないことを示します。</span><span class="sxs-lookup"><span data-stu-id="fb145-116">A value of **false** indicates that the recipient list is not modifiable.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="fb145-117">注釈</span><span class="sxs-lookup"><span data-stu-id="fb145-117">Remarks</span></span>

<span data-ttu-id="fb145-118">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fb145-118">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fb145-119">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fb145-119">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fb145-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="fb145-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fb145-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="fb145-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="fb145-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fb145-122">Schema name</span></span>  <br/> |<span data-ttu-id="fb145-123">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="fb145-123">Types schema</span></span>  <br/> |
|<span data-ttu-id="fb145-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fb145-124">Validation file</span></span>  <br/> |<span data-ttu-id="fb145-125">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="fb145-125">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="fb145-126">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fb145-126">Can be empty</span></span>  <br/> ||
   

