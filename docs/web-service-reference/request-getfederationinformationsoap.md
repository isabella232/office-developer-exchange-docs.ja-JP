---
title: Request (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: beeb5371-f57b-4346-9753-035dd42c6bee
description: Request 要素は、GetFederationInformationRequest (SOAP) 要求を表します。
ms.openlocfilehash: dbd88537d03f6325cf0025d08c63ae486544d705
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459582"
---
# <a name="request-getfederationinformation-soap"></a><span data-ttu-id="6a24d-103">Request (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6a24d-103">Request (GetFederationInformation) (SOAP)</span></span>

<span data-ttu-id="6a24d-104">**Request**要素は、 [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md)要求を表します。</span><span class="sxs-lookup"><span data-stu-id="6a24d-104">The **Request** element represents a [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md) request.</span></span> 
  
```XML
<Request>
   <Domain/>
</Request>
```

 <span data-ttu-id="6a24d-105">**GetFederationInformationRequest**</span><span class="sxs-lookup"><span data-stu-id="6a24d-105">**GetFederationInformationRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6a24d-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="6a24d-106">Attributes and elements</span></span>

<span data-ttu-id="6a24d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6a24d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6a24d-108">属性</span><span class="sxs-lookup"><span data-stu-id="6a24d-108">Attributes</span></span>

<span data-ttu-id="6a24d-109">なし。</span><span class="sxs-lookup"><span data-stu-id="6a24d-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="6a24d-110">子要素</span><span class="sxs-lookup"><span data-stu-id="6a24d-110">Child elements</span></span>

|<span data-ttu-id="6a24d-111">**Element**</span><span class="sxs-lookup"><span data-stu-id="6a24d-111">**Element**</span></span>|<span data-ttu-id="6a24d-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="6a24d-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a24d-113">ドメイン (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6a24d-113">Domain (GetFederationInformation) (SOAP)</span></span>](domain-getfederationinformationsoap.md) <br/> |<span data-ttu-id="6a24d-114">フェデレーション信頼があるドメインを識別します。</span><span class="sxs-lookup"><span data-stu-id="6a24d-114">Identifies the domain that has a federation trust.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6a24d-115">親要素</span><span class="sxs-lookup"><span data-stu-id="6a24d-115">Parent elements</span></span>

|<span data-ttu-id="6a24d-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="6a24d-116">**Element**</span></span>|<span data-ttu-id="6a24d-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="6a24d-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6a24d-118">GetFederationInformationRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="6a24d-118">GetFederationInformationRequestMessage (SOAP)</span></span>](getfederationinformationrequestmessage-soap.md) <br/> |<span data-ttu-id="6a24d-119">セキュリティトークンサービス (STS) の構成データを要求するために、サーバーへの呼び出しを準備します。</span><span class="sxs-lookup"><span data-stu-id="6a24d-119">Prepares a call to the server to request configuration data for the security token service (STS).</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="6a24d-120">要素の情報</span><span class="sxs-lookup"><span data-stu-id="6a24d-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6a24d-121">Namespace</span><span class="sxs-lookup"><span data-stu-id="6a24d-121">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="6a24d-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6a24d-122">Schema Name</span></span>  <br/> |<span data-ttu-id="6a24d-123">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="6a24d-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="6a24d-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6a24d-124">Validation File</span></span>  <br/> |<span data-ttu-id="6a24d-125">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="6a24d-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6a24d-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6a24d-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="6a24d-127">正しい</span><span class="sxs-lookup"><span data-stu-id="6a24d-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6a24d-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="6a24d-128">See also</span></span>



[<span data-ttu-id="6a24d-129">自動検出の使用</span><span class="sxs-lookup"><span data-stu-id="6a24d-129">Working with Autodiscover</span></span>](https://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)

