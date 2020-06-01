---
title: WebClientUrls (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: fdfe6059-a861-4fa2-a20e-ee6ab820bee9
description: WebClientUrls 要素は、Webclienturls (SOAP) 要素のコレクションを含むユーザー設定を表します。
ms.openlocfilehash: 80c8ab36e30146c78f4bdb4f40eb9f87a335199c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464925"
---
# <a name="webclienturls-soap"></a><span data-ttu-id="c4a84-103">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c4a84-103">WebClientUrls (SOAP)</span></span>

<span data-ttu-id="c4a84-104">**Webclienturls**要素は、 [webclienturls (SOAP)](webclienturl-soap.md)要素のコレクションを含むユーザー設定を表します。</span><span class="sxs-lookup"><span data-stu-id="c4a84-104">The **WebClientUrls** element represents a user setting that contains a collection of [WebClientUrl (SOAP)](webclienturl-soap.md) elements.</span></span> 
  
[<span data-ttu-id="c4a84-105">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c4a84-105">UserSetting (SOAP)</span></span>](usersetting-soap.md)
  
[<span data-ttu-id="c4a84-106">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c4a84-106">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)
  
[<span data-ttu-id="c4a84-107">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c4a84-107">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md)
  
```XML
<WebClientUrls>
     <WebClientUrl/>
</WebClientUrls>

```

 <span data-ttu-id="c4a84-108">**WebClientUrls**</span><span class="sxs-lookup"><span data-stu-id="c4a84-108">**WebClientUrls**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c4a84-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c4a84-109">Attributes and elements</span></span>

<span data-ttu-id="c4a84-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c4a84-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c4a84-111">属性</span><span class="sxs-lookup"><span data-stu-id="c4a84-111">Attributes</span></span>

<span data-ttu-id="c4a84-112">なし。</span><span class="sxs-lookup"><span data-stu-id="c4a84-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="c4a84-113">子要素</span><span class="sxs-lookup"><span data-stu-id="c4a84-113">Child elements</span></span>

|<span data-ttu-id="c4a84-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="c4a84-114">**Element**</span></span>|<span data-ttu-id="c4a84-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="c4a84-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4a84-116">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c4a84-116">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md) <br/> |<span data-ttu-id="c4a84-117">Exchange クライアントの URL を表します。</span><span class="sxs-lookup"><span data-stu-id="c4a84-117">Represents an Exchange client URL.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c4a84-118">親要素</span><span class="sxs-lookup"><span data-stu-id="c4a84-118">Parent elements</span></span>

|<span data-ttu-id="c4a84-119">**要素**</span><span class="sxs-lookup"><span data-stu-id="c4a84-119">**Element**</span></span>|<span data-ttu-id="c4a84-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="c4a84-120">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c4a84-121">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c4a84-121">UserSetting (SOAP)</span></span>](usersetting-soap.md) <br/> |<span data-ttu-id="c4a84-122">GetUserSettings 要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="c4a84-122">Represents a response to a GetUserSettings request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="c4a84-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c4a84-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c4a84-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="c4a84-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="c4a84-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c4a84-125">Schema Name</span></span>  <br/> |<span data-ttu-id="c4a84-126">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="c4a84-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="c4a84-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c4a84-127">Validation File</span></span>  <br/> |<span data-ttu-id="c4a84-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c4a84-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c4a84-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c4a84-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="c4a84-130">正しい</span><span class="sxs-lookup"><span data-stu-id="c4a84-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c4a84-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="c4a84-131">See also</span></span>



[<span data-ttu-id="c4a84-132">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="c4a84-132">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md)

