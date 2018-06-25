---
title: 要求 (GetFederationInformation) (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: beeb5371-f57b-4346-9753-035dd42c6bee
description: 要求要素は、GetFederationInformationRequest (SOAP) 要求を表します。
ms.openlocfilehash: 0fb9301c2f318aa2c27155675dd3c43b41aabecd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833119"
---
# <a name="request-getfederationinformation-soap"></a><span data-ttu-id="2cd45-103">要求 (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2cd45-103">Request (GetFederationInformation) (SOAP)</span></span>

<span data-ttu-id="2cd45-104">**要求**要素は、 [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md)要求を表します。</span><span class="sxs-lookup"><span data-stu-id="2cd45-104">The **Request** element represents a [GetFederationInformationRequest (SOAP)](getfederationinformationrequest-soap.md) request.</span></span> 
  
```XML
<Request>
   <Domain/>
</Request>
```

 <span data-ttu-id="2cd45-105">**GetFederationInformationRequest**</span><span class="sxs-lookup"><span data-stu-id="2cd45-105">**GetFederationInformationRequest**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2cd45-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2cd45-106">Attributes and elements</span></span>

<span data-ttu-id="2cd45-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2cd45-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2cd45-108">属性</span><span class="sxs-lookup"><span data-stu-id="2cd45-108">Attributes</span></span>

<span data-ttu-id="2cd45-109">なし。</span><span class="sxs-lookup"><span data-stu-id="2cd45-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="2cd45-110">子要素</span><span class="sxs-lookup"><span data-stu-id="2cd45-110">Child elements</span></span>

|<span data-ttu-id="2cd45-111">**要素**</span><span class="sxs-lookup"><span data-stu-id="2cd45-111">**Element**</span></span>|<span data-ttu-id="2cd45-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="2cd45-112">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cd45-113">ドメイン (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2cd45-113">Domain (GetFederationInformation) (SOAP)</span></span>](domain-getfederationinformationsoap.md) <br/> |<span data-ttu-id="2cd45-114">フェデレーションの信頼されているドメインを識別します。</span><span class="sxs-lookup"><span data-stu-id="2cd45-114">Identifies the domain that has a federation trust.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2cd45-115">親要素</span><span class="sxs-lookup"><span data-stu-id="2cd45-115">Parent elements</span></span>

|<span data-ttu-id="2cd45-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="2cd45-116">**Element**</span></span>|<span data-ttu-id="2cd45-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="2cd45-117">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2cd45-118">GetFederationInformationRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="2cd45-118">GetFederationInformationRequestMessage (SOAP)</span></span>](getfederationinformationrequestmessage-soap.md) <br/> |<span data-ttu-id="2cd45-119">セキュリティ トークン サービス (STS) の構成データを要求するサーバーへの呼び出しを準備します。</span><span class="sxs-lookup"><span data-stu-id="2cd45-119">Prepares a call to the server to request configuration data for the security token service (STS).</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="2cd45-120">要素情報</span><span class="sxs-lookup"><span data-stu-id="2cd45-120">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2cd45-121">名前空間</span><span class="sxs-lookup"><span data-stu-id="2cd45-121">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="2cd45-122">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2cd45-122">Schema Name</span></span>  <br/> |<span data-ttu-id="2cd45-123">スキーマの自動検出</span><span class="sxs-lookup"><span data-stu-id="2cd45-123">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="2cd45-124">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2cd45-124">Validation File</span></span>  <br/> |<span data-ttu-id="2cd45-125">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2cd45-125">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2cd45-126">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2cd45-126">Can be Empty</span></span>  <br/> |<span data-ttu-id="2cd45-127">True</span><span class="sxs-lookup"><span data-stu-id="2cd45-127">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2cd45-128">関連項目</span><span class="sxs-lookup"><span data-stu-id="2cd45-128">See also</span></span>



[<span data-ttu-id="2cd45-129">自動検出を使用します。</span><span class="sxs-lookup"><span data-stu-id="2cd45-129">Working with Autodiscover</span></span>](http://msdn.microsoft.com/library/39726b67-2eb2-451b-9307-cfd0b518b55c%28Office.15%29.aspx)

