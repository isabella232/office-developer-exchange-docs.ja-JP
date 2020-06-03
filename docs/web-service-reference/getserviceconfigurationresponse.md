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
description: GetServiceConfigurationResponse 要素は、GetServiceConfiguration 要求に対する応答を定義します。
ms.openlocfilehash: ae74bc13a59e1c7a6a4ad0dbfddeea37671c52b0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460527"
---
# <a name="getserviceconfigurationresponse"></a><span data-ttu-id="f6256-103">GetServiceConfigurationResponse</span><span class="sxs-lookup"><span data-stu-id="f6256-103">GetServiceConfigurationResponse</span></span>

<span data-ttu-id="f6256-104">**GetServiceConfigurationResponse**要素は、GetServiceConfiguration 要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="f6256-104">The **GetServiceConfigurationResponse** element defines a response to a GetServiceConfiguration request.</span></span> 
  
```XML
<GetServiceConfigurationResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ResponseMessages/>
</GetServiceConfigurationResponse>
```

 <span data-ttu-id="f6256-105">**GetServiceConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f6256-105">**GetServiceConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f6256-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="f6256-106">Attributes and elements</span></span>

<span data-ttu-id="f6256-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f6256-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f6256-108">属性</span><span class="sxs-lookup"><span data-stu-id="f6256-108">Attributes</span></span>

|<span data-ttu-id="f6256-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="f6256-109">**Attribute**</span></span>|<span data-ttu-id="f6256-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="f6256-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f6256-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="f6256-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f6256-112">応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="f6256-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="f6256-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="f6256-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="f6256-114">-成功</span><span class="sxs-lookup"><span data-stu-id="f6256-114">-  Success</span></span>  <br/><span data-ttu-id="f6256-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="f6256-115">-  Warning</span></span>  <br/><span data-ttu-id="f6256-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="f6256-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f6256-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="f6256-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="f6256-118">**値**</span><span class="sxs-lookup"><span data-stu-id="f6256-118">**Value**</span></span>|<span data-ttu-id="f6256-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="f6256-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f6256-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="f6256-120">**Success**</span></span> <br/> |<span data-ttu-id="f6256-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="f6256-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f6256-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="f6256-122">**Warning**</span></span> <br/> | <span data-ttu-id="f6256-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="f6256-123">Describes a request that was not processed.</span></span> <span data-ttu-id="f6256-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f6256-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="f6256-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f6256-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="f6256-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="f6256-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="f6256-127">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="f6256-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="f6256-128">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="f6256-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="f6256-129">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="f6256-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="f6256-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="f6256-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="f6256-131">-クォータが限界を超えています。</span><span class="sxs-lookup"><span data-stu-id="f6256-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="f6256-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="f6256-132">**Error**</span></span> <br/> | <span data-ttu-id="f6256-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="f6256-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="f6256-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f6256-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="f6256-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="f6256-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="f6256-136">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="f6256-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="f6256-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="f6256-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="f6256-138">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="f6256-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="f6256-139">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="f6256-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="f6256-140">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="f6256-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="f6256-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f6256-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f6256-142">子要素</span><span class="sxs-lookup"><span data-stu-id="f6256-142">Child elements</span></span>

|<span data-ttu-id="f6256-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="f6256-143">**Element**</span></span>|<span data-ttu-id="f6256-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="f6256-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f6256-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="f6256-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f6256-146">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="f6256-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f6256-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f6256-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f6256-148">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="f6256-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f6256-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f6256-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f6256-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="f6256-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="f6256-151">この要素には0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f6256-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f6256-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f6256-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f6256-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="f6256-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f6256-154">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="f6256-154">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span></span>](responsemessages-arrayofserviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="f6256-155">サービス構成応答メッセージの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="f6256-155">Contains an array of service configuration response messages.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f6256-156">親要素</span><span class="sxs-lookup"><span data-stu-id="f6256-156">Parent elements</span></span>

<span data-ttu-id="f6256-157">なし。</span><span class="sxs-lookup"><span data-stu-id="f6256-157">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="f6256-158">テキスト値</span><span class="sxs-lookup"><span data-stu-id="f6256-158">Text value</span></span>

<span data-ttu-id="f6256-159">なし。</span><span class="sxs-lookup"><span data-stu-id="f6256-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f6256-160">注釈</span><span class="sxs-lookup"><span data-stu-id="f6256-160">Remarks</span></span>

<span data-ttu-id="f6256-161">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f6256-161">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f6256-162">要素の情報</span><span class="sxs-lookup"><span data-stu-id="f6256-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f6256-163">Namespace</span><span class="sxs-lookup"><span data-stu-id="f6256-163">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f6256-164">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f6256-164">Schema Name</span></span>  <br/> |<span data-ttu-id="f6256-165">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="f6256-165">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f6256-166">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f6256-166">Validation File</span></span>  <br/> |<span data-ttu-id="f6256-167">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="f6256-167">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f6256-168">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f6256-168">Can be Empty</span></span>  <br/> |<span data-ttu-id="f6256-169">正しくない</span><span class="sxs-lookup"><span data-stu-id="f6256-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f6256-170">関連項目</span><span class="sxs-lookup"><span data-stu-id="f6256-170">See also</span></span>

- [<span data-ttu-id="f6256-171">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="f6256-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

