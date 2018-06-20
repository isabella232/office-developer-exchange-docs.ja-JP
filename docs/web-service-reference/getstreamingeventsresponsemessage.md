---
title: GetStreamingEventsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetStreamingEventsResponseMessage
api_type:
- schema
ms.assetid: 655e4e78-af74-48b0-a988-7d86ab368feb
description: GetStreamingEventsResponseMessage 要素には、状態および 1 つの GetStreamingEvents 操作要求の結果が含まれています。
ms.openlocfilehash: 5fcc7ddde41b49a5d8b304da0732f4472c61a76a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19831682"
---
# <a name="getstreamingeventsresponsemessage"></a><span data-ttu-id="e2d0b-103">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e2d0b-103">GetStreamingEventsResponseMessage</span></span>

<span data-ttu-id="e2d0b-104">**GetStreamingEventsResponseMessage**要素には、状態および 1 つの結果が含まれている[GetStreamingEvents の操作](getstreamingevents-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-104">The **GetStreamingEventsResponseMessage** element contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span> 
  
```xml
<GetStreamingEventsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notifications/>
   <ErrorSubscriptionIds/>
   <ConnectionStatus/>
</GetStreamingEventsResponseMessage>
```

 <span data-ttu-id="e2d0b-105">**GetStreamingEventsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e2d0b-105">**GetStreamingEventsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e2d0b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e2d0b-106">Attributes and elements</span></span>

<span data-ttu-id="e2d0b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e2d0b-108">属性</span><span class="sxs-lookup"><span data-stu-id="e2d0b-108">Attributes</span></span>

|<span data-ttu-id="e2d0b-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="e2d0b-109">**Attribute**</span></span>|<span data-ttu-id="e2d0b-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="e2d0b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e2d0b-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="e2d0b-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="e2d0b-112">[GetStreamingEvents 操作](getstreamingevents-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-112">Describes the status of a [GetStreamingEvents operation](getstreamingevents-operation.md) response.</span></span> <br/><br/><span data-ttu-id="e2d0b-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="e2d0b-114">-成功</span><span class="sxs-lookup"><span data-stu-id="e2d0b-114">-  Success</span></span>  <br/><span data-ttu-id="e2d0b-115">-警告</span><span class="sxs-lookup"><span data-stu-id="e2d0b-115">-  Warning</span></span>  <br/><span data-ttu-id="e2d0b-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="e2d0b-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="e2d0b-117">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="e2d0b-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="e2d0b-118">**値**</span><span class="sxs-lookup"><span data-stu-id="e2d0b-118">**Value**</span></span>|<span data-ttu-id="e2d0b-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="e2d0b-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e2d0b-120">成功</span><span class="sxs-lookup"><span data-stu-id="e2d0b-120">Success</span></span>  <br/> |<span data-ttu-id="e2d0b-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="e2d0b-122">警告</span><span class="sxs-lookup"><span data-stu-id="e2d0b-122">Warning</span></span>  <br/> | <span data-ttu-id="e2d0b-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-123">Describes a request that was not processed.</span></span> <span data-ttu-id="e2d0b-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="e2d0b-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="e2d0b-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="e2d0b-127">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="e2d0b-128">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="e2d0b-129">-メールボックス データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-129">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="e2d0b-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="e2d0b-131">クォータを超過しました。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="e2d0b-132">エラー</span><span class="sxs-lookup"><span data-stu-id="e2d0b-132">Error</span></span>  <br/> | <span data-ttu-id="e2d0b-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="e2d0b-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="e2d0b-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="e2d0b-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="e2d0b-136">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="e2d0b-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="e2d0b-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="e2d0b-138">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="e2d0b-139">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="e2d0b-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="e2d0b-140">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="e2d0b-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="e2d0b-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e2d0b-142">子要素</span><span class="sxs-lookup"><span data-stu-id="e2d0b-142">Child elements</span></span>

|<span data-ttu-id="e2d0b-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="e2d0b-143">**Element**</span></span>|<span data-ttu-id="e2d0b-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="e2d0b-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2d0b-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="e2d0b-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e2d0b-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e2d0b-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e2d0b-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e2d0b-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="e2d0b-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e2d0b-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e2d0b-150">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="e2d0b-151">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="e2d0b-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e2d0b-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e2d0b-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="e2d0b-154">通知</span><span class="sxs-lookup"><span data-stu-id="e2d0b-154">Notifications</span></span>](notifications.md) <br/> |<span data-ttu-id="e2d0b-155">サブスクリプションおよび最後の通知以降に発生したイベントに関する情報の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-155">Contains a list of information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
|[<span data-ttu-id="e2d0b-156">ErrorSubscriptionIds</span><span class="sxs-lookup"><span data-stu-id="e2d0b-156">ErrorSubscriptionIds</span></span>](errorsubscriptionids.md) <br/> |<span data-ttu-id="e2d0b-157">サブスクリプションが無効な Id の一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-157">Contains a list of subscription IDs that are invalid.</span></span>  <br/> |
|[<span data-ttu-id="e2d0b-158">ConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="e2d0b-158">ConnectionStatus</span></span>](connectionstatus.md) <br/> |<span data-ttu-id="e2d0b-159">ストリーミングのサブスクリプションの状態の説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-159">Provides a text description of the status of a streaming subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e2d0b-160">親要素</span><span class="sxs-lookup"><span data-stu-id="e2d0b-160">Parent elements</span></span>

|<span data-ttu-id="e2d0b-161">**要素**</span><span class="sxs-lookup"><span data-stu-id="e2d0b-161">**Element**</span></span>|<span data-ttu-id="e2d0b-162">**説明**</span><span class="sxs-lookup"><span data-stu-id="e2d0b-162">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e2d0b-163">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e2d0b-163">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="e2d0b-164">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-164">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="e2d0b-165">テキスト値</span><span class="sxs-lookup"><span data-stu-id="e2d0b-165">Text value</span></span>

<span data-ttu-id="e2d0b-166">なし。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-166">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e2d0b-167">備考</span><span class="sxs-lookup"><span data-stu-id="e2d0b-167">Remarks</span></span>

<span data-ttu-id="e2d0b-168">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e2d0b-168">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e2d0b-169">要素情報</span><span class="sxs-lookup"><span data-stu-id="e2d0b-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e2d0b-170">名前空間</span><span class="sxs-lookup"><span data-stu-id="e2d0b-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e2d0b-171">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e2d0b-171">Schema Name</span></span>  <br/> |<span data-ttu-id="e2d0b-172">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e2d0b-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e2d0b-173">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e2d0b-173">Validation File</span></span>  <br/> |<span data-ttu-id="e2d0b-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e2d0b-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e2d0b-175">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e2d0b-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="e2d0b-176">False</span><span class="sxs-lookup"><span data-stu-id="e2d0b-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e2d0b-177">関連項目</span><span class="sxs-lookup"><span data-stu-id="e2d0b-177">See also</span></span>

- [<span data-ttu-id="e2d0b-178">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="e2d0b-178">GetStreamingEvents</span></span>](getstreamingevents.md) 
- [<span data-ttu-id="e2d0b-179">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="e2d0b-179">GetStreamingEventsResponse</span></span>](getstreamingeventsresponse.md)
- [<span data-ttu-id="e2d0b-180">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="e2d0b-180">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)

