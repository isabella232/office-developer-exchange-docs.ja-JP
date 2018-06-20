---
title: ResponseCode (InvalidRecipientResponseCodeType)
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
description: ResponseCode 要素は、受信者が有効な理由についての情報を提供します。
ms.openlocfilehash: 3bff99dd1ac6603ce31d5ceb074e73ef48190bb2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833186"
---
# <a name="responsecode-invalidrecipientresponsecodetype"></a><span data-ttu-id="9cebc-103">ResponseCode (InvalidRecipientResponseCodeType)</span><span class="sxs-lookup"><span data-stu-id="9cebc-103">ResponseCode (InvalidRecipientResponseCodeType)</span></span>

<span data-ttu-id="9cebc-104">**ResponseCode**要素は、受信者が有効な理由についての情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="9cebc-104">The **ResponseCode** element provides information about why the recipient is invalid.</span></span> 
  
```XML
<ResponseCode>OtherError or RecipientOrganizationNotFederated or CannotObtainTokenFromSTS or SystemPolicyBlocksSharingWithThisRecipient or RecipientOrganizationFederatedWithUnknownTokenIssuer</ResponseCode>
```

 <span data-ttu-id="9cebc-105">**InvalidRecipientResponseCodeType**</span><span class="sxs-lookup"><span data-stu-id="9cebc-105">**InvalidRecipientResponseCodeType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9cebc-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9cebc-106">Attributes and elements</span></span>

<span data-ttu-id="9cebc-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9cebc-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9cebc-108">属性</span><span class="sxs-lookup"><span data-stu-id="9cebc-108">Attributes</span></span>

<span data-ttu-id="9cebc-109">なし。</span><span class="sxs-lookup"><span data-stu-id="9cebc-109">None.</span></span>
  
### <a name="child-elements"></a><span data-ttu-id="9cebc-110">子要素</span><span class="sxs-lookup"><span data-stu-id="9cebc-110">Child elements</span></span>

<span data-ttu-id="9cebc-111">なし。</span><span class="sxs-lookup"><span data-stu-id="9cebc-111">None.</span></span>
  
### <a name="parent-elements"></a><span data-ttu-id="9cebc-112">親要素</span><span class="sxs-lookup"><span data-stu-id="9cebc-112">Parent elements</span></span>

|<span data-ttu-id="9cebc-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="9cebc-113">**Element**</span></span>|<span data-ttu-id="9cebc-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="9cebc-114">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9cebc-115">InvalidRecipient</span><span class="sxs-lookup"><span data-stu-id="9cebc-115">InvalidRecipient</span></span>](invalidrecipient.md) <br/> |<span data-ttu-id="9cebc-116">受信者が有効な理由については、無効な受信者の SMTP アドレスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9cebc-116">Contains the SMTP address of the invalid recipient and information about why the recipient is invalid.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9cebc-117">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9cebc-117">Text value</span></span>

<span data-ttu-id="9cebc-118">次の表は、 **ResponseCode**要素の値を一覧します。</span><span class="sxs-lookup"><span data-stu-id="9cebc-118">The following table lists the possible values for the **ResponseCode** element.</span></span> 
  
|<span data-ttu-id="9cebc-119">**コード**</span><span class="sxs-lookup"><span data-stu-id="9cebc-119">**Code**</span></span>|<span data-ttu-id="9cebc-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="9cebc-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9cebc-121">OtherError</span><span class="sxs-lookup"><span data-stu-id="9cebc-121">OtherError</span></span>  <br/> |<span data-ttu-id="9cebc-122">エラーが、別のエラー応答コードが指定されていないことを示します。</span><span class="sxs-lookup"><span data-stu-id="9cebc-122">Indicates that the error is not specified by another error response code.</span></span>  <br/> |
|<span data-ttu-id="9cebc-123">RecipientOrganizationNotFederated</span><span class="sxs-lookup"><span data-stu-id="9cebc-123">RecipientOrganizationNotFederated</span></span>  <br/> |<span data-ttu-id="9cebc-124">共有関係は利用できない受信者の SMTP 電子メール アドレスで指定された組織のことを示します。</span><span class="sxs-lookup"><span data-stu-id="9cebc-124">Indicates that a sharing relationship is not available with the organization specified in the recipient's SMTP e-mail address.</span></span>  <br/> |
|<span data-ttu-id="9cebc-125">CannotObtainTokenFromSTS</span><span class="sxs-lookup"><span data-stu-id="9cebc-125">CannotObtainTokenFromSTS</span></span>  <br/> |<span data-ttu-id="9cebc-126">トークン サーバからセキュリティ トークンの取得に問題があったことを示します。</span><span class="sxs-lookup"><span data-stu-id="9cebc-126">Indicates that there was a problem obtaining a security token from the token server.</span></span>  <br/> |
|<span data-ttu-id="9cebc-127">SystemPolicyBlocksSharingWithThisRecipient</span><span class="sxs-lookup"><span data-stu-id="9cebc-127">SystemPolicyBlocksSharingWithThisRecipient</span></span>  <br/> |<span data-ttu-id="9cebc-128">システム管理者が指定された受信者との共有をブロックするシステム ポリシーを設定することを示します。</span><span class="sxs-lookup"><span data-stu-id="9cebc-128">Indicates that the system administrator has set a system policy that blocks sharing with the specified recipient.</span></span>  <br/> |
|<span data-ttu-id="9cebc-129">RecipientOrganizationFederatedWithUnknownTokenIssuer</span><span class="sxs-lookup"><span data-stu-id="9cebc-129">RecipientOrganizationFederatedWithUnknownTokenIssuer</span></span>  <br/> |<span data-ttu-id="9cebc-130">指定された受信者によって使用されるセキュリティ トークン サービスが正常であることを示します。</span><span class="sxs-lookup"><span data-stu-id="9cebc-130">Indicates that the secure token service that is used by the specified recipient is unknown.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="9cebc-131">備考</span><span class="sxs-lookup"><span data-stu-id="9cebc-131">Remarks</span></span>

<span data-ttu-id="9cebc-132">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9cebc-132">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9cebc-133">要素情報</span><span class="sxs-lookup"><span data-stu-id="9cebc-133">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9cebc-134">名前空間</span><span class="sxs-lookup"><span data-stu-id="9cebc-134">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="9cebc-135">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9cebc-135">Schema Name</span></span>  <br/> |<span data-ttu-id="9cebc-136">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="9cebc-136">Types schema</span></span>  <br/> |
|<span data-ttu-id="9cebc-137">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9cebc-137">Validation File</span></span>  <br/> |<span data-ttu-id="9cebc-138">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="9cebc-138">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="9cebc-139">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9cebc-139">Can be Empty</span></span>  <br/> |<span data-ttu-id="9cebc-140">False</span><span class="sxs-lookup"><span data-stu-id="9cebc-140">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9cebc-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="9cebc-141">See also</span></span>



[<span data-ttu-id="9cebc-142">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="9cebc-142">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)


- [<span data-ttu-id="9cebc-143">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9cebc-143">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

