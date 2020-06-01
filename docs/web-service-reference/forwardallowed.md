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
ms.lasthandoff: 05/31/2020
ms.locfileid: "44461934"
---
# <a name="forwardallowed"></a><span data-ttu-id="f9d01-103">ForwardAllowed</span><span class="sxs-lookup"><span data-stu-id="f9d01-103">ForwardAllowed</span></span>

<span data-ttu-id="f9d01-104">**Forwardallowed**要素は、転送メールを有効にするかどうかを指定します。</span><span class="sxs-lookup"><span data-stu-id="f9d01-104">The **ForwardAllowed** element specifies whether forwarding emails is enabled.</span></span> 
  
```XML
<ForwardAllowed>true | false</ForwardAllowed>
```

 <span data-ttu-id="f9d01-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="f9d01-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f9d01-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f9d01-106">Attributes and elements</span></span>

<span data-ttu-id="f9d01-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f9d01-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f9d01-108">属性</span><span class="sxs-lookup"><span data-stu-id="f9d01-108">Attributes</span></span>

<span data-ttu-id="f9d01-109">なし。</span><span class="sxs-lookup"><span data-stu-id="f9d01-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="f9d01-110">子要素</span><span class="sxs-lookup"><span data-stu-id="f9d01-110">Child elements</span></span>

<span data-ttu-id="f9d01-111">なし。</span><span class="sxs-lookup"><span data-stu-id="f9d01-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="f9d01-112">親要素</span><span class="sxs-lookup"><span data-stu-id="f9d01-112">Parent elements</span></span>

|<span data-ttu-id="f9d01-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="f9d01-113">**Element**</span></span>|<span data-ttu-id="f9d01-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="f9d01-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f9d01-115">RightsManagementLicenseData</span><span class="sxs-lookup"><span data-stu-id="f9d01-115">RightsManagementLicenseData</span></span>](rightsmanagementlicensedata.md) <br/> |<span data-ttu-id="f9d01-116">Rights management のライセンスに関する情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="f9d01-116">Specifies information about the rights management license.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="f9d01-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f9d01-117">Text value</span></span>

<span data-ttu-id="f9d01-118">**Forwardallowed**要素のテキスト値が**true**の場合は、メール転送が許可されていることを示します。</span><span class="sxs-lookup"><span data-stu-id="f9d01-118">A text value of **true** for the **ForwardAllowed** element indicates that forwarding emails is allowed.</span></span> <span data-ttu-id="f9d01-119">値が**false**の場合、転送が許可されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="f9d01-119">A value of **false** indicates that forwarding is not allowed.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="f9d01-120">注釈</span><span class="sxs-lookup"><span data-stu-id="f9d01-120">Remarks</span></span>

<span data-ttu-id="f9d01-121">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f9d01-121">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="f9d01-122">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f9d01-122">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f9d01-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f9d01-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f9d01-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="f9d01-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="f9d01-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f9d01-125">Schema Name</span></span>  <br/> |<span data-ttu-id="f9d01-126">型スキーマ</span><span class="sxs-lookup"><span data-stu-id="f9d01-126">Type schema</span></span>  <br/> |
|<span data-ttu-id="f9d01-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f9d01-127">Validation File</span></span>  <br/> |<span data-ttu-id="f9d01-128">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="f9d01-128">types.xsd</span></span>  <br/> |
|<span data-ttu-id="f9d01-129">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="f9d01-129">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="f9d01-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="f9d01-130">See also</span></span>



- [<span data-ttu-id="f9d01-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f9d01-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

