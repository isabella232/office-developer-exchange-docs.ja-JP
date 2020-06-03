---
title: Max受信者 Spergetmailヒント要求
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxRecipientsPerGetMailTipsRequest
api_type:
- schema
ms.assetid: 8ff5df18-1989-4217-b4c0-599232911d0c
description: Max受信者 Spergetmailヒント要求要素は、Getメールヒント操作に渡すことができる受信者の最大数を示します。
ms.openlocfilehash: cec343182b364fce040d5e32928cbeb569a22124
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468405"
---
# <a name="maxrecipientspergetmailtipsrequest"></a><span data-ttu-id="c6f95-103">Max受信者 Spergetmailヒント要求</span><span class="sxs-lookup"><span data-stu-id="c6f95-103">MaxRecipientsPerGetMailTipsRequest</span></span>

<span data-ttu-id="c6f95-104">**Max受信者 Spergetmailヒント要求**要素は、 [getメールヒント操作](getmailtips-operation.md)に渡すことができる受信者の最大数を示します。</span><span class="sxs-lookup"><span data-stu-id="c6f95-104">The **MaxRecipientsPerGetMailTipsRequest** element indicates the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span>
  
```XML
<MaxRecipientsPerGetMailTipsRequest/>
```

 <span data-ttu-id="c6f95-105">**int**</span><span class="sxs-lookup"><span data-stu-id="c6f95-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c6f95-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c6f95-106">Attributes and elements</span></span>

<span data-ttu-id="c6f95-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c6f95-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c6f95-108">属性</span><span class="sxs-lookup"><span data-stu-id="c6f95-108">Attributes</span></span>

<span data-ttu-id="c6f95-109">なし。</span><span class="sxs-lookup"><span data-stu-id="c6f95-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c6f95-110">子要素</span><span class="sxs-lookup"><span data-stu-id="c6f95-110">Child elements</span></span>

<span data-ttu-id="c6f95-111">なし。</span><span class="sxs-lookup"><span data-stu-id="c6f95-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="c6f95-112">親要素</span><span class="sxs-lookup"><span data-stu-id="c6f95-112">Parent elements</span></span>

|<span data-ttu-id="c6f95-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="c6f95-113">**Element**</span></span>|<span data-ttu-id="c6f95-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="c6f95-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c6f95-115">Mailヒント構成 (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="c6f95-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="c6f95-116">メールヒントサービスのサービス構成情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="c6f95-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="c6f95-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c6f95-117">Text value</span></span>

<span data-ttu-id="c6f95-118">テキスト値は、 [Getmailtips ヒント操作](getmailtips-operation.md)に渡すことができる受信者の最大数を表す整数です。</span><span class="sxs-lookup"><span data-stu-id="c6f95-118">The text value is an integer that represents the maximum number of recipients that can be passed to the [GetMailTips operation](getmailtips-operation.md).</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c6f95-119">注釈</span><span class="sxs-lookup"><span data-stu-id="c6f95-119">Remarks</span></span>

<span data-ttu-id="c6f95-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="c6f95-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c6f95-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c6f95-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c6f95-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="c6f95-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="c6f95-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c6f95-123">Schema Name</span></span>  <br/> |<span data-ttu-id="c6f95-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="c6f95-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="c6f95-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c6f95-125">Validation File</span></span>  <br/> |<span data-ttu-id="c6f95-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="c6f95-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="c6f95-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c6f95-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="c6f95-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="c6f95-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c6f95-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="c6f95-129">See also</span></span>



[<span data-ttu-id="c6f95-130">GetMailTips ヒント操作</span><span class="sxs-lookup"><span data-stu-id="c6f95-130">GetMailTips operation</span></span>](getmailtips-operation.md)


- [<span data-ttu-id="c6f95-131">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c6f95-131">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

