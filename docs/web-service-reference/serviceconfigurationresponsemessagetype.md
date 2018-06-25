---
title: ServiceConfigurationResponseMessageType
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ServiceConfigurationResponseMessageType
api_type:
- schema
ms.assetid: ccfb0578-c648-44c2-ac4d-7620d881363e
description: ServiceConfigurationResponseMessageType 要素には、サービスの構成設定が含まれています。
ms.openlocfilehash: fb7841f346083017319cece4479fea8bbfb6de17
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833393"
---
# <a name="serviceconfigurationresponsemessagetype"></a><span data-ttu-id="30de1-103">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="30de1-103">ServiceConfigurationResponseMessageType</span></span>

<span data-ttu-id="30de1-104">**ServiceConfigurationResponseMessageType**要素には、サービスの構成設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="30de1-104">The **ServiceConfigurationResponseMessageType** element contains service configuration settings.</span></span> 
  
```XML
<ServiceConfigurationResponseMessageType ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailTipsConfiguration/>
   <UnifiedMessagingConfiguration/>
   <ProtectionRulesConfiguration/>
</ServiceConfigurationResponseMessageType>
```

 <span data-ttu-id="30de1-105">**ServiceConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="30de1-105">**ServiceConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="30de1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="30de1-106">Attributes and elements</span></span>

<span data-ttu-id="30de1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="30de1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="30de1-108">属性</span><span class="sxs-lookup"><span data-stu-id="30de1-108">Attributes</span></span>

|<span data-ttu-id="30de1-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="30de1-109">**Attribute**</span></span>|<span data-ttu-id="30de1-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="30de1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="30de1-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="30de1-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="30de1-112">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="30de1-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="30de1-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="30de1-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="30de1-114">-成功</span><span class="sxs-lookup"><span data-stu-id="30de1-114">-  Success</span></span>  <br/><span data-ttu-id="30de1-115">-警告</span><span class="sxs-lookup"><span data-stu-id="30de1-115">-  Warning</span></span>  <br/><span data-ttu-id="30de1-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="30de1-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="30de1-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="30de1-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="30de1-118">**値**</span><span class="sxs-lookup"><span data-stu-id="30de1-118">**Value**</span></span>|<span data-ttu-id="30de1-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="30de1-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="30de1-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="30de1-120">**Success**</span></span> <br/> |<span data-ttu-id="30de1-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="30de1-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="30de1-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="30de1-122">**Warning**</span></span> <br/> | <span data-ttu-id="30de1-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="30de1-123">Describes a request that was not processed.</span></span> <span data-ttu-id="30de1-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="30de1-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="30de1-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="30de1-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="30de1-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="30de1-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="30de1-127">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="30de1-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="30de1-128">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="30de1-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="30de1-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="30de1-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="30de1-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="30de1-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="30de1-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="30de1-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="30de1-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="30de1-132">**Error**</span></span> <br/> | <span data-ttu-id="30de1-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="30de1-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="30de1-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="30de1-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="30de1-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="30de1-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="30de1-136">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="30de1-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="30de1-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="30de1-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="30de1-138">属性または要素はコンテキスト内で有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="30de1-138">-  An attribute or element is not valid in the context</span></span>  <br/><span data-ttu-id="30de1-139">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="30de1-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="30de1-140">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="30de1-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="30de1-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="30de1-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="30de1-142">子要素</span><span class="sxs-lookup"><span data-stu-id="30de1-142">Child elements</span></span>

|<span data-ttu-id="30de1-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="30de1-143">**Element**</span></span>|<span data-ttu-id="30de1-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="30de1-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30de1-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="30de1-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="30de1-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="30de1-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="30de1-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="30de1-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="30de1-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="30de1-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="30de1-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="30de1-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="30de1-150">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="30de1-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="30de1-151">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="30de1-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="30de1-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="30de1-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="30de1-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="30de1-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="30de1-154">MailTipsConfiguration (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="30de1-154">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="30de1-155">メール ヒント サービスのサービスの構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="30de1-155">Contains service configuration information for the mail tips service.</span></span>  <br/> |
|[<span data-ttu-id="30de1-156">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="30de1-156">UnifiedMessagingConfiguration</span></span>](unifiedmessagingconfiguration.md) <br/> |<span data-ttu-id="30de1-157">ユニファイド メッセージング サービスのサービスの構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="30de1-157">Contains service configuration information for the Unified Messaging service.</span></span>  <br/> |
|[<span data-ttu-id="30de1-158">ProtectionRulesConfiguration</span><span class="sxs-lookup"><span data-stu-id="30de1-158">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="30de1-159">保護ルールのサービスのサービスの構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="30de1-159">Contains service configuration information for the protection rules service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="30de1-160">親要素</span><span class="sxs-lookup"><span data-stu-id="30de1-160">Parent elements</span></span>

|<span data-ttu-id="30de1-161">**要素**</span><span class="sxs-lookup"><span data-stu-id="30de1-161">**Element**</span></span>|<span data-ttu-id="30de1-162">**説明**</span><span class="sxs-lookup"><span data-stu-id="30de1-162">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="30de1-163">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="30de1-163">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span></span>](responsemessages-arrayofserviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="30de1-164">サービス構成の応答メッセージの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="30de1-164">Contains an array of service configuration response messages.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="30de1-165">テキスト値</span><span class="sxs-lookup"><span data-stu-id="30de1-165">Text value</span></span>

<span data-ttu-id="30de1-166">なし。</span><span class="sxs-lookup"><span data-stu-id="30de1-166">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="30de1-167">備考</span><span class="sxs-lookup"><span data-stu-id="30de1-167">Remarks</span></span>

<span data-ttu-id="30de1-168">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="30de1-168">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="30de1-169">要素情報</span><span class="sxs-lookup"><span data-stu-id="30de1-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="30de1-170">名前空間</span><span class="sxs-lookup"><span data-stu-id="30de1-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="30de1-171">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="30de1-171">Schema Name</span></span>  <br/> |<span data-ttu-id="30de1-172">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="30de1-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="30de1-173">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="30de1-173">Validation File</span></span>  <br/> |<span data-ttu-id="30de1-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="30de1-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="30de1-175">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="30de1-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="30de1-176">False</span><span class="sxs-lookup"><span data-stu-id="30de1-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="30de1-177">関連項目</span><span class="sxs-lookup"><span data-stu-id="30de1-177">See also</span></span>

- [<span data-ttu-id="30de1-178">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="30de1-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

