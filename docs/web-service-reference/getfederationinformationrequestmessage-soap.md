---
title: GetFederationInformationRequestMessage (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 3b0f5841-0c8f-4a9d-be75-cdf6cc2c35ab
description: GetFederationInformationRequestMessage 要素は、セキュリティトークンサービス (STS) の構成データを要求するために、サーバーへの呼び出しを準備します。
ms.openlocfilehash: cc1e4d67f5bba6e571aeb94d3f27b67baac4c224
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467026"
---
# <a name="getfederationinformationrequestmessage-soap"></a><span data-ttu-id="468e2-103">GetFederationInformationRequestMessage (SOAP)</span><span class="sxs-lookup"><span data-stu-id="468e2-103">GetFederationInformationRequestMessage (SOAP)</span></span>

<span data-ttu-id="468e2-104">**GetFederationInformationRequestMessage**要素は、セキュリティトークンサービス (STS) の構成データを要求するために、サーバーへの呼び出しを準備します。</span><span class="sxs-lookup"><span data-stu-id="468e2-104">The **GetFederationInformationRequestMessage** element prepares a call to the server to request configuration data for the security token service (STS).</span></span> 
  
```XML
<GetFederationInformationRequestMessage>
   <Request/>
</GetFederationInformationRequestMessage>

```

## <a name="attributes-and-elements"></a><span data-ttu-id="468e2-105">属性と要素</span><span class="sxs-lookup"><span data-stu-id="468e2-105">Attributes and elements</span></span>

<span data-ttu-id="468e2-106">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="468e2-106">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="468e2-107">属性</span><span class="sxs-lookup"><span data-stu-id="468e2-107">Attributes</span></span>

<span data-ttu-id="468e2-108">なし。</span><span class="sxs-lookup"><span data-stu-id="468e2-108">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="468e2-109">子要素</span><span class="sxs-lookup"><span data-stu-id="468e2-109">Child elements</span></span>

|<span data-ttu-id="468e2-110">**Element**</span><span class="sxs-lookup"><span data-stu-id="468e2-110">**Element**</span></span>|<span data-ttu-id="468e2-111">**説明**</span><span class="sxs-lookup"><span data-stu-id="468e2-111">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="468e2-112">Request (GetFederationInformation) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="468e2-112">Request (GetFederationInformation) (SOAP)</span></span>](request-getfederationinformationsoap.md) <br/> |<span data-ttu-id="468e2-113">**GetFederationInformation**要求を表します。</span><span class="sxs-lookup"><span data-stu-id="468e2-113">Represents a **GetFederationInformation** request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="468e2-114">親要素</span><span class="sxs-lookup"><span data-stu-id="468e2-114">Parent elements</span></span>

<span data-ttu-id="468e2-115">なし。</span><span class="sxs-lookup"><span data-stu-id="468e2-115">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="468e2-116">テキスト値</span><span class="sxs-lookup"><span data-stu-id="468e2-116">Text value</span></span>

<span data-ttu-id="468e2-117">なし。</span><span class="sxs-lookup"><span data-stu-id="468e2-117">None.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="468e2-118">要素の情報</span><span class="sxs-lookup"><span data-stu-id="468e2-118">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="468e2-119">Namespace</span><span class="sxs-lookup"><span data-stu-id="468e2-119">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="468e2-120">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="468e2-120">Schema Name</span></span>  <br/> |<span data-ttu-id="468e2-121">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="468e2-121">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="468e2-122">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="468e2-122">Validation File</span></span>  <br/> |<span data-ttu-id="468e2-123">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="468e2-123">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="468e2-124">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="468e2-124">Can be Empty</span></span>  <br/> |<span data-ttu-id="468e2-125">正しい</span><span class="sxs-lookup"><span data-stu-id="468e2-125">True</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="468e2-126">関連項目</span><span class="sxs-lookup"><span data-stu-id="468e2-126">See also</span></span>



[<span data-ttu-id="468e2-127">GetFederationInformation 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="468e2-127">GetFederationInformation operation (SOAP)</span></span>](getfederationinformation-operation-soap.md)

