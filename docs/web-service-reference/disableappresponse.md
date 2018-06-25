---
title: DisableAppResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 11ebe618-d759-4f16-be99-eaaa817ba782
description: DisableAppResponse 要素は、DisableApp 要求への応答を指定します。
ms.openlocfilehash: 740801fa4b60e217f0b9148bcfcc5b206e96bf31
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760065"
---
# <a name="disableappresponse"></a><span data-ttu-id="3e426-103">DisableAppResponse</span><span class="sxs-lookup"><span data-stu-id="3e426-103">DisableAppResponse</span></span>

<span data-ttu-id="3e426-104">**DisableAppResponse**要素は、 **DisableApp**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="3e426-104">The **DisableAppResponse** element specifies the response to a **DisableApp** request.</span></span> 
  
```XML
<DisableAppResponse>
    <MessageText></MessageText>
    <ResponseCode></ResponeCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</DisableAppResponse>
```

 <span data-ttu-id="3e426-105">**DisableAppResponseType**</span><span class="sxs-lookup"><span data-stu-id="3e426-105">**DisableAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3e426-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3e426-106">Attributes and elements</span></span>

<span data-ttu-id="3e426-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3e426-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3e426-108">属性</span><span class="sxs-lookup"><span data-stu-id="3e426-108">Attributes</span></span>

<span data-ttu-id="3e426-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3e426-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3e426-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3e426-110">Child elements</span></span>

|<span data-ttu-id="3e426-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="3e426-111">**Element**</span></span>|<span data-ttu-id="3e426-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3e426-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3e426-113">MessageText</span><span class="sxs-lookup"><span data-stu-id="3e426-113">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="3e426-114">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="3e426-114">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="3e426-115">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3e426-115">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="3e426-116">要求に関するステータス情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="3e426-116">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="3e426-117">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3e426-117">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="3e426-118">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="3e426-118">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="3e426-119">MessageXml</span><span class="sxs-lookup"><span data-stu-id="3e426-119">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="3e426-120">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="3e426-120">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3e426-121">親要素</span><span class="sxs-lookup"><span data-stu-id="3e426-121">Parent elements</span></span>

<span data-ttu-id="3e426-122">なし。</span><span class="sxs-lookup"><span data-stu-id="3e426-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="3e426-123">備考</span><span class="sxs-lookup"><span data-stu-id="3e426-123">Remarks</span></span>

<span data-ttu-id="3e426-124">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3e426-124">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="3e426-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="3e426-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3e426-126">要素情報</span><span class="sxs-lookup"><span data-stu-id="3e426-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3e426-127">名前空間</span><span class="sxs-lookup"><span data-stu-id="3e426-127">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3e426-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3e426-128">Schema Name</span></span>  <br/> |<span data-ttu-id="3e426-129">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="3e426-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="3e426-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3e426-130">Validation File</span></span>  <br/> |<span data-ttu-id="3e426-131">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3e426-131">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3e426-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="3e426-132">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="3e426-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="3e426-133">See also</span></span>

- [<span data-ttu-id="3e426-134">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="3e426-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

