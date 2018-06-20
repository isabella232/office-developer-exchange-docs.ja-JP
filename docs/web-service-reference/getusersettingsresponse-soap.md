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
description: GetUserSettingsResponse 要素は、GetUserSettings の操作 (SOAP) 要求に対する応答を表します。
ms.openlocfilehash: 24dbfb1582f628fd0130aa82ea5f1beedd31b156
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831705"
---
# <a name="getusersettingsresponse-soap"></a><span data-ttu-id="3b8d3-103">GetUserSettingsResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3b8d3-103">GetUserSettingsResponse (SOAP)</span></span>

<span data-ttu-id="3b8d3-104">**GetUserSettingsResponse**要素は、 [GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)要求に対する応答を表します。</span><span class="sxs-lookup"><span data-stu-id="3b8d3-104">The **GetUserSettingsResponse** element represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span> 
  
```XML
<GetUserSettingsResponse>
   <ErrorCode/>
   <ErrorMessage/>
   <UserResponses/>
</GetUserSettingsResponse>
```

 <span data-ttu-id="3b8d3-105">**GetUserSettingsResponse**</span><span class="sxs-lookup"><span data-stu-id="3b8d3-105">**GetUserSettingsResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b8d3-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3b8d3-106">Attributes and elements</span></span>

<span data-ttu-id="3b8d3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3b8d3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b8d3-108">属性</span><span class="sxs-lookup"><span data-stu-id="3b8d3-108">Attributes</span></span>

<span data-ttu-id="3b8d3-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3b8d3-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3b8d3-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3b8d3-110">Child elements</span></span>

|<span data-ttu-id="3b8d3-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="3b8d3-111">**Element**</span></span>|<span data-ttu-id="3b8d3-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3b8d3-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b8d3-113">エラー コード (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3b8d3-113">ErrorCode (SOAP)</span></span>](errorcode-soap.md) <br/> |<span data-ttu-id="3b8d3-114">自動検出サービスによって返されるエラー コードを表します。</span><span class="sxs-lookup"><span data-stu-id="3b8d3-114">Represents an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="3b8d3-115">エラー メッセージ (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3b8d3-115">ErrorMessage (SOAP)</span></span>](errormessage-soap.md) <br/> |<span data-ttu-id="3b8d3-116">自動検出サービスによって返されるエラー コードに関連付けられているメッセージを表します。</span><span class="sxs-lookup"><span data-stu-id="3b8d3-116">Represents a message that is associated with an error code that is returned by the Autodiscover service.</span></span>  <br/> |
|[<span data-ttu-id="3b8d3-117">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3b8d3-117">UserResponses (SOAP)</span></span>](userresponses-soap.md) <br/> |<span data-ttu-id="3b8d3-118">要求された各ユーザーの構成設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3b8d3-118">Contains the configuration settings for each requested user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3b8d3-119">親要素</span><span class="sxs-lookup"><span data-stu-id="3b8d3-119">Parent elements</span></span>

<span data-ttu-id="3b8d3-120">なし。</span><span class="sxs-lookup"><span data-stu-id="3b8d3-120">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="3b8d3-121">テキスト値</span><span class="sxs-lookup"><span data-stu-id="3b8d3-121">Text value</span></span>

<span data-ttu-id="3b8d3-122">なし。</span><span class="sxs-lookup"><span data-stu-id="3b8d3-122">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3b8d3-123">要素情報</span><span class="sxs-lookup"><span data-stu-id="3b8d3-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b8d3-124">名前空間</span><span class="sxs-lookup"><span data-stu-id="3b8d3-124">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="3b8d3-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3b8d3-125">Schema Name</span></span>  <br/> |<span data-ttu-id="3b8d3-126">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="3b8d3-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="3b8d3-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3b8d3-127">Validation File</span></span>  <br/> |<span data-ttu-id="3b8d3-128">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3b8d3-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3b8d3-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3b8d3-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="3b8d3-130">True</span><span class="sxs-lookup"><span data-stu-id="3b8d3-130">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3b8d3-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="3b8d3-131">See also</span></span>



[<span data-ttu-id="3b8d3-132">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3b8d3-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

