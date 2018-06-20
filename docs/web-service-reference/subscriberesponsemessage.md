---
title: SubscribeResponseMessage
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
description: SubscribeResponseMessage 要素には、状態および 1 つの受信操作要求の結果が含まれています。
ms.openlocfilehash: 97c7bd9f12511ff226e75f53278c13481679c8a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833621"
---
# <a name="subscriberesponsemessage"></a><span data-ttu-id="2759b-103">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2759b-103">SubscribeResponseMessage</span></span>

<span data-ttu-id="2759b-104">**SubscribeResponseMessage**要素には、状態および 1 つの結果が含まれている[購読操作](subscribe-operation.md)要求します。</span><span class="sxs-lookup"><span data-stu-id="2759b-104">The **SubscribeResponseMessage** element contains the status and result of a single [Subscribe operation](subscribe-operation.md) request.</span></span> 
  
- [<span data-ttu-id="2759b-105">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="2759b-105">SubscribeResponse</span></span>](subscriberesponse.md)
- [<span data-ttu-id="2759b-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2759b-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="2759b-107">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2759b-107">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
  
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

 <span data-ttu-id="2759b-108">**SubscribeResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="2759b-108">**SubscribeResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2759b-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2759b-109">Attributes and elements</span></span>

<span data-ttu-id="2759b-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2759b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2759b-111">属性</span><span class="sxs-lookup"><span data-stu-id="2759b-111">Attributes</span></span>

|<span data-ttu-id="2759b-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="2759b-112">**Attribute**</span></span>|<span data-ttu-id="2759b-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="2759b-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2759b-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="2759b-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="2759b-115">[Subscribe 操作](subscribe-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="2759b-115">Describes the status of a [Subscribe operation](subscribe-operation.md) response.</span></span> <br/><br/><span data-ttu-id="2759b-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="2759b-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="2759b-117">-成功</span><span class="sxs-lookup"><span data-stu-id="2759b-117">-  Success</span></span>  <br/><span data-ttu-id="2759b-118">-警告</span><span class="sxs-lookup"><span data-stu-id="2759b-118">-  Warning</span></span>  <br/><span data-ttu-id="2759b-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="2759b-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="2759b-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="2759b-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="2759b-121">**値**</span><span class="sxs-lookup"><span data-stu-id="2759b-121">**Value**</span></span>|<span data-ttu-id="2759b-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="2759b-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2759b-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="2759b-123">**Success**</span></span> <br/> |<span data-ttu-id="2759b-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="2759b-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="2759b-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="2759b-125">**Warning**</span></span> <br/> | <span data-ttu-id="2759b-126">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="2759b-126">Describes a request that was not processed.</span></span> <span data-ttu-id="2759b-127">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="2759b-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="2759b-128">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2759b-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="2759b-129">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="2759b-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="2759b-130">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="2759b-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="2759b-131">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="2759b-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="2759b-132">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="2759b-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="2759b-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="2759b-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="2759b-134">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="2759b-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="2759b-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="2759b-135">**Error**</span></span> <br/> | <span data-ttu-id="2759b-136">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="2759b-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="2759b-137">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="2759b-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="2759b-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="2759b-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="2759b-139">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="2759b-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="2759b-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="2759b-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="2759b-141">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="2759b-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="2759b-142">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="2759b-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="2759b-143">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="2759b-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="2759b-144">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="2759b-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2759b-145">子要素</span><span class="sxs-lookup"><span data-stu-id="2759b-145">Child elements</span></span>

|<span data-ttu-id="2759b-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="2759b-146">**Element**</span></span>|<span data-ttu-id="2759b-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="2759b-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2759b-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="2759b-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="2759b-149">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="2759b-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="2759b-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2759b-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="2759b-151">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="2759b-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="2759b-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="2759b-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="2759b-153">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="2759b-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="2759b-154">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2759b-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="2759b-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="2759b-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="2759b-156">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="2759b-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="2759b-157">サブスクリプション Id (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="2759b-157">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="2759b-158">サブスクリプションの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="2759b-158">Represents the identifier for a subscription.</span></span>  <br/> |
|[<span data-ttu-id="2759b-159">透かし</span><span class="sxs-lookup"><span data-stu-id="2759b-159">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="2759b-160">メールボックス イベント キュー内のイベント ブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="2759b-160">Represents an event bookmark in the mailbox event queue.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2759b-161">親要素</span><span class="sxs-lookup"><span data-stu-id="2759b-161">Parent elements</span></span>

|<span data-ttu-id="2759b-162">**要素**</span><span class="sxs-lookup"><span data-stu-id="2759b-162">**Element**</span></span>|<span data-ttu-id="2759b-163">**説明**</span><span class="sxs-lookup"><span data-stu-id="2759b-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2759b-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2759b-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="2759b-165">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2759b-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2759b-166">備考</span><span class="sxs-lookup"><span data-stu-id="2759b-166">Remarks</span></span>

<span data-ttu-id="2759b-167">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2759b-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2759b-168">要素情報</span><span class="sxs-lookup"><span data-stu-id="2759b-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2759b-169">名前空間</span><span class="sxs-lookup"><span data-stu-id="2759b-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2759b-170">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2759b-170">Schema Name</span></span>  <br/> |<span data-ttu-id="2759b-171">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="2759b-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2759b-172">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2759b-172">Validation File</span></span>  <br/> |<span data-ttu-id="2759b-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2759b-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2759b-174">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2759b-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="2759b-175">False</span><span class="sxs-lookup"><span data-stu-id="2759b-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2759b-176">関連項目</span><span class="sxs-lookup"><span data-stu-id="2759b-176">See also</span></span>

- [<span data-ttu-id="2759b-177">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="2759b-177">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="2759b-178">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="2759b-178">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="2759b-179">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="2759b-179">Unsubscribe operation</span></span>](unsubscribe-operation.md)

