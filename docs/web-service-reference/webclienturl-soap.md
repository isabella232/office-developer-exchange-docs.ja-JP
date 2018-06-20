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
ms.openlocfilehash: 649845018acee1706a96f9e37475a6d5c5fa0aa7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19840014"
---
# <a name="webclienturl-soap"></a><span data-ttu-id="0efa9-103">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0efa9-103">WebClientUrl (SOAP)</span></span>

<span data-ttu-id="0efa9-104">**WebClientUrl**要素は、Exchange web クライアントの URL を表します。</span><span class="sxs-lookup"><span data-stu-id="0efa9-104">The **WebClientUrl** element represents the URL of an Exchange web client.</span></span> 
  
[<span data-ttu-id="0efa9-105">UserSetting (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0efa9-105">UserSetting (SOAP)</span></span>](usersetting-soap.md)
  
[<span data-ttu-id="0efa9-106">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0efa9-106">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)
  
[<span data-ttu-id="0efa9-107">WebClientUrl (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0efa9-107">WebClientUrl (SOAP)</span></span>](webclienturl-soap.md)
  
```XML
<WebClientUrl>
    <AuthenticationMethods/>
    <Url/>
</WebClientUrl>
```

 <span data-ttu-id="0efa9-108">**WebClientUrl**</span><span class="sxs-lookup"><span data-stu-id="0efa9-108">**WebClientUrl**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0efa9-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0efa9-109">Attributes and elements</span></span>

<span data-ttu-id="0efa9-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0efa9-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0efa9-111">属性</span><span class="sxs-lookup"><span data-stu-id="0efa9-111">Attributes</span></span>

<span data-ttu-id="0efa9-112">なし。</span><span class="sxs-lookup"><span data-stu-id="0efa9-112">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="0efa9-113">子要素</span><span class="sxs-lookup"><span data-stu-id="0efa9-113">Child elements</span></span>

|<span data-ttu-id="0efa9-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="0efa9-114">**Element**</span></span>|<span data-ttu-id="0efa9-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="0efa9-115">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0efa9-116">AuthenticationMethods (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0efa9-116">AuthenticationMethods (SOAP)</span></span>](authenticationmethods-soap.md) <br/> |<span data-ttu-id="0efa9-117">指定した URL にアクセスするときに使用する認証メソッドを表します。</span><span class="sxs-lookup"><span data-stu-id="0efa9-117">Represents the authentication method to use when accessing the specified URL.</span></span>  <br/> |
|[<span data-ttu-id="0efa9-118">Url (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0efa9-118">Url (SOAP)</span></span>](url-soap.md) <br/> |<span data-ttu-id="0efa9-119">URL の web アドレスを表します。</span><span class="sxs-lookup"><span data-stu-id="0efa9-119">Represents the web address for the URL.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0efa9-120">親要素</span><span class="sxs-lookup"><span data-stu-id="0efa9-120">Parent elements</span></span>

|<span data-ttu-id="0efa9-121">**要素**</span><span class="sxs-lookup"><span data-stu-id="0efa9-121">**Element**</span></span>|<span data-ttu-id="0efa9-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="0efa9-122">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0efa9-123">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0efa9-123">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md) <br/> |<span data-ttu-id="0efa9-124">**WebClientUrl**要素のコレクションを含むユーザー設定を表します。</span><span class="sxs-lookup"><span data-stu-id="0efa9-124">Represents a user setting that contains a collection of **WebClientUrl** elements.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="0efa9-125">要素情報</span><span class="sxs-lookup"><span data-stu-id="0efa9-125">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0efa9-126">名前空間</span><span class="sxs-lookup"><span data-stu-id="0efa9-126">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="0efa9-127">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0efa9-127">Schema Name</span></span>  <br/> |<span data-ttu-id="0efa9-128">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="0efa9-128">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="0efa9-129">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0efa9-129">Validation File</span></span>  <br/> |<span data-ttu-id="0efa9-130">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0efa9-130">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0efa9-131">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0efa9-131">Can be Empty</span></span>  <br/> |<span data-ttu-id="0efa9-132">True</span><span class="sxs-lookup"><span data-stu-id="0efa9-132">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0efa9-133">関連項目</span><span class="sxs-lookup"><span data-stu-id="0efa9-133">See also</span></span>



[<span data-ttu-id="0efa9-134">Url (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0efa9-134">Url (SOAP)</span></span>](url-soap.md)
  
[<span data-ttu-id="0efa9-135">WebClientUrls (SOAP)</span><span class="sxs-lookup"><span data-stu-id="0efa9-135">WebClientUrls (SOAP)</span></span>](webclienturls-soap.md)

