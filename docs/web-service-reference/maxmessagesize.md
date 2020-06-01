---
title: MaxMessageSize
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MaxMessageSize
api_type:
- schema
ms.assetid: bb98ac72-9409-4332-81bb-ee3bebb9a00e
description: MaxMessageSize 要素は、受信者が受け付けることができる最大メッセージサイズを表します。
ms.openlocfilehash: 727eed38a129800b7d38aa49c41cdacfa13e7a36
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468412"
---
# <a name="maxmessagesize"></a><span data-ttu-id="12b30-103">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="12b30-103">MaxMessageSize</span></span>

<span data-ttu-id="12b30-104">**Maxmessagesize**要素は、受信者が受け付けることができる最大メッセージサイズを表します。</span><span class="sxs-lookup"><span data-stu-id="12b30-104">The **MaxMessageSize** element represents the maximum message size a recipient can accept.</span></span> 
  
```XML
<MaxMessageSize/>
```

 <span data-ttu-id="12b30-105">**int**</span><span class="sxs-lookup"><span data-stu-id="12b30-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="12b30-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="12b30-106">Attributes and elements</span></span>

<span data-ttu-id="12b30-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="12b30-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="12b30-108">属性</span><span class="sxs-lookup"><span data-stu-id="12b30-108">Attributes</span></span>

<span data-ttu-id="12b30-109">なし。</span><span class="sxs-lookup"><span data-stu-id="12b30-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="12b30-110">子要素</span><span class="sxs-lookup"><span data-stu-id="12b30-110">Child elements</span></span>

<span data-ttu-id="12b30-111">なし。</span><span class="sxs-lookup"><span data-stu-id="12b30-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="12b30-112">親要素</span><span class="sxs-lookup"><span data-stu-id="12b30-112">Parent elements</span></span>

|<span data-ttu-id="12b30-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="12b30-113">**Element**</span></span>|<span data-ttu-id="12b30-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="12b30-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="12b30-115">メールヒント</span><span class="sxs-lookup"><span data-stu-id="12b30-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="12b30-116">さまざまな種類のメールヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="12b30-116">Represents values for various types of mail tips.</span></span>  <br/> |
|[<span data-ttu-id="12b30-117">Mailヒント構成 (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="12b30-117">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="12b30-118">メールヒントサービスのサービス構成情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="12b30-118">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="12b30-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="12b30-119">Text value</span></span>

<span data-ttu-id="12b30-120">テキスト値は、受信者が受け付けることができる最大メッセージサイズを表す整数型 (integer) の値です。</span><span class="sxs-lookup"><span data-stu-id="12b30-120">The text value is an integer that represents the maximum message size a recipient can accept.</span></span> <span data-ttu-id="12b30-121">この値は、キロバイトまたはメガバイト単位で測定できます。</span><span class="sxs-lookup"><span data-stu-id="12b30-121">This value can be measured in kilobytes or megabytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="12b30-122">注釈</span><span class="sxs-lookup"><span data-stu-id="12b30-122">Remarks</span></span>

<span data-ttu-id="12b30-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="12b30-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="12b30-124">要素の情報</span><span class="sxs-lookup"><span data-stu-id="12b30-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="12b30-125">Namespace</span><span class="sxs-lookup"><span data-stu-id="12b30-125">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="12b30-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="12b30-126">Schema Name</span></span>  <br/> |<span data-ttu-id="12b30-127">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="12b30-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="12b30-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="12b30-128">Validation File</span></span>  <br/> |<span data-ttu-id="12b30-129">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="12b30-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="12b30-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="12b30-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="12b30-131">正しくない</span><span class="sxs-lookup"><span data-stu-id="12b30-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="12b30-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="12b30-132">See also</span></span>



- [<span data-ttu-id="12b30-133">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="12b30-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

