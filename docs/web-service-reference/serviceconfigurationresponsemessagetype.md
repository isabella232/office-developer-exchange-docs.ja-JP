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
description: ServiceConfigurationResponseMessageType 要素には、サービス構成設定が含まれています。
ms.openlocfilehash: 4c84a49b2403343a1defd00696858489497d6214
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44439106"
---
# <a name="serviceconfigurationresponsemessagetype"></a><span data-ttu-id="600ff-103">ServiceConfigurationResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="600ff-103">ServiceConfigurationResponseMessageType</span></span>

<span data-ttu-id="600ff-104">**ServiceConfigurationResponseMessageType**要素には、サービス構成設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="600ff-104">The **ServiceConfigurationResponseMessageType** element contains service configuration settings.</span></span> 
  
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

 <span data-ttu-id="600ff-105">**ServiceConfigurationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="600ff-105">**ServiceConfigurationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="600ff-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="600ff-106">Attributes and elements</span></span>

<span data-ttu-id="600ff-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="600ff-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="600ff-108">属性</span><span class="sxs-lookup"><span data-stu-id="600ff-108">Attributes</span></span>

|<span data-ttu-id="600ff-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="600ff-109">**Attribute**</span></span>|<span data-ttu-id="600ff-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="600ff-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="600ff-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="600ff-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="600ff-112">応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="600ff-112">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="600ff-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="600ff-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="600ff-114">-成功</span><span class="sxs-lookup"><span data-stu-id="600ff-114">-  Success</span></span>  <br/><span data-ttu-id="600ff-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="600ff-115">-  Warning</span></span>  <br/><span data-ttu-id="600ff-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="600ff-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="600ff-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="600ff-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="600ff-118">**値**</span><span class="sxs-lookup"><span data-stu-id="600ff-118">**Value**</span></span>|<span data-ttu-id="600ff-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="600ff-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="600ff-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="600ff-120">**Success**</span></span> <br/> |<span data-ttu-id="600ff-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="600ff-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="600ff-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="600ff-122">**Warning**</span></span> <br/> | <span data-ttu-id="600ff-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="600ff-123">Describes a request that was not processed.</span></span> <span data-ttu-id="600ff-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="600ff-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="600ff-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="600ff-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="600ff-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="600ff-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="600ff-127">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="600ff-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="600ff-128">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="600ff-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="600ff-129">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="600ff-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="600ff-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="600ff-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="600ff-131">-クォータが限界を超えています。</span><span class="sxs-lookup"><span data-stu-id="600ff-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="600ff-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="600ff-132">**Error**</span></span> <br/> | <span data-ttu-id="600ff-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="600ff-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="600ff-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="600ff-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="600ff-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="600ff-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="600ff-136">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="600ff-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="600ff-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="600ff-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="600ff-138">-コンテキスト内で属性または要素が無効です</span><span class="sxs-lookup"><span data-stu-id="600ff-138">-  An attribute or element is not valid in the context</span></span>  <br/><span data-ttu-id="600ff-139">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="600ff-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="600ff-140">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="600ff-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="600ff-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="600ff-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="600ff-142">子要素</span><span class="sxs-lookup"><span data-stu-id="600ff-142">Child elements</span></span>

|<span data-ttu-id="600ff-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="600ff-143">**Element**</span></span>|<span data-ttu-id="600ff-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="600ff-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="600ff-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="600ff-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="600ff-146">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="600ff-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="600ff-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="600ff-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="600ff-148">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="600ff-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="600ff-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="600ff-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="600ff-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="600ff-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="600ff-151">この要素には0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="600ff-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="600ff-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="600ff-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="600ff-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="600ff-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="600ff-154">Mailヒント構成 (MailTipsServiceConfiguration)</span><span class="sxs-lookup"><span data-stu-id="600ff-154">MailTipsConfiguration (MailTipsServiceConfiguration)</span></span>](mailtipsconfiguration-mailtipsserviceconfiguration.md) <br/> |<span data-ttu-id="600ff-155">メールヒントサービスのサービス構成情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="600ff-155">Contains service configuration information for the mail tips service.</span></span>  <br/> |
|[<span data-ttu-id="600ff-156">UnifiedMessagingConfiguration</span><span class="sxs-lookup"><span data-stu-id="600ff-156">UnifiedMessagingConfiguration</span></span>](unifiedmessagingconfiguration.md) <br/> |<span data-ttu-id="600ff-157">ユニファイドメッセージングサービスのサービス構成情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="600ff-157">Contains service configuration information for the Unified Messaging service.</span></span>  <br/> |
|[<span data-ttu-id="600ff-158">Protectionルールの構成</span><span class="sxs-lookup"><span data-stu-id="600ff-158">ProtectionRulesConfiguration</span></span>](protectionrulesconfiguration.md) <br/> |<span data-ttu-id="600ff-159">保護ルールサービスのサービス構成情報が保存されています。</span><span class="sxs-lookup"><span data-stu-id="600ff-159">Contains service configuration information for the protection rules service.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="600ff-160">親要素</span><span class="sxs-lookup"><span data-stu-id="600ff-160">Parent elements</span></span>

|<span data-ttu-id="600ff-161">**要素**</span><span class="sxs-lookup"><span data-stu-id="600ff-161">**Element**</span></span>|<span data-ttu-id="600ff-162">**説明**</span><span class="sxs-lookup"><span data-stu-id="600ff-162">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="600ff-163">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="600ff-163">ResponseMessages (ArrayOfServiceConfigurationResponseMessageType)</span></span>](responsemessages-arrayofserviceconfigurationresponsemessagetype.md) <br/> |<span data-ttu-id="600ff-164">サービス構成応答メッセージの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="600ff-164">Contains an array of service configuration response messages.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="600ff-165">テキスト値</span><span class="sxs-lookup"><span data-stu-id="600ff-165">Text value</span></span>

<span data-ttu-id="600ff-166">なし。</span><span class="sxs-lookup"><span data-stu-id="600ff-166">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="600ff-167">注釈</span><span class="sxs-lookup"><span data-stu-id="600ff-167">Remarks</span></span>

<span data-ttu-id="600ff-168">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="600ff-168">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="600ff-169">要素の情報</span><span class="sxs-lookup"><span data-stu-id="600ff-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="600ff-170">Namespace</span><span class="sxs-lookup"><span data-stu-id="600ff-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="600ff-171">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="600ff-171">Schema Name</span></span>  <br/> |<span data-ttu-id="600ff-172">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="600ff-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="600ff-173">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="600ff-173">Validation File</span></span>  <br/> |<span data-ttu-id="600ff-174">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="600ff-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="600ff-175">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="600ff-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="600ff-176">正しくない</span><span class="sxs-lookup"><span data-stu-id="600ff-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="600ff-177">関連項目</span><span class="sxs-lookup"><span data-stu-id="600ff-177">See also</span></span>

- [<span data-ttu-id="600ff-178">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="600ff-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

