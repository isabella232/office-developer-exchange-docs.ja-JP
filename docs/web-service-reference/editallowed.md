---
title: EditAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e63c4f7e-77c0-4826-b4e2-43b795d03914
description: EditAllowed 要素は、Information Rights Management を編集できるかどうかを指定します。
ms.openlocfilehash: 979fbaa9fcfbd1015468a8ae00628959bad0bf56
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463483"
---
# <a name="editallowed"></a><span data-ttu-id="996b3-103">EditAllowed</span><span class="sxs-lookup"><span data-stu-id="996b3-103">EditAllowed</span></span>

<span data-ttu-id="996b3-104">**Editallowed**要素は、Information Rights Management を編集できるかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="996b3-104">The **EditAllowed** element specifies whether Information Rights Management can be edited.</span></span> 
  
```XML
<EditAllowed> true | false </EditAllowed>
```

 <span data-ttu-id="996b3-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="996b3-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="996b3-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="996b3-106">Attributes and elements</span></span>

<span data-ttu-id="996b3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="996b3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="996b3-108">属性</span><span class="sxs-lookup"><span data-stu-id="996b3-108">Attributes</span></span>

<span data-ttu-id="996b3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="996b3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="996b3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="996b3-110">Child elements</span></span>

<span data-ttu-id="996b3-111">なし。</span><span class="sxs-lookup"><span data-stu-id="996b3-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="996b3-112">親要素</span><span class="sxs-lookup"><span data-stu-id="996b3-112">Parent elements</span></span>

|<span data-ttu-id="996b3-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="996b3-113">**Element**</span></span>|<span data-ttu-id="996b3-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="996b3-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="996b3-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="996b3-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="996b3-116">Rights management のライセンスに関する情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="996b3-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="996b3-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="996b3-117">Text value</span></span>

<span data-ttu-id="996b3-118">**Editallowed**要素のテキスト値が**true の場合**、INFORMATION Rights Management (IRM) が編集可能であることを示します。</span><span class="sxs-lookup"><span data-stu-id="996b3-118">A text value of **true** for the **EditAllowed** element indicates that Information Rights Management (IRM) can be edited.</span></span> <span data-ttu-id="996b3-119">値が**false**の場合は、IRM を編集できないことを示します。</span><span class="sxs-lookup"><span data-stu-id="996b3-119">A value of **false** indicates that IRM cannot be edited.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="996b3-120">注釈</span><span class="sxs-lookup"><span data-stu-id="996b3-120">Remarks</span></span>

<span data-ttu-id="996b3-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="996b3-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="996b3-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="996b3-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="996b3-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="996b3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="996b3-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="996b3-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="996b3-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="996b3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="996b3-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="996b3-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="996b3-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="996b3-127">Validation File</span></span>  <br/> |<span data-ttu-id="996b3-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="996b3-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="996b3-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="996b3-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="996b3-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="996b3-130">See also</span></span>



- [<span data-ttu-id="996b3-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="996b3-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

