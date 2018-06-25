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
description: MaxMessageSize 要素は、受信者が受け入れることができるメッセージの最大サイズを表します。
ms.openlocfilehash: 13a5679a03420655356269a7e8b5e22950724164
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832383"
---
# <a name="maxmessagesize"></a><span data-ttu-id="55bcd-103">MaxMessageSize</span><span class="sxs-lookup"><span data-stu-id="55bcd-103">MaxMessageSize</span></span>

<span data-ttu-id="55bcd-104">**MaxMessageSize**要素は、受信者が受け入れることができるメッセージの最大サイズを表します。</span><span class="sxs-lookup"><span data-stu-id="55bcd-104">The **MaxMessageSize** element represents the maximum message size a recipient can accept.</span></span> 
  
```XML
<MaxMessageSize/>
```

 <span data-ttu-id="55bcd-105">**int**</span><span class="sxs-lookup"><span data-stu-id="55bcd-105">**int**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="55bcd-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="55bcd-106">Attributes and elements</span></span>

<span data-ttu-id="55bcd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="55bcd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="55bcd-108">属性</span><span class="sxs-lookup"><span data-stu-id="55bcd-108">Attributes</span></span>

<span data-ttu-id="55bcd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="55bcd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="55bcd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="55bcd-110">Child elements</span></span>

<span data-ttu-id="55bcd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="55bcd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="55bcd-112">親要素</span><span class="sxs-lookup"><span data-stu-id="55bcd-112">Parent elements</span></span>

|<span data-ttu-id="55bcd-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="55bcd-113">**Element**</span></span>|<span data-ttu-id="55bcd-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="55bcd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="55bcd-115">メール ヒント</span><span class="sxs-lookup"><span data-stu-id="55bcd-115">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="55bcd-116">さまざまな種類のメール ヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="55bcd-116">Represents values for various types of mail tips.</span></span>  <br/> |
|[<span data-ttu-id="55bcd-117">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="55bcd-117">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="55bcd-118">メール ヒント サービスのサービスの構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="55bcd-118">Contains service configuration information for the mail tips service.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="55bcd-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="55bcd-119">Text value</span></span>

<span data-ttu-id="55bcd-120">テキスト値は、受信者のメッセージの最大サイズを表す整数を受け入れることができます。</span><span class="sxs-lookup"><span data-stu-id="55bcd-120">The text value is an integer that represents the maximum message size a recipient can accept.</span></span> <span data-ttu-id="55bcd-121">キロバイトまたはメガバイト単位でこの値を測定することができます。</span><span class="sxs-lookup"><span data-stu-id="55bcd-121">This value can be measured in kilobytes or megabytes.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="55bcd-122">備考</span><span class="sxs-lookup"><span data-stu-id="55bcd-122">Remarks</span></span>

<span data-ttu-id="55bcd-123">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="55bcd-123">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="55bcd-124">要素情報</span><span class="sxs-lookup"><span data-stu-id="55bcd-124">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="55bcd-125">名前空間</span><span class="sxs-lookup"><span data-stu-id="55bcd-125">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="55bcd-126">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="55bcd-126">Schema Name</span></span>  <br/> |<span data-ttu-id="55bcd-127">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="55bcd-127">Types schema</span></span>  <br/> |
|<span data-ttu-id="55bcd-128">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="55bcd-128">Validation File</span></span>  <br/> |<span data-ttu-id="55bcd-129">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="55bcd-129">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="55bcd-130">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="55bcd-130">Can be Empty</span></span>  <br/> |<span data-ttu-id="55bcd-131">False</span><span class="sxs-lookup"><span data-stu-id="55bcd-131">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="55bcd-132">関連項目</span><span class="sxs-lookup"><span data-stu-id="55bcd-132">See also</span></span>



- [<span data-ttu-id="55bcd-133">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="55bcd-133">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

