---
title: SendNotificationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendNotificationResponseMessage
api_type:
- schema
ms.assetid: 2c6d681b-67ac-4331-bc6b-a2e709b638e3
description: SendNotificationResponseMessage 要素には、状態および 1 つの SendNotification 操作要求の結果が含まれています。
ms.openlocfilehash: 49677b6d61f525b469679ec3fdcb8aadcca7239d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/21/2018
ms.locfileid: "19833348"
---
# <a name="sendnotificationresponsemessage"></a><span data-ttu-id="388dd-103">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="388dd-103">SendNotificationResponseMessage</span></span>

<span data-ttu-id="388dd-104">**SendNotificationResponseMessage**要素には、状態および 1 つの**SendNotification**操作要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="388dd-104">The **SendNotificationResponseMessage** element contains the status and result of a single **SendNotification** operation request.</span></span> 
  
```xml
<SendNotificationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notification/>
</SendNotificationResponseMessage>
```

 <span data-ttu-id="388dd-105">**SendNotificationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="388dd-105">**SendNotificationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="388dd-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="388dd-106">Attributes and elements</span></span>

<span data-ttu-id="388dd-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="388dd-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="388dd-108">属性</span><span class="sxs-lookup"><span data-stu-id="388dd-108">Attributes</span></span>

|<span data-ttu-id="388dd-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="388dd-109">**Attribute**</span></span>|<span data-ttu-id="388dd-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="388dd-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="388dd-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="388dd-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="388dd-112">**SendNotification**操作の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="388dd-112">Describes the status of a **SendNotification** operation response.</span></span> <br/><br/><span data-ttu-id="388dd-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="388dd-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="388dd-114">-成功</span><span class="sxs-lookup"><span data-stu-id="388dd-114">-  Success</span></span>  <br/><span data-ttu-id="388dd-115">-警告</span><span class="sxs-lookup"><span data-stu-id="388dd-115">-  Warning</span></span>  <br/><span data-ttu-id="388dd-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="388dd-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="388dd-117">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="388dd-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="388dd-118">**値**</span><span class="sxs-lookup"><span data-stu-id="388dd-118">**Value**</span></span>|<span data-ttu-id="388dd-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="388dd-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="388dd-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="388dd-120">**Success**</span></span> <br/> |<span data-ttu-id="388dd-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="388dd-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="388dd-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="388dd-122">**Warning**</span></span> <br/> | <span data-ttu-id="388dd-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="388dd-123">Describes a request that was not processed.</span></span> <span data-ttu-id="388dd-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="388dd-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="388dd-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="388dd-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="388dd-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="388dd-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="388dd-127">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="388dd-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="388dd-128">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="388dd-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="388dd-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="388dd-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="388dd-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="388dd-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="388dd-131">クォータを超過しました。</span><span class="sxs-lookup"><span data-stu-id="388dd-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="388dd-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="388dd-132">**Error**</span></span> <br/> | <span data-ttu-id="388dd-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="388dd-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="388dd-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="388dd-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="388dd-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="388dd-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="388dd-136">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="388dd-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="388dd-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="388dd-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="388dd-138">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="388dd-138">-  Attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="388dd-139">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="388dd-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="388dd-140">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="388dd-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="388dd-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="388dd-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="388dd-142">子要素</span><span class="sxs-lookup"><span data-stu-id="388dd-142">Child elements</span></span>

|<span data-ttu-id="388dd-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="388dd-143">**Element**</span></span>|<span data-ttu-id="388dd-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="388dd-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="388dd-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="388dd-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="388dd-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="388dd-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="388dd-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="388dd-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="388dd-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="388dd-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="388dd-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="388dd-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="388dd-150">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="388dd-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="388dd-151">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="388dd-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="388dd-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="388dd-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="388dd-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="388dd-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="388dd-154">通知</span><span class="sxs-lookup"><span data-stu-id="388dd-154">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="388dd-155">サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="388dd-155">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="388dd-156">親要素</span><span class="sxs-lookup"><span data-stu-id="388dd-156">Parent elements</span></span>

|<span data-ttu-id="388dd-157">**要素**</span><span class="sxs-lookup"><span data-stu-id="388dd-157">**Element**</span></span>|<span data-ttu-id="388dd-158">**説明**</span><span class="sxs-lookup"><span data-stu-id="388dd-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="388dd-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="388dd-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="388dd-160">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="388dd-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="388dd-161">テキスト値</span><span class="sxs-lookup"><span data-stu-id="388dd-161">Text value</span></span>

<span data-ttu-id="388dd-162">なし。</span><span class="sxs-lookup"><span data-stu-id="388dd-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="388dd-163">備考</span><span class="sxs-lookup"><span data-stu-id="388dd-163">Remarks</span></span>

<span data-ttu-id="388dd-164">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="388dd-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="388dd-165">要素情報</span><span class="sxs-lookup"><span data-stu-id="388dd-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="388dd-166">名前空間</span><span class="sxs-lookup"><span data-stu-id="388dd-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="388dd-167">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="388dd-167">Schema Name</span></span>  <br/> |<span data-ttu-id="388dd-168">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="388dd-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="388dd-169">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="388dd-169">Validation File</span></span>  <br/> |<span data-ttu-id="388dd-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="388dd-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="388dd-171">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="388dd-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="388dd-172">False</span><span class="sxs-lookup"><span data-stu-id="388dd-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="388dd-173">関連項目</span><span class="sxs-lookup"><span data-stu-id="388dd-173">See also</span></span>

- [<span data-ttu-id="388dd-174">SendNotification</span><span class="sxs-lookup"><span data-stu-id="388dd-174">SendNotification</span></span>](sendnotification.md)
- [<span data-ttu-id="388dd-175">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="388dd-175">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="388dd-176">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="388dd-176">Unsubscribe operation</span></span>](unsubscribe-operation.md)

