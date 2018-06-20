---
title: UserResponses (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: a48766df-4cc8-47c2-a8c1-826daec94e5a
description: UserResponses 要素には、要求された各ユーザーの構成設定が含まれています。
ms.openlocfilehash: bee7f3c9a95c1facfe0adc990516dfa323d9c8cf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839947"
---
# <a name="userresponses-soap"></a><span data-ttu-id="4339e-103">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4339e-103">UserResponses (SOAP)</span></span>

<span data-ttu-id="4339e-104">**UserResponses**要素には、要求された各ユーザーの構成設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4339e-104">The **UserResponses** element contains the configuration settings for each requested user.</span></span> 
  
```XML
<UserResponses>
   <UserResponse/>
</UserResponses>
```

 <span data-ttu-id="4339e-105">**ArrayOfUserResponse**</span><span class="sxs-lookup"><span data-stu-id="4339e-105">**ArrayOfUserResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4339e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4339e-106">Attributes and elements</span></span>

<span data-ttu-id="4339e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4339e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4339e-108">属性</span><span class="sxs-lookup"><span data-stu-id="4339e-108">Attributes</span></span>

<span data-ttu-id="4339e-109">なし。</span><span class="sxs-lookup"><span data-stu-id="4339e-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="4339e-110">子要素</span><span class="sxs-lookup"><span data-stu-id="4339e-110">Child elements</span></span>

|<span data-ttu-id="4339e-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="4339e-111">**Element**</span></span>|<span data-ttu-id="4339e-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="4339e-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4339e-113">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4339e-113">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="4339e-114">個々 のユーザーに対して[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)要求に対する応答を表します。</span><span class="sxs-lookup"><span data-stu-id="4339e-114">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4339e-115">親要素</span><span class="sxs-lookup"><span data-stu-id="4339e-115">Parent elements</span></span>

|<span data-ttu-id="4339e-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="4339e-116">**Element**</span></span>|<span data-ttu-id="4339e-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="4339e-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4339e-118">応答 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4339e-118">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="4339e-119">[GetUserSettings 操作 (SOAP)](getusersettings-operation-soap.md)要求への応答が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4339e-119">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="4339e-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="4339e-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4339e-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="4339e-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="4339e-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4339e-122">Schema Name</span></span>  <br/> |<span data-ttu-id="4339e-123">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="4339e-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="4339e-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4339e-124">Validation File</span></span>  <br/> |<span data-ttu-id="4339e-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4339e-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4339e-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4339e-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="4339e-127">True</span><span class="sxs-lookup"><span data-stu-id="4339e-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4339e-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="4339e-128">See also</span></span>



[<span data-ttu-id="4339e-129">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="4339e-129">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

