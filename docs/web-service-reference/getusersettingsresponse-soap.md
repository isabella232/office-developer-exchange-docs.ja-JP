---
title: GetUserSettingsResponse (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: e7cd470d-5861-41e7-9e66-73ef7a59700b
description: GetUserSettingsResponse 要素は、GetUserSettings 操作 (SOAP) 要求への応答を表します。
ms.openlocfilehash: a41a195a003789ddaef81f844e47aad689df0937
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530149"
---
# <a name="getusersettingsresponse-soap"></a><span data-ttu-id="6a026-103">GetUserSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6a026-103">GetUserSettingsResponse (SOAP)</span></span>

<span data-ttu-id="6a026-104">**Getusersettingsresponse**要素は、 [getusersettings 操作 (SOAP)](getusersettings-operation-soap.md)要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="6a026-104">The **GetUserSettingsResponse** element represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span> 
  
```XML
<GetUserSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</GetUserSettingsResponse>
```

 <span data-ttu-id="6a026-105">**GetUserSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="6a026-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a026-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6a026-106">Attributes and elements</span></span>

<span data-ttu-id="6a026-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6a026-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a026-108">属性</span><span class="sxs-lookup"><span data-stu-id="6a026-108">Attributes</span></span>

<span data-ttu-id="6a026-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6a026-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a026-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6a026-110">Child elements</span></span>

|<span data-ttu-id="6a026-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="6a026-111">**Element**</span></span>|<span data-ttu-id="6a026-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6a026-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a026-113">ErrorCode (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6a026-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="6a026-114">自動検出サービスによって返されるエラーコードを表します。</span><span class="sxs-lookup"><span data-stu-id="6a026-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="6a026-115">ErrorMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6a026-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="6a026-116">自動検出サービスによって返されるエラーコードに関連付けられているメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="6a026-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="6a026-117">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6a026-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="6a026-118">要求された各ユーザーの構成設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="6a026-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6a026-119">親要素</span><span class="sxs-lookup"><span data-stu-id="6a026-119">Parent elements</span></span>

<span data-ttu-id="6a026-120">なし。</span><span class="sxs-lookup"><span data-stu-id="6a026-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="6a026-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6a026-121">Text value</span></span>

<span data-ttu-id="6a026-122">なし。</span><span class="sxs-lookup"><span data-stu-id="6a026-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6a026-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6a026-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a026-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="6a026-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="6a026-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6a026-125">Schema Name</span></span>  <br/> |<span data-ttu-id="6a026-126">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="6a026-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="6a026-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6a026-127">Validation File</span></span>  <br/> |<span data-ttu-id="6a026-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="6a026-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6a026-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6a026-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="6a026-130">正しい</span><span class="sxs-lookup"><span data-stu-id="6a026-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6a026-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="6a026-131">See also</span></span>



[<span data-ttu-id="6a026-132">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6a026-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

