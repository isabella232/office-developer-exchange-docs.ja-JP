---
title: Mailヒント有効
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsEnabled
api_type:
- schema
ms.assetid: 737388b3-7b73-42af-94d3-3dbb0659718f
description: Mailヒント Enabled 要素は、メールヒントサービスが利用可能かどうかを示します。
ms.openlocfilehash: 6be923733f1cbd584010ce5f8ee5b96178d5c2c0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468013"
---
# <a name="mailtipsenabled"></a><span data-ttu-id="e8cb1-103">Mailヒント有効</span><span class="sxs-lookup"><span data-stu-id="e8cb1-103">MailTipsEnabled</span></span>

<span data-ttu-id="e8cb1-104">**Mailヒント enabled**要素は、メールヒントサービスが利用可能かどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="e8cb1-104">The **MailTipsEnabled** element indicates whether the mail tips service is available.</span></span> 
  
```xml
<MailTipsEnabled>true | false</MailTipsEnabled>
```

 <span data-ttu-id="e8cb1-105">**Boolean**</span><span class="sxs-lookup"><span data-stu-id="e8cb1-105">**Boolean**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e8cb1-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="e8cb1-106">Attributes and elements</span></span>

<span data-ttu-id="e8cb1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e8cb1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e8cb1-108">属性</span><span class="sxs-lookup"><span data-stu-id="e8cb1-108">Attributes</span></span>

<span data-ttu-id="e8cb1-109">なし。</span><span class="sxs-lookup"><span data-stu-id="e8cb1-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="e8cb1-110">子要素</span><span class="sxs-lookup"><span data-stu-id="e8cb1-110">Child elements</span></span>

<span data-ttu-id="e8cb1-111">なし。</span><span class="sxs-lookup"><span data-stu-id="e8cb1-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="e8cb1-112">親要素</span><span class="sxs-lookup"><span data-stu-id="e8cb1-112">Parent elements</span></span>

|<span data-ttu-id="e8cb1-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e8cb1-113">**Element**</span></span>|<span data-ttu-id="e8cb1-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e8cb1-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e8cb1-115">Mailヒント構成 (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="e8cb1-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="e8cb1-116">メールヒントサービスのサービス構成情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="e8cb1-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e8cb1-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e8cb1-117">Text value</span></span>

<span data-ttu-id="e8cb1-118">メールヒントサービスが利用可能な場合は、この要素のテキスト値は**true**です。</span><span class="sxs-lookup"><span data-stu-id="e8cb1-118">The text value of this element is **true** if the mail tips service is available.</span></span> <span data-ttu-id="e8cb1-119">メールヒントサービスが利用できない場合、値は**false**です。</span><span class="sxs-lookup"><span data-stu-id="e8cb1-119">The value is **false** if the mail tips service is not available.</span></span> 
  
## <a name="remarks"></a><span data-ttu-id="e8cb1-120">注釈</span><span class="sxs-lookup"><span data-stu-id="e8cb1-120">Remarks</span></span>

<span data-ttu-id="e8cb1-121">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="e8cb1-121">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e8cb1-122">要素の情報</span><span class="sxs-lookup"><span data-stu-id="e8cb1-122">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e8cb1-123">Namespace</span><span class="sxs-lookup"><span data-stu-id="e8cb1-123">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="e8cb1-124">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e8cb1-124">Schema Name</span></span>  <br/> |<span data-ttu-id="e8cb1-125">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="e8cb1-125">Types schema</span></span>  <br/> |
|<span data-ttu-id="e8cb1-126">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e8cb1-126">Validation File</span></span>  <br/> |<span data-ttu-id="e8cb1-127">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="e8cb1-127">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="e8cb1-128">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e8cb1-128">Can be Empty</span></span>  <br/> |<span data-ttu-id="e8cb1-129">正しくない</span><span class="sxs-lookup"><span data-stu-id="e8cb1-129">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e8cb1-130">関連項目</span><span class="sxs-lookup"><span data-stu-id="e8cb1-130">See also</span></span>



- [<span data-ttu-id="e8cb1-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="e8cb1-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

