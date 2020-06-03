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
description: UserResponses 要素には、要求された各ユーザーの構成設定が含まれます。
ms.openlocfilehash: db2bab16334b90395d29dc03353dce05b0e45357
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526747"
---
# <a name="userresponses-soap"></a><span data-ttu-id="3208a-103">UserResponses (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3208a-103">UserResponses (SOAP)</span></span>

<span data-ttu-id="3208a-104">**Userresponses**要素には、要求された各ユーザーの構成設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="3208a-104">The **UserResponses** element contains the configuration settings for each requested user.</span></span> 
  
```XML
<UserResponses>
   <UserResponse/>
</UserResponses>
```

 <span data-ttu-id="3208a-105">**ArrayOfUserResponse**</span><span class="sxs-lookup"><span data-stu-id="3208a-105">**ArrayOfUserResponse**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3208a-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3208a-106">Attributes and elements</span></span>

<span data-ttu-id="3208a-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3208a-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3208a-108">属性</span><span class="sxs-lookup"><span data-stu-id="3208a-108">Attributes</span></span>

<span data-ttu-id="3208a-109">なし。</span><span class="sxs-lookup"><span data-stu-id="3208a-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="3208a-110">子要素</span><span class="sxs-lookup"><span data-stu-id="3208a-110">Child elements</span></span>

|<span data-ttu-id="3208a-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="3208a-111">**Element**</span></span>|<span data-ttu-id="3208a-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3208a-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3208a-113">UserResponse (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3208a-113">UserResponse (SOAP)</span></span>](userresponse-soap.md) <br/> |<span data-ttu-id="3208a-114">個々のユーザーの[Getusersettings 操作 (SOAP)](getusersettings-operation-soap.md)要求への応答を表します。</span><span class="sxs-lookup"><span data-stu-id="3208a-114">Represents a response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request for an individual user.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3208a-115">親要素</span><span class="sxs-lookup"><span data-stu-id="3208a-115">Parent elements</span></span>

|<span data-ttu-id="3208a-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="3208a-116">**Element**</span></span>|<span data-ttu-id="3208a-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="3208a-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3208a-118">応答 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3208a-118">Response (SOAP)</span></span>](response-soap.md) <br/> |<span data-ttu-id="3208a-119">[Getusersettings 操作 (SOAP)](getusersettings-operation-soap.md)要求への応答を格納します。</span><span class="sxs-lookup"><span data-stu-id="3208a-119">Contains the response to a [GetUserSettings operation (SOAP)](getusersettings-operation-soap.md) request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="3208a-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3208a-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3208a-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="3208a-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="3208a-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3208a-122">Schema Name</span></span>  <br/> |<span data-ttu-id="3208a-123">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="3208a-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="3208a-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3208a-124">Validation File</span></span>  <br/> |<span data-ttu-id="3208a-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3208a-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3208a-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3208a-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="3208a-127">正しい</span><span class="sxs-lookup"><span data-stu-id="3208a-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3208a-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="3208a-128">See also</span></span>



[<span data-ttu-id="3208a-129">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="3208a-129">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)

