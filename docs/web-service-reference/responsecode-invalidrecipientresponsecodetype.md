---
title: 応答 Secmode (Invalid受信者応答 Secodetype)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseCode
api_type:
- schema
ms.assetid: 582e9caa-d2bc-4be1-a460-739294f9ef18
description: 応答 Secな要素は、受信者が無効である理由についての情報を提供します。
ms.openlocfilehash: d78de64de7725007ec51a55dad13d1cc892a25e6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529722"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a><span data-ttu-id="8f5cd-103">応答 Secmode (Invalid受信者応答 Secodetype)</span><span class="sxs-lookup"><span data-stu-id="8f5cd-103">ResponseCode (InvalidRecipientResponseCodeType)</span></span>

<span data-ttu-id="8f5cd-104">応答**secな**要素は、受信者が無効である理由についての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="8f5cd-104">The **ResponseCode** element provides information about why the recipient is invalid.</span></span> 
  
```XML
<ResponseCode>OtherError or RecipientOrganizationNotFederated or CannotObtainTokenFromSTS or SystemPolicyBlocksSharingWithThisRecipient or RecipientOrganizationFederatedWithUnknownTokenIssuer</ResponseCode>
```

 <span data-ttu-id="8f5cd-105">**Invalid受信者応答 Secodetype**</span><span class="sxs-lookup"><span data-stu-id="8f5cd-105">**InvalidRecipientResponseCodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8f5cd-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8f5cd-106">Attributes and elements</span></span>

<span data-ttu-id="8f5cd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8f5cd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8f5cd-108">属性</span><span class="sxs-lookup"><span data-stu-id="8f5cd-108">Attributes</span></span>

<span data-ttu-id="8f5cd-109">なし。</span><span class="sxs-lookup"><span data-stu-id="8f5cd-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="8f5cd-110">子要素</span><span class="sxs-lookup"><span data-stu-id="8f5cd-110">Child elements</span></span>

<span data-ttu-id="8f5cd-111">なし。</span><span class="sxs-lookup"><span data-stu-id="8f5cd-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="8f5cd-112">親要素</span><span class="sxs-lookup"><span data-stu-id="8f5cd-112">Parent elements</span></span>

|<span data-ttu-id="8f5cd-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="8f5cd-113">**Element**</span></span>|<span data-ttu-id="8f5cd-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="8f5cd-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f5cd-115">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="8f5cd-115">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="8f5cd-116">無効な受信者の SMTP アドレスと、受信者が無効である理由についての情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="8f5cd-116">Contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8f5cd-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8f5cd-117">Text value</span></span>

<span data-ttu-id="8f5cd-118">次の表**に、指定**できる値を示します。</span><span class="sxs-lookup"><span data-stu-id="8f5cd-118">The following table lists the possible values for the **ResponseCode** element.</span></span> 
  
|<span data-ttu-id="8f5cd-119">**コード**</span><span class="sxs-lookup"><span data-stu-id="8f5cd-119">**Code**</span></span>|<span data-ttu-id="8f5cd-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="8f5cd-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8f5cd-121">OtherError</span><span class="sxs-lookup"><span data-stu-id="8f5cd-121">OtherError</span></span>  <br/> |<span data-ttu-id="8f5cd-122">エラーが別のエラー応答コードによって指定されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="8f5cd-122">Indicates that the error is not specified by another error response code.</span></span>  <br/> |
|<span data-ttu-id="8f5cd-123">受信者組織のフェデレーション</span><span class="sxs-lookup"><span data-stu-id="8f5cd-123">RecipientOrganizationNotFederated</span></span>  <br/> |<span data-ttu-id="8f5cd-124">受信者の SMTP 電子メールアドレスで指定されている組織との共有関係が使用できないことを示します。</span><span class="sxs-lookup"><span data-stu-id="8f5cd-124">Indicates that a sharing relationship is not available with the organization specified in the recipient's SMTP e-mail address.</span></span>  <br/> |
|<span data-ttu-id="8f5cd-125">CannotObtainTokenFromSTS</span><span class="sxs-lookup"><span data-stu-id="8f5cd-125">CannotObtainTokenFromSTS</span></span>  <br/> |<span data-ttu-id="8f5cd-126">トークンサーバーからセキュリティトークンを取得するときに問題が発生したことを示します。</span><span class="sxs-lookup"><span data-stu-id="8f5cd-126">Indicates that there was a problem obtaining a security token from the token server.</span></span>  <br/> |
|<span data-ttu-id="8f5cd-127">Systempolicyblockssharingwithrecipient</span><span class="sxs-lookup"><span data-stu-id="8f5cd-127">SystemPolicyBlocksSharingWithThisRecipient</span></span>  <br/> |<span data-ttu-id="8f5cd-128">システム管理者が、指定された受信者との共有をブロックするシステムポリシーを設定したことを示します。</span><span class="sxs-lookup"><span data-stu-id="8f5cd-128">Indicates that the system administrator has set a system policy that blocks sharing with the specified recipient.</span></span>  <br/> |
|<span data-ttu-id="8f5cd-129">RecipientOrganizationFederatedWithUnknownTokenIssuer</span><span class="sxs-lookup"><span data-stu-id="8f5cd-129">RecipientOrganizationFederatedWithUnknownTokenIssuer</span></span>  <br/> |<span data-ttu-id="8f5cd-130">指定した受信者が使用する secure token service が不明であることを示します。</span><span class="sxs-lookup"><span data-stu-id="8f5cd-130">Indicates that the secure token service that is used by the specified recipient is unknown.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8f5cd-131">注釈</span><span class="sxs-lookup"><span data-stu-id="8f5cd-131">Remarks</span></span>

<span data-ttu-id="8f5cd-132">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8f5cd-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8f5cd-133">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8f5cd-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8f5cd-134">Namespace</span><span class="sxs-lookup"><span data-stu-id="8f5cd-134">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="8f5cd-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8f5cd-135">Schema Name</span></span>  <br/> |<span data-ttu-id="8f5cd-136">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="8f5cd-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="8f5cd-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8f5cd-137">Validation File</span></span>  <br/> |<span data-ttu-id="8f5cd-138">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="8f5cd-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="8f5cd-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8f5cd-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="8f5cd-140">正しくない</span><span class="sxs-lookup"><span data-stu-id="8f5cd-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8f5cd-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="8f5cd-141">See also</span></span>



[<span data-ttu-id="8f5cd-142">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="8f5cd-142">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="8f5cd-143">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8f5cd-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

