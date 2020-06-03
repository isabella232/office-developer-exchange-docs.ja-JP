---
title: ForwardAllowed
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: bc32e0f4-61e9-4c9f-9a03-90a07eb51c53
description: ForwardAllowed 要素は、転送メールを有効にするかどうかを指定します。
ms.openlocfilehash: 3c722809bf68239c7d776108cb60d98afbed6e93
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461934"
---
# <a name="forwardallowed"></a><span data-ttu-id="e4eb8-103">ForwardAllowed</span><span class="sxs-lookup"><span data-stu-id="e4eb8-103">ForwardAllowed</span></span>

<span data-ttu-id="e4eb8-104">**Forwardallowed**要素は、転送メールを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="e4eb8-104">The **ForwardAllowed** element specifies whether forwarding emails is enabled.</span></span> 
  
```XML
<ForwardAllowed>true | false</ForwardAllowed>
```

 <span data-ttu-id="e4eb8-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e4eb8-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e4eb8-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e4eb8-106">Attributes and elements</span></span>

<span data-ttu-id="e4eb8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e4eb8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4eb8-108">属性</span><span class="sxs-lookup"><span data-stu-id="e4eb8-108">Attributes</span></span>

<span data-ttu-id="e4eb8-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e4eb8-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e4eb8-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e4eb8-110">Child elements</span></span>

<span data-ttu-id="e4eb8-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e4eb8-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e4eb8-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e4eb8-112">Parent elements</span></span>

|<span data-ttu-id="e4eb8-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e4eb8-113">**Element**</span></span>|<span data-ttu-id="e4eb8-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e4eb8-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e4eb8-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="e4eb8-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="e4eb8-116">Rights management のライセンスに関する情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="e4eb8-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e4eb8-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e4eb8-117">Text value</span></span>

<span data-ttu-id="e4eb8-118">**Forwardallowed**要素のテキスト値が**true**の場合は、メール転送が許可されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="e4eb8-118">A text value of **true** for the **ForwardAllowed** element indicates that forwarding emails is allowed.</span></span> <span data-ttu-id="e4eb8-119">値が**false**の場合、転送が許可されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="e4eb8-119">A value of **false** indicates that forwarding is not allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e4eb8-120">注釈</span><span class="sxs-lookup"><span data-stu-id="e4eb8-120">Remarks</span></span>

<span data-ttu-id="e4eb8-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e4eb8-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="e4eb8-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e4eb8-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e4eb8-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e4eb8-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e4eb8-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="e4eb8-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e4eb8-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e4eb8-125">Schema Name</span></span>  <br/> |<span data-ttu-id="e4eb8-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="e4eb8-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="e4eb8-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e4eb8-127">Validation File</span></span>  <br/> |<span data-ttu-id="e4eb8-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e4eb8-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="e4eb8-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="e4eb8-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="e4eb8-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="e4eb8-130">See also</span></span>



- [<span data-ttu-id="e4eb8-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e4eb8-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

