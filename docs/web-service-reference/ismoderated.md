---
title: IsModerated
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsModerated
api_type:
- schema
ms.assetid: a7562256-feb9-41a1-857e-b5d41cbed680
description: IsModerated 要素は、受信者のメールボックスがモデレートされているかどうかを示します。
ms.openlocfilehash: 930d5a7e09712f35d22850a93462d051a34785a1
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44435486"
---
# <a name="ismoderated"></a><span data-ttu-id="70cfe-103">IsModerated</span><span class="sxs-lookup"><span data-stu-id="70cfe-103">IsModerated</span></span>

<span data-ttu-id="70cfe-104">**Ismoderated**要素は、受信者のメールボックスがモデレートされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="70cfe-104">The **IsModerated** element indicates whether the recipient's mailbox is being moderated.</span></span> 
  
```XML
<IsModerated>true | false</IsModerated>
```

 <span data-ttu-id="70cfe-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="70cfe-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="70cfe-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="70cfe-106">Attributes and elements</span></span>

<span data-ttu-id="70cfe-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="70cfe-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="70cfe-108">属性</span><span class="sxs-lookup"><span data-stu-id="70cfe-108">Attributes</span></span>

<span data-ttu-id="70cfe-109">なし。</span><span class="sxs-lookup"><span data-stu-id="70cfe-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="70cfe-110">子要素</span><span class="sxs-lookup"><span data-stu-id="70cfe-110">Child elements</span></span>

<span data-ttu-id="70cfe-111">なし。</span><span class="sxs-lookup"><span data-stu-id="70cfe-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="70cfe-112">親要素</span><span class="sxs-lookup"><span data-stu-id="70cfe-112">Parent elements</span></span>

|<span data-ttu-id="70cfe-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="70cfe-113">**Element**</span></span>|<span data-ttu-id="70cfe-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="70cfe-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="70cfe-115">メールヒント</span><span class="sxs-lookup"><span data-stu-id="70cfe-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="70cfe-116">さまざまな種類のメールヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="70cfe-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="70cfe-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="70cfe-117">Text value</span></span>

<span data-ttu-id="70cfe-118">この要素のテキスト値は、受信者のメールボックスがモデレートされている場合は**true**です。</span><span class="sxs-lookup"><span data-stu-id="70cfe-118">The text value for this element is **true** if the recipient's mailbox is being moderated.</span></span> <span data-ttu-id="70cfe-119">受信者のメールボックスがモデレートされていない場合、値は**false**になります。</span><span class="sxs-lookup"><span data-stu-id="70cfe-119">The value is **false** if the recipient's mailbox is not being moderated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="70cfe-120">注釈</span><span class="sxs-lookup"><span data-stu-id="70cfe-120">Remarks</span></span>

<span data-ttu-id="70cfe-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="70cfe-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="70cfe-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="70cfe-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="70cfe-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="70cfe-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="70cfe-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="70cfe-124">Schema Name</span></span>  <br/> |<span data-ttu-id="70cfe-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="70cfe-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="70cfe-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="70cfe-126">Validation File</span></span>  <br/> |<span data-ttu-id="70cfe-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="70cfe-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="70cfe-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="70cfe-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="70cfe-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="70cfe-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="70cfe-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="70cfe-130">See also</span></span>



- [<span data-ttu-id="70cfe-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="70cfe-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

