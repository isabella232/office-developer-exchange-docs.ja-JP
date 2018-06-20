---
title: GetServiceConfigurationResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServiceConfigurationResponse
api_type:
- schema
ms.assetid: 313dac99-0e5c-4198-bafa-89e749934ac7
description: GetServiceConfigurationResponse 要素は、GetServiceConfiguration 要求への応答を定義します。
ms.openlocfilehash: 7abc81222125334de2a6ab6e4a618b48fe0caf4f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831668"
---
# <a name="getserviceconfigurationresponse"></a><span data-ttu-id="b88e9-103">GetServiceConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="b88e9-103">GetServiceConfigurationResponse</span></span>

<span data-ttu-id="b88e9-104">**GetServiceConfigurationResponse**要素は、GetServiceConfiguration 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="b88e9-104">The **GetServiceConfigurationResponse** element defines a response to a GetServiceConfiguration request.</span></span> 
  
```XML
<GetServiceConfigurationResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ResponseMessages/>
</GetServiceConfigurationResponse>
```

 <span data-ttu-id="b88e9-105">**GetServiceConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b88e9-105">**GetServiceConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b88e9-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b88e9-106">Attributes and elements</span></span>

<span data-ttu-id="b88e9-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b88e9-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b88e9-108">属性</span><span class="sxs-lookup"><span data-stu-id="b88e9-108">Attributes</span></span>

|<span data-ttu-id="b88e9-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="b88e9-109">**Attribute**</span></span>|<span data-ttu-id="b88e9-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="b88e9-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b88e9-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="b88e9-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="b88e9-112">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b88e9-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="b88e9-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="b88e9-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="b88e9-114">-成功</span><span class="sxs-lookup"><span data-stu-id="b88e9-114">-  Success</span></span>  <br/><span data-ttu-id="b88e9-115">-警告</span><span class="sxs-lookup"><span data-stu-id="b88e9-115">-  Warning</span></span>  <br/><span data-ttu-id="b88e9-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="b88e9-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="b88e9-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="b88e9-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="b88e9-118">**値**</span><span class="sxs-lookup"><span data-stu-id="b88e9-118">**Value**</span></span>|<span data-ttu-id="b88e9-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="b88e9-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b88e9-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="b88e9-120">**Success**</span></span> <br/> |<span data-ttu-id="b88e9-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b88e9-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="b88e9-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="b88e9-122">**Warning**</span></span> <br/> | <span data-ttu-id="b88e9-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b88e9-123">Describes a request that was not processed.</span></span> <span data-ttu-id="b88e9-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="b88e9-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="b88e9-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b88e9-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="b88e9-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="b88e9-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="b88e9-127">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="b88e9-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="b88e9-128">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="b88e9-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="b88e9-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="b88e9-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="b88e9-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="b88e9-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="b88e9-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="b88e9-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="b88e9-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="b88e9-132">**Error**</span></span> <br/> | <span data-ttu-id="b88e9-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b88e9-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="b88e9-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="b88e9-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="b88e9-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="b88e9-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="b88e9-136">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="b88e9-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="b88e9-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="b88e9-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="b88e9-138">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="b88e9-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="b88e9-139">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="b88e9-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="b88e9-140">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="b88e9-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="b88e9-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="b88e9-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b88e9-142">子要素</span><span class="sxs-lookup"><span data-stu-id="b88e9-142">Child elements</span></span>

|<span data-ttu-id="b88e9-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="b88e9-143">**Element**</span></span>|<span data-ttu-id="b88e9-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="b88e9-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b88e9-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="b88e9-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b88e9-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="b88e9-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b88e9-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b88e9-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b88e9-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="b88e9-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="b88e9-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b88e9-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b88e9-150">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="b88e9-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="b88e9-151">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b88e9-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b88e9-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b88e9-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b88e9-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="b88e9-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="b88e9-154">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="b88e9-154">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span></span>](responsemessages-arrayofserviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="b88e9-155">サービス構成の応答メッセージの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b88e9-155">Contains an array of service configuration response messages.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b88e9-156">親要素</span><span class="sxs-lookup"><span data-stu-id="b88e9-156">Parent elements</span></span>

<span data-ttu-id="b88e9-157">なし。</span><span class="sxs-lookup"><span data-stu-id="b88e9-157">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="b88e9-158">テキスト値</span><span class="sxs-lookup"><span data-stu-id="b88e9-158">Text value</span></span>

<span data-ttu-id="b88e9-159">なし。</span><span class="sxs-lookup"><span data-stu-id="b88e9-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="b88e9-160">備考</span><span class="sxs-lookup"><span data-stu-id="b88e9-160">Remarks</span></span>

<span data-ttu-id="b88e9-161">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="b88e9-161">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b88e9-162">要素情報</span><span class="sxs-lookup"><span data-stu-id="b88e9-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b88e9-163">名前空間</span><span class="sxs-lookup"><span data-stu-id="b88e9-163">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b88e9-164">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b88e9-164">Schema Name</span></span>  <br/> |<span data-ttu-id="b88e9-165">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="b88e9-165">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b88e9-166">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b88e9-166">Validation File</span></span>  <br/> |<span data-ttu-id="b88e9-167">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b88e9-167">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b88e9-168">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b88e9-168">Can be Empty</span></span>  <br/> |<span data-ttu-id="b88e9-169">False</span><span class="sxs-lookup"><span data-stu-id="b88e9-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b88e9-170">関連項目</span><span class="sxs-lookup"><span data-stu-id="b88e9-170">See also</span></span>

- [<span data-ttu-id="b88e9-171">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="b88e9-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

