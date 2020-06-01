---
title: ApplyConversationActionResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationActionResponseMessage
api_type:
- schema
ms.assetid: a09edc89-7f2f-4846-a3a5-06694c97b9f6
description: ApplyConversationActionResponseMessage 要素には、ApplyConversationAction 操作要求の状態と結果が含まれています。
ms.openlocfilehash: 377aee12d8cc7d6b4aff8d6fc2a6cb67b3bcd10b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44464694"
---
# <a name="applyconversationactionresponsemessage"></a><span data-ttu-id="4a4e9-103">ApplyConversationActionResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4a4e9-103">ApplyConversationActionResponseMessage</span></span>

<span data-ttu-id="4a4e9-104">**ApplyConversationActionResponseMessage**要素には、 [ApplyConversationAction 操作](applyconversationaction-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-104">The **ApplyConversationActionResponseMessage** element contains the status and results of an [ApplyConversationAction operation](applyconversationaction-operation.md) request.</span></span>  
  
- [<span data-ttu-id="4a4e9-105">ApplyConversationActionResponse</span><span class="sxs-lookup"><span data-stu-id="4a4e9-105">ApplyConversationActionResponse</span></span>](applyconversationactionresponse.md)
- [<span data-ttu-id="4a4e9-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4a4e9-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="4a4e9-107">ApplyConversationActionResponseMessage</span><span class="sxs-lookup"><span data-stu-id="4a4e9-107">ApplyConversationActionResponseMessage</span></span>](applyconversationactionresponsemessage.md)
  
```XML
<ApplyConversationActionResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ApplyConversationActionResponseMessage>
```

 <span data-ttu-id="4a4e9-108">**ApplyConversationActionResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="4a4e9-108">**ApplyConversationActionResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4a4e9-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="4a4e9-109">Attributes and elements</span></span>

<span data-ttu-id="4a4e9-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4a4e9-111">属性</span><span class="sxs-lookup"><span data-stu-id="4a4e9-111">Attributes</span></span>

|<span data-ttu-id="4a4e9-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="4a4e9-112">**Attribute**</span></span>|<span data-ttu-id="4a4e9-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="4a4e9-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4a4e9-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="4a4e9-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="4a4e9-115">応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-115">Describes the status of the response.</span></span><br/><br/><span data-ttu-id="4a4e9-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-116">The following values are valid for this attribute:</span></span><ul><li><span data-ttu-id="4a4e9-117">Success</span><span class="sxs-lookup"><span data-stu-id="4a4e9-117">Success</span></span></li><li><span data-ttu-id="4a4e9-118">警告</span><span class="sxs-lookup"><span data-stu-id="4a4e9-118">Warning</span></span></li><li><span data-ttu-id="4a4e9-119">Error</span><span class="sxs-lookup"><span data-stu-id="4a4e9-119">Error</span></span></li></ul> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="4a4e9-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="4a4e9-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="4a4e9-121">**値**</span><span class="sxs-lookup"><span data-stu-id="4a4e9-121">**Value**</span></span>|<span data-ttu-id="4a4e9-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="4a4e9-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4a4e9-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="4a4e9-123">**Success**</span></span> <br/> |<span data-ttu-id="4a4e9-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="4a4e9-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="4a4e9-125">**Warning**</span></span> <br/> | <span data-ttu-id="4a4e9-126">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-126">Describes a request that was not processed.</span></span> <span data-ttu-id="4a4e9-127">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="4a4e9-128">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-128">The following are examples of sources of warnings:</span></span><ul><li><span data-ttu-id="4a4e9-129">Exchange ストアは、バッチ処理中にオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-129">The Exchange store is offline during the batch.</span></span></li><li><span data-ttu-id="4a4e9-130">Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-130">Active Directory Domain Services (AD DS) is offline.</span></span></li><li><span data-ttu-id="4a4e9-131">メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-131">Mailboxes were moved.</span></span></li><li><span data-ttu-id="4a4e9-132">メッセージデータベース (MDB) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-132">The message database (MDB) is offline.</span></span></li><li><span data-ttu-id="4a4e9-133">パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-133">A password is expired.</span></span></li><li><span data-ttu-id="4a4e9-134">クォータが制限を超えています。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-134">A quota has been exceeded.</span></span></li></ul> |
|<span data-ttu-id="4a4e9-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="4a4e9-135">**Error**</span></span> <br/> | <span data-ttu-id="4a4e9-136">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="4a4e9-137">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-137">The following are examples of sources of errors:</span></span>  <ul><li><span data-ttu-id="4a4e9-138">無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="4a4e9-138">Invalid attributes or elements</span></span></li><li><span data-ttu-id="4a4e9-139">範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="4a4e9-139">Attributes or elements that are out of range</span></span></li><li><span data-ttu-id="4a4e9-140">不明なタグ</span><span class="sxs-lookup"><span data-stu-id="4a4e9-140">An unknown tag</span></span>  </li><li><span data-ttu-id="4a4e9-141">コンテキストで有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="4a4e9-141">An attribute or element that is not valid in the context</span></span></li><li><span data-ttu-id="4a4e9-142">クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="4a4e9-142">An unauthorized access attempt by any client</span></span></li><li><span data-ttu-id="4a4e9-143">有効なクライアント側の呼び出しに応答した場合のサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="4a4e9-143">A server-side failure in response to a valid client-side call</span></span></li></ul><span data-ttu-id="4a4e9-144">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4a4e9-145">子要素</span><span class="sxs-lookup"><span data-stu-id="4a4e9-145">Child elements</span></span>

|<span data-ttu-id="4a4e9-146">**Element**</span><span class="sxs-lookup"><span data-stu-id="4a4e9-146">**Element**</span></span>|<span data-ttu-id="4a4e9-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="4a4e9-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a4e9-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="4a4e9-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4a4e9-149">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4a4e9-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4a4e9-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4a4e9-151">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="4a4e9-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4a4e9-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4a4e9-153">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="4a4e9-154">この要素には0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="4a4e9-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="4a4e9-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4a4e9-156">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4a4e9-157">親要素</span><span class="sxs-lookup"><span data-stu-id="4a4e9-157">Parent elements</span></span>

|<span data-ttu-id="4a4e9-158">**要素**</span><span class="sxs-lookup"><span data-stu-id="4a4e9-158">**Element**</span></span>|<span data-ttu-id="4a4e9-159">**説明**</span><span class="sxs-lookup"><span data-stu-id="4a4e9-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4a4e9-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="4a4e9-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="4a4e9-161">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="4a4e9-162">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4a4e9-162">Text value</span></span>

<span data-ttu-id="4a4e9-163">なし。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-163">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4a4e9-164">注釈</span><span class="sxs-lookup"><span data-stu-id="4a4e9-164">Remarks</span></span>

<span data-ttu-id="4a4e9-165">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-165">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="4a4e9-166">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="4a4e9-166">Version differences</span></span>

<span data-ttu-id="4a4e9-167">Build 15.00.0986.00 以降のバージョンの Exchange では、 **ApplyConversationActionResponseMessage**要素の型は**ApplyConversationActionResponseMessageType**です。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-167">In versions of Exchange starting with build 15.00.0986.00, the **ApplyConversationActionResponseMessage** element is of type **ApplyConversationActionResponseMessageType**.</span></span> <span data-ttu-id="4a4e9-168">以前のバージョンでは、要素の種類は**Responsemessagetype**です。</span><span class="sxs-lookup"><span data-stu-id="4a4e9-168">In previous versions, the element is of type **ResponseMessageType**.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4a4e9-169">要素の情報</span><span class="sxs-lookup"><span data-stu-id="4a4e9-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4a4e9-170">Namespace</span><span class="sxs-lookup"><span data-stu-id="4a4e9-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4a4e9-171">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4a4e9-171">Schema Name</span></span>  <br/> |<span data-ttu-id="4a4e9-172">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="4a4e9-172">Message schema</span></span>  <br/> |
|<span data-ttu-id="4a4e9-173">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4a4e9-173">Validation File</span></span>  <br/> |<span data-ttu-id="4a4e9-174">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="4a4e9-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4a4e9-175">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="4a4e9-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="4a4e9-176">正しくない</span><span class="sxs-lookup"><span data-stu-id="4a4e9-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4a4e9-177">関連項目</span><span class="sxs-lookup"><span data-stu-id="4a4e9-177">See also</span></span>

- [<span data-ttu-id="4a4e9-178">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="4a4e9-178">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="4a4e9-179">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="4a4e9-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

