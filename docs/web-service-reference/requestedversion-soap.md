---
title: RequestedVersion (SOAP)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
localization_priority: Normal
api_type:
- schema
ms.assetid: 962036c9-9b13-4669-bed2-2502c0f5aabe
description: RequestedVersion 要素は、クライアントが要求を処理する必要のある最小サービスバージョンを指定します。
ms.openlocfilehash: ded276b3eb2c70b6edd39ca12289098de2b3faea
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459168"
---
# <a name="requestedversion-soap"></a><span data-ttu-id="51aec-103">RequestedVersion (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51aec-103">RequestedVersion (SOAP)</span></span>

<span data-ttu-id="51aec-104">**Requestedversion**要素は、クライアントが要求を処理する必要のある最小サービスバージョンを指定します。</span><span class="sxs-lookup"><span data-stu-id="51aec-104">The **RequestedVersion** element specifies the minimum service version that the client wants the request to be processed on.</span></span> 
  
```XML
<RequestedVersion/>
```

 <span data-ttu-id="51aec-105">**ExchangeVersion**</span><span class="sxs-lookup"><span data-stu-id="51aec-105">**ExchangeVersion**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="51aec-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="51aec-106">Attributes and elements</span></span>

<span data-ttu-id="51aec-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="51aec-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="51aec-108">属性</span><span class="sxs-lookup"><span data-stu-id="51aec-108">Attributes</span></span>

<span data-ttu-id="51aec-109">なし。</span><span class="sxs-lookup"><span data-stu-id="51aec-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="51aec-110">子要素</span><span class="sxs-lookup"><span data-stu-id="51aec-110">Child elements</span></span>

<span data-ttu-id="51aec-111">なし。</span><span class="sxs-lookup"><span data-stu-id="51aec-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="51aec-112">親要素</span><span class="sxs-lookup"><span data-stu-id="51aec-112">Parent elements</span></span>

|<span data-ttu-id="51aec-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="51aec-113">**Element**</span></span>|<span data-ttu-id="51aec-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="51aec-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="51aec-115">要求 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51aec-115">Request (SOAP)</span></span>](request-soap.md) <br/> |<span data-ttu-id="51aec-116">要求された構成設定と対象ユーザーが含まれます。</span><span class="sxs-lookup"><span data-stu-id="51aec-116">Contains the requested configuration settings and the target users.</span></span>  <br/> |
|[<span data-ttu-id="51aec-117">Request (GetDomainSettings) (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51aec-117">Request (GetDomainSettings) (SOAP)</span></span>](request-getdomainsettingssoap.md) <br/> |<span data-ttu-id="51aec-118">ドメイン設定を取得するための要求を表します。</span><span class="sxs-lookup"><span data-stu-id="51aec-118">Represents a request to get domain settings.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="51aec-119">テキスト値</span><span class="sxs-lookup"><span data-stu-id="51aec-119">Text value</span></span>

<span data-ttu-id="51aec-120">**Requestedversion**要素のテキスト値には、Exchange2010、Exchange2010_SP1、Exchange2010_SP2、または Exchange2013 を指定できます。</span><span class="sxs-lookup"><span data-stu-id="51aec-120">The text value for the **RequestedVersion** element can be Exchange2010, Exchange2010_SP1, Exchange2010_SP2, or Exchange2013.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="51aec-121">注釈</span><span class="sxs-lookup"><span data-stu-id="51aec-121">Remarks</span></span>

<span data-ttu-id="51aec-122">この要素が存在しない場合は、最新のサービスバージョンが使用されます。</span><span class="sxs-lookup"><span data-stu-id="51aec-122">If this element is not present, the latest service version is used.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="51aec-123">要素の情報</span><span class="sxs-lookup"><span data-stu-id="51aec-123">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="51aec-124">Namespace</span><span class="sxs-lookup"><span data-stu-id="51aec-124">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/2010/Autodiscover  <br/> |
|<span data-ttu-id="51aec-125">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="51aec-125">Schema Name</span></span>  <br/> |<span data-ttu-id="51aec-126">自動検出スキーマ</span><span class="sxs-lookup"><span data-stu-id="51aec-126">Autodiscover schema</span></span>  <br/> |
|<span data-ttu-id="51aec-127">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="51aec-127">Validation File</span></span>  <br/> |<span data-ttu-id="51aec-128">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="51aec-128">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="51aec-129">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="51aec-129">Can be Empty</span></span>  <br/> |<span data-ttu-id="51aec-130">正しくない</span><span class="sxs-lookup"><span data-stu-id="51aec-130">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="51aec-131">関連項目</span><span class="sxs-lookup"><span data-stu-id="51aec-131">See also</span></span>



[<span data-ttu-id="51aec-132">GetUserSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51aec-132">GetUserSettings operation (SOAP)</span></span>](getusersettings-operation-soap.md)
  
[<span data-ttu-id="51aec-133">GetDomainSettings 操作 (SOAP)</span><span class="sxs-lookup"><span data-stu-id="51aec-133">GetDomainSettings operation (SOAP)</span></span>](getdomainsettings-operation-soap.md)

