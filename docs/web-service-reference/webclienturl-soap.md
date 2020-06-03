---
title: WebClientUrl (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 7f8cb6d6-4aac-4a1f-8bec-2dcb90fc1df6
description: WebClientUrl 要素は、Exchange web クライアントの URL を表します。
ms.openlocfilehash: bcf9c8d4fe80de8af4c9500e5e850558a8451d4e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464974"
---
# <a name="webclienturl-soap"></a><span data-ttu-id="d58d0-103">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d58d0-103">WebClientUrl (SOAP)</span></span>

<span data-ttu-id="d58d0-104">**Webclienturl**要素は、Exchange web クライアントの URL を表します。</span><span class="sxs-lookup"><span data-stu-id="d58d0-104">The **WebClientUrl** element represents the URL of an Exchange web client.</span></span> 
  
[<span data-ttu-id="d58d0-105">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d58d0-105">UserSetting (SOAP)</span></span>](usersetting-soap.md)
  
[<span data-ttu-id="d58d0-106">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d58d0-106">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)
  
[<span data-ttu-id="d58d0-107">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d58d0-107">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md)
  
```XML
<WebClientUrl>
    <AuthenticationMethods/>
    <Url/>
</WebClientUrl>
```

 <span data-ttu-id="d58d0-108">**WebClientUrl**</span><span class="sxs-lookup"><span data-stu-id="d58d0-108">**WebClientUrl**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d58d0-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d58d0-109">Attributes and elements</span></span>

<span data-ttu-id="d58d0-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d58d0-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d58d0-111">属性</span><span class="sxs-lookup"><span data-stu-id="d58d0-111">Attributes</span></span>

<span data-ttu-id="d58d0-112">なし。</span><span class="sxs-lookup"><span data-stu-id="d58d0-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="d58d0-113">子要素</span><span class="sxs-lookup"><span data-stu-id="d58d0-113">Child elements</span></span>

|<span data-ttu-id="d58d0-114">**Element**</span><span class="sxs-lookup"><span data-stu-id="d58d0-114">**Element**</span></span>|<span data-ttu-id="d58d0-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="d58d0-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d58d0-116">AuthenticationMethods (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d58d0-116">AuthenticationMethods (SOAP)</span></span>](authenticationmethods-soap.md) <br/> |<span data-ttu-id="d58d0-117">指定した URL にアクセスするときに使用する認証方法を表します。</span><span class="sxs-lookup"><span data-stu-id="d58d0-117">Represents the authentication method to use when accessing the specified URL.</span></span>  <br/> |
|[<span data-ttu-id="d58d0-118">Url (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d58d0-118">Url (SOAP)</span></span>](url-soap.md) <br/> |<span data-ttu-id="d58d0-119">URL の web アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="d58d0-119">Represents the web address for the URL.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d58d0-120">親要素</span><span class="sxs-lookup"><span data-stu-id="d58d0-120">Parent elements</span></span>

|<span data-ttu-id="d58d0-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="d58d0-121">**Element**</span></span>|<span data-ttu-id="d58d0-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="d58d0-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d58d0-123">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d58d0-123">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md) <br/> |<span data-ttu-id="d58d0-124">**Webclienturl**要素のコレクションを含むユーザー設定を表します。</span><span class="sxs-lookup"><span data-stu-id="d58d0-124">Represents a user setting that contains a collection of **WebClientUrl** elements.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="d58d0-125">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d58d0-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d58d0-126">Namespace</span><span class="sxs-lookup"><span data-stu-id="d58d0-126">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="d58d0-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d58d0-127">Schema Name</span></span>  <br/> |<span data-ttu-id="d58d0-128">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="d58d0-128">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="d58d0-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d58d0-129">Validation File</span></span>  <br/> |<span data-ttu-id="d58d0-130">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d58d0-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d58d0-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d58d0-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="d58d0-132">正しい</span><span class="sxs-lookup"><span data-stu-id="d58d0-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d58d0-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="d58d0-133">See also</span></span>



[<span data-ttu-id="d58d0-134">Url (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d58d0-134">Url (SOAP)</span></span>](url-soap.md)
  
[<span data-ttu-id="d58d0-135">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="d58d0-135">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)

