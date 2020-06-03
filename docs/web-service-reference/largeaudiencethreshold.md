---
title: LargeAudienceThreshold
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- LargeAudienceThreshold
api_type:
- schema
ms.assetid: dacd9db7-b8f0-445d-a3d1-3356b8c2bcd1
description: LargeAudienceThreshold 要素は、クライアントの大規模な対象ユーザーのしきい値を表します。
ms.openlocfilehash: 6d85f9eaf8b7723713877d376876461befa92324
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44466389"
---
# <a name="largeaudiencethreshold"></a><span data-ttu-id="a8f6a-103">LargeAudienceThreshold</span><span class="sxs-lookup"><span data-stu-id="a8f6a-103">LargeAudienceThreshold</span></span>

<span data-ttu-id="a8f6a-104">**LargeAudienceThreshold**要素は、クライアントの大規模な対象ユーザーのしきい値を表します。</span><span class="sxs-lookup"><span data-stu-id="a8f6a-104">The **LargeAudienceThreshold** element represents the large audience threshold for a client.</span></span> 
  
```XML
<LargeAudienceThreshold/>
```

 <span data-ttu-id="a8f6a-105">**int**</span><span class="sxs-lookup"><span data-stu-id="a8f6a-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="a8f6a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="a8f6a-106">Attributes and elements</span></span>

<span data-ttu-id="a8f6a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a8f6a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a8f6a-108">属性</span><span class="sxs-lookup"><span data-stu-id="a8f6a-108">Attributes</span></span>

<span data-ttu-id="a8f6a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="a8f6a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="a8f6a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="a8f6a-110">Child elements</span></span>

<span data-ttu-id="a8f6a-111">なし。</span><span class="sxs-lookup"><span data-stu-id="a8f6a-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="a8f6a-112">親要素</span><span class="sxs-lookup"><span data-stu-id="a8f6a-112">Parent elements</span></span>

|<span data-ttu-id="a8f6a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a8f6a-113">**Element**</span></span>|<span data-ttu-id="a8f6a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a8f6a-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a8f6a-115">Mailヒント構成 (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="a8f6a-115">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="a8f6a-116">メールヒントサービスのサービス構成情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="a8f6a-116">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="a8f6a-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="a8f6a-117">Text value</span></span>

<span data-ttu-id="a8f6a-118">テキスト値は、メッセージが複数のユーザーに送信されることを示す、対象ユーザーのしきい値を表す整数です。</span><span class="sxs-lookup"><span data-stu-id="a8f6a-118">The text value is an integer that represents the audience threshold that indicates that the message is going to more than one person.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="a8f6a-119">注釈</span><span class="sxs-lookup"><span data-stu-id="a8f6a-119">Remarks</span></span>

<span data-ttu-id="a8f6a-120">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="a8f6a-120">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a8f6a-121">要素の情報</span><span class="sxs-lookup"><span data-stu-id="a8f6a-121">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a8f6a-122">Namespace</span><span class="sxs-lookup"><span data-stu-id="a8f6a-122">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="a8f6a-123">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a8f6a-123">Schema Name</span></span>  <br/> |<span data-ttu-id="a8f6a-124">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="a8f6a-124">Types schema</span></span>  <br/> |
|<span data-ttu-id="a8f6a-125">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a8f6a-125">Validation File</span></span>  <br/> |<span data-ttu-id="a8f6a-126">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="a8f6a-126">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="a8f6a-127">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a8f6a-127">Can be Empty</span></span>  <br/> |<span data-ttu-id="a8f6a-128">正しくない</span><span class="sxs-lookup"><span data-stu-id="a8f6a-128">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a8f6a-129">関連項目</span><span class="sxs-lookup"><span data-stu-id="a8f6a-129">See also</span></span>



- [<span data-ttu-id="a8f6a-130">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="a8f6a-130">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

