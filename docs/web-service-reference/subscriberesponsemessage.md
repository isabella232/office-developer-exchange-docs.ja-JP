---
title: メッセージの表示
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SubscribeResponseMessage
api_type:
- schema
ms.assetid: d121d38a-a61a-4f9c-a477-fc6d7f9af77e
description: /要求は、単一の Subscribe 操作要求の状態と結果を含みます。
ms.openlocfilehash: eea7356dbcf1887383d56e40a4f6dcd091535fa3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465374"
---
# <a name="subscriberesponsemessage"></a><span data-ttu-id="3b707-103">メッセージの表示</span><span class="sxs-lookup"><span data-stu-id="3b707-103">SubscribeResponseMessage</span></span>

<span data-ttu-id="3b707-104">/要求**は、単一**の[Subscribe 操作](subscribe-operation.md)要求の状態と結果を含みます。</span><span class="sxs-lookup"><span data-stu-id="3b707-104">The **SubscribeResponseMessage** element contains the status and result of a single [Subscribe operation](subscribe-operation.md) request.</span></span> 
  
- [<span data-ttu-id="3b707-105">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="3b707-105">SubscribeResponse</span></span>](subscriberesponse.md)
- [<span data-ttu-id="3b707-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3b707-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="3b707-107">メッセージの表示</span><span class="sxs-lookup"><span data-stu-id="3b707-107">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
  
```xml
<SubscribeResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SubscriptionId/>
   <Watermark/>
</SubscribeResponseMessage>
```

 <span data-ttu-id="3b707-108">**オンラインでのお電話**</span><span class="sxs-lookup"><span data-stu-id="3b707-108">**SubscribeResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3b707-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3b707-109">Attributes and elements</span></span>

<span data-ttu-id="3b707-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3b707-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3b707-111">属性</span><span class="sxs-lookup"><span data-stu-id="3b707-111">Attributes</span></span>

|<span data-ttu-id="3b707-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="3b707-112">**Attribute**</span></span>|<span data-ttu-id="3b707-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="3b707-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3b707-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="3b707-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="3b707-115">[サブスクライブ操作](subscribe-operation.md)応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="3b707-115">Describes the status of a [Subscribe operation](subscribe-operation.md) response.</span></span> <br/><br/><span data-ttu-id="3b707-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="3b707-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="3b707-117">-成功</span><span class="sxs-lookup"><span data-stu-id="3b707-117">-  Success</span></span>  <br/><span data-ttu-id="3b707-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="3b707-118">-  Warning</span></span>  <br/><span data-ttu-id="3b707-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="3b707-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="3b707-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="3b707-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="3b707-121">**値**</span><span class="sxs-lookup"><span data-stu-id="3b707-121">**Value**</span></span>|<span data-ttu-id="3b707-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="3b707-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3b707-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="3b707-123">**Success**</span></span> <br/> |<span data-ttu-id="3b707-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="3b707-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="3b707-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="3b707-125">**Warning**</span></span> <br/> | <span data-ttu-id="3b707-126">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="3b707-126">Describes a request that was not processed.</span></span> <span data-ttu-id="3b707-127">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3b707-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="3b707-128">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3b707-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="3b707-129">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="3b707-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="3b707-130">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="3b707-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="3b707-131">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="3b707-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="3b707-132">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="3b707-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="3b707-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="3b707-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="3b707-134">-クォータが限界を超えています。</span><span class="sxs-lookup"><span data-stu-id="3b707-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="3b707-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="3b707-135">**Error**</span></span> <br/> | <span data-ttu-id="3b707-136">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="3b707-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="3b707-137">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3b707-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="3b707-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="3b707-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="3b707-139">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="3b707-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="3b707-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="3b707-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="3b707-141">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="3b707-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="3b707-142">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="3b707-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="3b707-143">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="3b707-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="3b707-144">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3b707-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3b707-145">子要素</span><span class="sxs-lookup"><span data-stu-id="3b707-145">Child elements</span></span>

|<span data-ttu-id="3b707-146">**Element**</span><span class="sxs-lookup"><span data-stu-id="3b707-146">**Element**</span></span>|<span data-ttu-id="3b707-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="3b707-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b707-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="3b707-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="3b707-149">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="3b707-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="3b707-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3b707-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="3b707-151">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="3b707-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="3b707-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3b707-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="3b707-153">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="3b707-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="3b707-154">この要素には0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3b707-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="3b707-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="3b707-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="3b707-156">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="3b707-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="3b707-157">SubscriptionId (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="3b707-157">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="3b707-158">サブスクリプションの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="3b707-158">Represents the identifier for a subscription.</span></span>  <br/> |
|[<span data-ttu-id="3b707-159">Watermark</span><span class="sxs-lookup"><span data-stu-id="3b707-159">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="3b707-160">メールボックスイベントキュー内のイベントブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="3b707-160">Represents an event bookmark in the mailbox event queue.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3b707-161">親要素</span><span class="sxs-lookup"><span data-stu-id="3b707-161">Parent elements</span></span>

|<span data-ttu-id="3b707-162">**要素**</span><span class="sxs-lookup"><span data-stu-id="3b707-162">**Element**</span></span>|<span data-ttu-id="3b707-163">**説明**</span><span class="sxs-lookup"><span data-stu-id="3b707-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3b707-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3b707-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="3b707-165">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="3b707-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3b707-166">注釈</span><span class="sxs-lookup"><span data-stu-id="3b707-166">Remarks</span></span>

<span data-ttu-id="3b707-167">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="3b707-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="3b707-168">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3b707-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3b707-169">Namespace</span><span class="sxs-lookup"><span data-stu-id="3b707-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3b707-170">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3b707-170">Schema Name</span></span>  <br/> |<span data-ttu-id="3b707-171">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="3b707-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3b707-172">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3b707-172">Validation File</span></span>  <br/> |<span data-ttu-id="3b707-173">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3b707-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3b707-174">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3b707-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="3b707-175">正しくない</span><span class="sxs-lookup"><span data-stu-id="3b707-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3b707-176">関連項目</span><span class="sxs-lookup"><span data-stu-id="3b707-176">See also</span></span>

- [<span data-ttu-id="3b707-177">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="3b707-177">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="3b707-178">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="3b707-178">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="3b707-179">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="3b707-179">Unsubscribe operation</span></span>](unsubscribe-operation.md)

