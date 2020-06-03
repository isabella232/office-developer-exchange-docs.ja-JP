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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44435486"
---
# <a name="ismoderated"></a><span data-ttu-id="57162-103">IsModerated</span><span class="sxs-lookup"><span data-stu-id="57162-103">IsModerated</span></span>

<span data-ttu-id="57162-104">**Ismoderated**要素は、受信者のメールボックスがモデレートされているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="57162-104">The **IsModerated** element indicates whether the recipient's mailbox is being moderated.</span></span> 
  
```XML
<IsModerated>true | false</IsModerated>
```

 <span data-ttu-id="57162-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="57162-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57162-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="57162-106">Attributes and elements</span></span>

<span data-ttu-id="57162-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="57162-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57162-108">属性</span><span class="sxs-lookup"><span data-stu-id="57162-108">Attributes</span></span>

<span data-ttu-id="57162-109">なし。</span><span class="sxs-lookup"><span data-stu-id="57162-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="57162-110">子要素</span><span class="sxs-lookup"><span data-stu-id="57162-110">Child elements</span></span>

<span data-ttu-id="57162-111">なし。</span><span class="sxs-lookup"><span data-stu-id="57162-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="57162-112">親要素</span><span class="sxs-lookup"><span data-stu-id="57162-112">Parent elements</span></span>

|<span data-ttu-id="57162-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="57162-113">**Element**</span></span>|<span data-ttu-id="57162-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="57162-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57162-115">メールヒント</span><span class="sxs-lookup"><span data-stu-id="57162-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="57162-116">さまざまな種類のメールヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="57162-116">Represents values for various types of mail tips.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="57162-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="57162-117">Text value</span></span>

<span data-ttu-id="57162-118">この要素のテキスト値は、受信者のメールボックスがモデレートされている場合は**true**です。</span><span class="sxs-lookup"><span data-stu-id="57162-118">The text value for this element is **true** if the recipient's mailbox is being moderated.</span></span> <span data-ttu-id="57162-119">受信者のメールボックスがモデレートされていない場合、値は**false**になります。</span><span class="sxs-lookup"><span data-stu-id="57162-119">The value is **false** if the recipient's mailbox is not being moderated.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="57162-120">注釈</span><span class="sxs-lookup"><span data-stu-id="57162-120">Remarks</span></span>

<span data-ttu-id="57162-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="57162-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57162-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="57162-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57162-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="57162-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="57162-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="57162-124">Schema Name</span></span>  <br/> |<span data-ttu-id="57162-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="57162-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="57162-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="57162-126">Validation File</span></span>  <br/> |<span data-ttu-id="57162-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="57162-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="57162-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="57162-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="57162-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="57162-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57162-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="57162-130">See also</span></span>



- [<span data-ttu-id="57162-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="57162-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

