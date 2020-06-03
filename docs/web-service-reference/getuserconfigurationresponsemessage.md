---
title: GetUserConfigurationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetUserConfigurationResponseMessage
api_type:
- schema
ms.assetid: f75e29eb-ae98-46fd-8da2-1c76a57f5458
description: GetUserConfigurationResponseMessage 要素は、ユーザー構成オブジェクトを返す応答を表します。
ms.openlocfilehash: 6aefa2364bfce9c3f928aedc4c018ebb3f85d28b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457691"
---
# <a name="getuserconfigurationresponsemessage"></a><span data-ttu-id="21b2c-103">GetUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="21b2c-103">GetUserConfigurationResponseMessage</span></span>

<span data-ttu-id="21b2c-104">**GetUserConfigurationResponseMessage**要素は、ユーザー構成オブジェクトを返す応答を表します。</span><span class="sxs-lookup"><span data-stu-id="21b2c-104">The **GetUserConfigurationResponseMessage** element represents a response that returns a user configuration object.</span></span> 
  
```xml
<GetUserConfigurationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <UserConfiguration/>
</GetUserConfigurationResponseMessage>
```

 <span data-ttu-id="21b2c-105">**GetUserConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="21b2c-105">**GetUserConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="21b2c-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="21b2c-106">Attributes and elements</span></span>

<span data-ttu-id="21b2c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="21b2c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="21b2c-108">属性</span><span class="sxs-lookup"><span data-stu-id="21b2c-108">Attributes</span></span>

|<span data-ttu-id="21b2c-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="21b2c-109">**Attribute**</span></span>|<span data-ttu-id="21b2c-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="21b2c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="21b2c-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="21b2c-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="21b2c-112">応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="21b2c-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="21b2c-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="21b2c-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="21b2c-114">-成功</span><span class="sxs-lookup"><span data-stu-id="21b2c-114">-  Success</span></span>  <br/><span data-ttu-id="21b2c-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="21b2c-115">-  Warning</span></span>  <br/><span data-ttu-id="21b2c-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="21b2c-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="21b2c-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="21b2c-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="21b2c-118">**値**</span><span class="sxs-lookup"><span data-stu-id="21b2c-118">**Value**</span></span>|<span data-ttu-id="21b2c-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="21b2c-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="21b2c-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="21b2c-120">**Success**</span></span> <br/> |<span data-ttu-id="21b2c-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="21b2c-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="21b2c-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="21b2c-122">**Warning**</span></span> <br/> | <span data-ttu-id="21b2c-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="21b2c-123">Describes a request that was not processed.</span></span> <span data-ttu-id="21b2c-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="21b2c-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="21b2c-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="21b2c-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="21b2c-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="21b2c-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="21b2c-127">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="21b2c-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="21b2c-128">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="21b2c-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="21b2c-129">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="21b2c-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="21b2c-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="21b2c-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="21b2c-131">-クォータが限界を超えています。</span><span class="sxs-lookup"><span data-stu-id="21b2c-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="21b2c-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="21b2c-132">**Error**</span></span> <br/> | <span data-ttu-id="21b2c-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="21b2c-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="21b2c-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="21b2c-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="21b2c-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="21b2c-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="21b2c-136">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="21b2c-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="21b2c-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="21b2c-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="21b2c-138">-コンテキスト内で属性または要素が無効です</span><span class="sxs-lookup"><span data-stu-id="21b2c-138">-  An attribute or element is not valid in the context</span></span>  <br/><span data-ttu-id="21b2c-139">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="21b2c-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="21b2c-140">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="21b2c-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="21b2c-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="21b2c-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="21b2c-142">子要素</span><span class="sxs-lookup"><span data-stu-id="21b2c-142">Child elements</span></span>

|<span data-ttu-id="21b2c-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="21b2c-143">**Element**</span></span>|<span data-ttu-id="21b2c-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="21b2c-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21b2c-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="21b2c-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="21b2c-146">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="21b2c-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="21b2c-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="21b2c-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="21b2c-148">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="21b2c-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="21b2c-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="21b2c-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="21b2c-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="21b2c-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="21b2c-151">この要素には0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="21b2c-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="21b2c-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="21b2c-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="21b2c-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="21b2c-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="21b2c-154">UserConfiguration</span><span class="sxs-lookup"><span data-stu-id="21b2c-154">UserConfiguration</span></span>](userconfiguration.md) <br/> |<span data-ttu-id="21b2c-155">1つのユーザー構成オブジェクトを格納します。</span><span class="sxs-lookup"><span data-stu-id="21b2c-155">Contains a single user configuration object.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="21b2c-156">親要素</span><span class="sxs-lookup"><span data-stu-id="21b2c-156">Parent elements</span></span>

|<span data-ttu-id="21b2c-157">**要素**</span><span class="sxs-lookup"><span data-stu-id="21b2c-157">**Element**</span></span>|<span data-ttu-id="21b2c-158">**説明**</span><span class="sxs-lookup"><span data-stu-id="21b2c-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="21b2c-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="21b2c-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="21b2c-160">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="21b2c-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="21b2c-161">テキスト値</span><span class="sxs-lookup"><span data-stu-id="21b2c-161">Text value</span></span>

<span data-ttu-id="21b2c-162">なし。</span><span class="sxs-lookup"><span data-stu-id="21b2c-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="21b2c-163">注釈</span><span class="sxs-lookup"><span data-stu-id="21b2c-163">Remarks</span></span>

<span data-ttu-id="21b2c-164">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="21b2c-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="21b2c-165">要素の情報</span><span class="sxs-lookup"><span data-stu-id="21b2c-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="21b2c-166">Namespace</span><span class="sxs-lookup"><span data-stu-id="21b2c-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="21b2c-167">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="21b2c-167">Schema Name</span></span>  <br/> |<span data-ttu-id="21b2c-168">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="21b2c-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="21b2c-169">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="21b2c-169">Validation File</span></span>  <br/> |<span data-ttu-id="21b2c-170">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="21b2c-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="21b2c-171">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="21b2c-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="21b2c-172">正しくない</span><span class="sxs-lookup"><span data-stu-id="21b2c-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="21b2c-173">関連項目</span><span class="sxs-lookup"><span data-stu-id="21b2c-173">See also</span></span>

- [<span data-ttu-id="21b2c-174">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="21b2c-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

