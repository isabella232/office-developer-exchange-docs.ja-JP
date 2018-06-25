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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833621"
---
# <a name="subscriberesponsemessage"></a><span data-ttu-id="62cd2-103">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="62cd2-103">SubscribeResponseMessage</span></span>

<span data-ttu-id="62cd2-104">**SubscribeResponseMessage**要素には、状態および 1 つの結果が含まれている[購読操作](subscribe-operation.md)要求します。</span><span class="sxs-lookup"><span data-stu-id="62cd2-104">The **SubscribeResponseMessage** element contains the status and result of a single [Subscribe operation](subscribe-operation.md) request.</span></span> 
  
- [<span data-ttu-id="62cd2-105">SubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="62cd2-105">SubscribeResponse</span></span>](subscriberesponse.md)
- [<span data-ttu-id="62cd2-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="62cd2-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="62cd2-107">SubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="62cd2-107">SubscribeResponseMessage</span></span>](subscriberesponsemessage.md)
  
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

 <span data-ttu-id="62cd2-108">**SubscribeResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="62cd2-108">**SubscribeResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="62cd2-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="62cd2-109">Attributes and elements</span></span>

<span data-ttu-id="62cd2-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="62cd2-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="62cd2-111">属性</span><span class="sxs-lookup"><span data-stu-id="62cd2-111">Attributes</span></span>

|<span data-ttu-id="62cd2-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="62cd2-112">**Attribute**</span></span>|<span data-ttu-id="62cd2-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="62cd2-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="62cd2-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="62cd2-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="62cd2-115">[Subscribe 操作](subscribe-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="62cd2-115">Describes the status of a [Subscribe operation](subscribe-operation.md) response.</span></span> <br/><br/><span data-ttu-id="62cd2-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="62cd2-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="62cd2-117">-成功</span><span class="sxs-lookup"><span data-stu-id="62cd2-117">-  Success</span></span>  <br/><span data-ttu-id="62cd2-118">-警告</span><span class="sxs-lookup"><span data-stu-id="62cd2-118">-  Warning</span></span>  <br/><span data-ttu-id="62cd2-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="62cd2-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="62cd2-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="62cd2-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="62cd2-121">**値**</span><span class="sxs-lookup"><span data-stu-id="62cd2-121">**Value**</span></span>|<span data-ttu-id="62cd2-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="62cd2-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="62cd2-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="62cd2-123">**Success**</span></span> <br/> |<span data-ttu-id="62cd2-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="62cd2-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="62cd2-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="62cd2-125">**Warning**</span></span> <br/> | <span data-ttu-id="62cd2-126">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="62cd2-126">Describes a request that was not processed.</span></span> <span data-ttu-id="62cd2-127">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="62cd2-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="62cd2-128">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="62cd2-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="62cd2-129">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="62cd2-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="62cd2-130">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="62cd2-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="62cd2-131">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="62cd2-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="62cd2-132">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="62cd2-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="62cd2-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="62cd2-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="62cd2-134">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="62cd2-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="62cd2-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="62cd2-135">**Error**</span></span> <br/> | <span data-ttu-id="62cd2-136">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="62cd2-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="62cd2-137">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="62cd2-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="62cd2-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="62cd2-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="62cd2-139">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="62cd2-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="62cd2-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="62cd2-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="62cd2-141">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="62cd2-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="62cd2-142">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="62cd2-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="62cd2-143">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="62cd2-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="62cd2-144">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="62cd2-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="62cd2-145">子要素</span><span class="sxs-lookup"><span data-stu-id="62cd2-145">Child elements</span></span>

|<span data-ttu-id="62cd2-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="62cd2-146">**Element**</span></span>|<span data-ttu-id="62cd2-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="62cd2-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62cd2-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="62cd2-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="62cd2-149">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="62cd2-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="62cd2-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="62cd2-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="62cd2-151">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="62cd2-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="62cd2-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="62cd2-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="62cd2-153">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="62cd2-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="62cd2-154">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="62cd2-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="62cd2-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="62cd2-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="62cd2-156">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="62cd2-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="62cd2-157">サブスクリプション Id (GetEvents)</span><span class="sxs-lookup"><span data-stu-id="62cd2-157">SubscriptionId (GetEvents)</span></span>](subscriptionid-getevents.md) <br/> |<span data-ttu-id="62cd2-158">サブスクリプションの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="62cd2-158">Represents the identifier for a subscription.</span></span>  <br/> |
|[<span data-ttu-id="62cd2-159">透かし</span><span class="sxs-lookup"><span data-stu-id="62cd2-159">Watermark</span></span>](watermark.md) <br/> |<span data-ttu-id="62cd2-160">メールボックス イベント キュー内のイベント ブックマークを表します。</span><span class="sxs-lookup"><span data-stu-id="62cd2-160">Represents an event bookmark in the mailbox event queue.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="62cd2-161">親要素</span><span class="sxs-lookup"><span data-stu-id="62cd2-161">Parent elements</span></span>

|<span data-ttu-id="62cd2-162">**要素**</span><span class="sxs-lookup"><span data-stu-id="62cd2-162">**Element**</span></span>|<span data-ttu-id="62cd2-163">**説明**</span><span class="sxs-lookup"><span data-stu-id="62cd2-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="62cd2-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="62cd2-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="62cd2-165">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="62cd2-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="62cd2-166">備考</span><span class="sxs-lookup"><span data-stu-id="62cd2-166">Remarks</span></span>

<span data-ttu-id="62cd2-167">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="62cd2-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="62cd2-168">要素情報</span><span class="sxs-lookup"><span data-stu-id="62cd2-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="62cd2-169">名前空間</span><span class="sxs-lookup"><span data-stu-id="62cd2-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="62cd2-170">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="62cd2-170">Schema Name</span></span>  <br/> |<span data-ttu-id="62cd2-171">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="62cd2-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="62cd2-172">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="62cd2-172">Validation File</span></span>  <br/> |<span data-ttu-id="62cd2-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="62cd2-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="62cd2-174">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="62cd2-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="62cd2-175">False</span><span class="sxs-lookup"><span data-stu-id="62cd2-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="62cd2-176">関連項目</span><span class="sxs-lookup"><span data-stu-id="62cd2-176">See also</span></span>

- [<span data-ttu-id="62cd2-177">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="62cd2-177">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="62cd2-178">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="62cd2-178">GetEvents operation</span></span>](getevents-operation.md)
- [<span data-ttu-id="62cd2-179">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="62cd2-179">Unsubscribe operation</span></span>](unsubscribe-operation.md)

