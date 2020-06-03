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
ms.openlocfilehash: cc28abf644247339e1226cd0e13824cc5f5669be
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455647"
---
# <a name="disableappresponse"></a><span data-ttu-id="d2f92-103">DisableAppResponse</span><span class="sxs-lookup"><span data-stu-id="d2f92-103">DisableAppResponse</span></span>

<span data-ttu-id="d2f92-104">**DisableAppResponse**要素は、 **disableapp**要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="d2f92-104">The **DisableAppResponse** element specifies the response to a **DisableApp** request.</span></span> 
  
```XML
<DisableAppResponse>
    <MessageText></MessageText>
    <ResponseCode></ResponeCode>
    <DescriptiveLinkKey></DescriptiveLinkKey>
    <MessageXml></MessageXml>
</DisableAppResponse>
```

 <span data-ttu-id="d2f92-105">**DisableAppResponseType**</span><span class="sxs-lookup"><span data-stu-id="d2f92-105">**DisableAppResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2f92-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d2f92-106">Attributes and elements</span></span>

<span data-ttu-id="d2f92-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d2f92-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2f92-108">属性</span><span class="sxs-lookup"><span data-stu-id="d2f92-108">Attributes</span></span>

<span data-ttu-id="d2f92-109">なし。</span><span class="sxs-lookup"><span data-stu-id="d2f92-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d2f92-110">子要素</span><span class="sxs-lookup"><span data-stu-id="d2f92-110">Child elements</span></span>

|<span data-ttu-id="d2f92-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="d2f92-111">**Element**</span></span>|<span data-ttu-id="d2f92-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2f92-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2f92-113">MessageText</span><span class="sxs-lookup"><span data-stu-id="d2f92-113">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d2f92-114">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="d2f92-114">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d2f92-115">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d2f92-115">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d2f92-116">要求に関する状態情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="d2f92-116">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="d2f92-117">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d2f92-117">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d2f92-118">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="d2f92-118">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="d2f92-119">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d2f92-119">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d2f92-120">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="d2f92-120">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d2f92-121">親要素</span><span class="sxs-lookup"><span data-stu-id="d2f92-121">Parent elements</span></span>

<span data-ttu-id="d2f92-122">なし。</span><span class="sxs-lookup"><span data-stu-id="d2f92-122">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d2f92-123">注釈</span><span class="sxs-lookup"><span data-stu-id="d2f92-123">Remarks</span></span>

<span data-ttu-id="d2f92-124">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d2f92-124">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="d2f92-125">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d2f92-125">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2f92-126">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d2f92-126">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2f92-127">Namespace</span><span class="sxs-lookup"><span data-stu-id="d2f92-127">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d2f92-128">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d2f92-128">Schema Name</span></span>  <br/> |<span data-ttu-id="d2f92-129">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d2f92-129">Message schema</span></span>  <br/> |
|<span data-ttu-id="d2f92-130">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d2f92-130">Validation File</span></span>  <br/> |<span data-ttu-id="d2f92-131">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d2f92-131">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d2f92-132">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d2f92-132">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="d2f92-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="d2f92-133">See also</span></span>

- [<span data-ttu-id="d2f92-134">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d2f92-134">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

