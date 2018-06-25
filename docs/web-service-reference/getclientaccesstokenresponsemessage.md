---
title: GetClientAccessTokenResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 45ca2500-ceab-4c98-9576-cb9e158e5896
description: GetClientAccessTokenResponseMessage 要素は、GetClientAccessToken 要求の応答メッセージを指定します。
ms.openlocfilehash: 16fe684dd48f77156ed88d02a6ae7b8f3312cd87
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760656"
---
# <a name="getclientaccesstokenresponsemessage"></a><span data-ttu-id="fa998-103">GetClientAccessTokenResponseMessage</span><span class="sxs-lookup"><span data-stu-id="fa998-103">GetClientAccessTokenResponseMessage</span></span>

<span data-ttu-id="fa998-104">**GetClientAccessTokenResponseMessage**要素は、 **GetClientAccessToken**要求の応答メッセージを指定します。</span><span class="sxs-lookup"><span data-stu-id="fa998-104">The **GetClientAccessTokenResponseMessage** element specifies the response message for a **GetClientAccessToken** request.</span></span> 
  
```XML
<GetClientAccessTokenResponseMessage ResponseClass=" Success | Warning | Error ">
    <Token/>
    <MessageText/>
    <ResponseCode/>
    <DescriptiveLinkKey/>
    <MessageXml/>
</GetClientAccessTokenResponseMessage>
```

 <span data-ttu-id="fa998-105">**GetClientAccessTokenResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="fa998-105">**GetClientAccessTokenResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="fa998-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="fa998-106">Attributes and elements</span></span>

<span data-ttu-id="fa998-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="fa998-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="fa998-108">属性</span><span class="sxs-lookup"><span data-stu-id="fa998-108">Attributes</span></span>

|<span data-ttu-id="fa998-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="fa998-109">**Attribute**</span></span>|<span data-ttu-id="fa998-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="fa998-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fa998-111">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="fa998-111">ResponseClass</span></span>  <br/> |<span data-ttu-id="fa998-112">応答のクラスを示します。</span><span class="sxs-lookup"><span data-stu-id="fa998-112">Indicates the class of the response.</span></span>  <br/> |
   
#### <a name="responseclass"></a><span data-ttu-id="fa998-113">ResponseClass</span><span class="sxs-lookup"><span data-stu-id="fa998-113">ResponseClass</span></span>

|<span data-ttu-id="fa998-114">**値**</span><span class="sxs-lookup"><span data-stu-id="fa998-114">**Value**</span></span>|<span data-ttu-id="fa998-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="fa998-115">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="fa998-116">成功</span><span class="sxs-lookup"><span data-stu-id="fa998-116">Success</span></span>  <br/> |<span data-ttu-id="fa998-117">成功を示します。</span><span class="sxs-lookup"><span data-stu-id="fa998-117">Indicates success.</span></span>  <br/> |
|<span data-ttu-id="fa998-118">警告</span><span class="sxs-lookup"><span data-stu-id="fa998-118">Warning</span></span>  <br/> |<span data-ttu-id="fa998-119">警告を示します。</span><span class="sxs-lookup"><span data-stu-id="fa998-119">Indicates a warning.</span></span>  <br/> |
|<span data-ttu-id="fa998-120">エラー</span><span class="sxs-lookup"><span data-stu-id="fa998-120">Error</span></span>  <br/> |<span data-ttu-id="fa998-121">エラーを示します。</span><span class="sxs-lookup"><span data-stu-id="fa998-121">Indicates an error.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="fa998-122">子要素</span><span class="sxs-lookup"><span data-stu-id="fa998-122">Child elements</span></span>

|<span data-ttu-id="fa998-123">**要素**</span><span class="sxs-lookup"><span data-stu-id="fa998-123">**Element**</span></span>|<span data-ttu-id="fa998-124">**説明**</span><span class="sxs-lookup"><span data-stu-id="fa998-124">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa998-125">トークン (ClientAccessTokenType)</span><span class="sxs-lookup"><span data-stu-id="fa998-125">Token (ClientAccessTokenType)</span></span>](token-clientaccesstokentype.md) <br/> |<span data-ttu-id="fa998-126">クライアントのアクセス トークンを指定します。</span><span class="sxs-lookup"><span data-stu-id="fa998-126">Specifies a client access token.</span></span>  <br/> |
|[<span data-ttu-id="fa998-127">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="fa998-127">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="fa998-128">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="fa998-128">Currently unused and reserved for future use.</span></span>  <br/> |
|[<span data-ttu-id="fa998-129">MessageText</span><span class="sxs-lookup"><span data-stu-id="fa998-129">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="fa998-130">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="fa998-130">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="fa998-131">MessageXml</span><span class="sxs-lookup"><span data-stu-id="fa998-131">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="fa998-132">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="fa998-132">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="fa998-133">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="fa998-133">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="fa998-134">要求に関するステータス情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="fa998-134">Provides status information about the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="fa998-135">親要素</span><span class="sxs-lookup"><span data-stu-id="fa998-135">Parent elements</span></span>

|<span data-ttu-id="fa998-136">**要素**</span><span class="sxs-lookup"><span data-stu-id="fa998-136">**Element**</span></span>|<span data-ttu-id="fa998-137">**説明**</span><span class="sxs-lookup"><span data-stu-id="fa998-137">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="fa998-138">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="fa998-138">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="fa998-139">Exchange Web サービス (EWS) 要求の応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="fa998-139">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="fa998-140">備考</span><span class="sxs-lookup"><span data-stu-id="fa998-140">Remarks</span></span>

<span data-ttu-id="fa998-141">この要素は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="fa998-141">This element was introduced in Exchange Server 2013.</span></span>
  
<span data-ttu-id="fa998-142">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="fa998-142">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="fa998-143">要素情報</span><span class="sxs-lookup"><span data-stu-id="fa998-143">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="fa998-144">名前空間</span><span class="sxs-lookup"><span data-stu-id="fa998-144">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="fa998-145">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="fa998-145">Schema Name</span></span>  <br/> |<span data-ttu-id="fa998-146">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="fa998-146">Message schema</span></span>  <br/> |
|<span data-ttu-id="fa998-147">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="fa998-147">Validation File</span></span>  <br/> |<span data-ttu-id="fa998-148">messages.xsd</span><span class="sxs-lookup"><span data-stu-id="fa998-148">messages.xsd</span></span>  <br/> |
|<span data-ttu-id="fa998-149">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="fa998-149">Can Be Empty</span></span>  <br/> ||
   
## <a name="see-also"></a><span data-ttu-id="fa998-150">関連項目</span><span class="sxs-lookup"><span data-stu-id="fa998-150">See also</span></span>



- [<span data-ttu-id="fa998-151">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="fa998-151">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

