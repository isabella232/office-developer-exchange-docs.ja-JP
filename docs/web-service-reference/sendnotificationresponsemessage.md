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
description: SendNotificationResponseMessage 要素には、1回の SendNotification 操作要求の状態と結果が含まれています。
ms.openlocfilehash: cf44a09624d1b8a7341f9dd98db48472fea7393b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462109"
---
# <a name="sendnotificationresponsemessage"></a><span data-ttu-id="13fd3-103">SendNotificationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="13fd3-103">SendNotificationResponseMessage</span></span>

<span data-ttu-id="13fd3-104">**SendNotificationResponseMessage**要素には、1回の**sendnotification**操作要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="13fd3-104">The **SendNotificationResponseMessage** element contains the status and result of a single **SendNotification** operation request.</span></span> 
  
```xml
<SendNotificationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notification/>
</SendNotificationResponseMessage>
```

 <span data-ttu-id="13fd3-105">**SendNotificationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="13fd3-105">**SendNotificationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="13fd3-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="13fd3-106">Attributes and elements</span></span>

<span data-ttu-id="13fd3-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="13fd3-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="13fd3-108">属性</span><span class="sxs-lookup"><span data-stu-id="13fd3-108">Attributes</span></span>

|<span data-ttu-id="13fd3-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="13fd3-109">**Attribute**</span></span>|<span data-ttu-id="13fd3-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="13fd3-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="13fd3-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="13fd3-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="13fd3-112">**Sendnotification**操作応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="13fd3-112">Describes the status of a **SendNotification** operation response.</span></span> <br/><br/><span data-ttu-id="13fd3-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="13fd3-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="13fd3-114">-成功</span><span class="sxs-lookup"><span data-stu-id="13fd3-114">-  Success</span></span>  <br/><span data-ttu-id="13fd3-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="13fd3-115">-  Warning</span></span>  <br/><span data-ttu-id="13fd3-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="13fd3-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="13fd3-117">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="13fd3-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="13fd3-118">**値**</span><span class="sxs-lookup"><span data-stu-id="13fd3-118">**Value**</span></span>|<span data-ttu-id="13fd3-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="13fd3-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="13fd3-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="13fd3-120">**Success**</span></span> <br/> |<span data-ttu-id="13fd3-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="13fd3-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="13fd3-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="13fd3-122">**Warning**</span></span> <br/> | <span data-ttu-id="13fd3-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="13fd3-123">Describes a request that was not processed.</span></span> <span data-ttu-id="13fd3-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="13fd3-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="13fd3-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="13fd3-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="13fd3-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="13fd3-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="13fd3-127">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="13fd3-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="13fd3-128">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="13fd3-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="13fd3-129">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="13fd3-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="13fd3-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="13fd3-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="13fd3-131">-クォータを超過しました。</span><span class="sxs-lookup"><span data-stu-id="13fd3-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="13fd3-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="13fd3-132">**Error**</span></span> <br/> | <span data-ttu-id="13fd3-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="13fd3-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="13fd3-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="13fd3-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="13fd3-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="13fd3-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="13fd3-136">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="13fd3-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="13fd3-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="13fd3-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="13fd3-138">-コンテキスト内で有効でない属性または要素</span><span class="sxs-lookup"><span data-stu-id="13fd3-138">-  Attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="13fd3-139">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="13fd3-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="13fd3-140">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="13fd3-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="13fd3-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="13fd3-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="13fd3-142">子要素</span><span class="sxs-lookup"><span data-stu-id="13fd3-142">Child elements</span></span>

|<span data-ttu-id="13fd3-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="13fd3-143">**Element**</span></span>|<span data-ttu-id="13fd3-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="13fd3-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13fd3-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="13fd3-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="13fd3-146">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="13fd3-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="13fd3-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="13fd3-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="13fd3-148">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="13fd3-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="13fd3-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="13fd3-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="13fd3-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="13fd3-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="13fd3-151">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="13fd3-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="13fd3-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="13fd3-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="13fd3-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="13fd3-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="13fd3-154">通知</span><span class="sxs-lookup"><span data-stu-id="13fd3-154">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="13fd3-155">サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="13fd3-155">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="13fd3-156">親要素</span><span class="sxs-lookup"><span data-stu-id="13fd3-156">Parent elements</span></span>

|<span data-ttu-id="13fd3-157">**要素**</span><span class="sxs-lookup"><span data-stu-id="13fd3-157">**Element**</span></span>|<span data-ttu-id="13fd3-158">**説明**</span><span class="sxs-lookup"><span data-stu-id="13fd3-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="13fd3-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="13fd3-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="13fd3-160">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="13fd3-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="13fd3-161">テキスト値</span><span class="sxs-lookup"><span data-stu-id="13fd3-161">Text value</span></span>

<span data-ttu-id="13fd3-162">なし。</span><span class="sxs-lookup"><span data-stu-id="13fd3-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="13fd3-163">注釈</span><span class="sxs-lookup"><span data-stu-id="13fd3-163">Remarks</span></span>

<span data-ttu-id="13fd3-164">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="13fd3-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="13fd3-165">要素の情報</span><span class="sxs-lookup"><span data-stu-id="13fd3-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="13fd3-166">Namespace</span><span class="sxs-lookup"><span data-stu-id="13fd3-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="13fd3-167">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="13fd3-167">Schema Name</span></span>  <br/> |<span data-ttu-id="13fd3-168">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="13fd3-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="13fd3-169">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="13fd3-169">Validation File</span></span>  <br/> |<span data-ttu-id="13fd3-170">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="13fd3-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="13fd3-171">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="13fd3-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="13fd3-172">正しくない</span><span class="sxs-lookup"><span data-stu-id="13fd3-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="13fd3-173">関連項目</span><span class="sxs-lookup"><span data-stu-id="13fd3-173">See also</span></span>

- [<span data-ttu-id="13fd3-174">SendNotification</span><span class="sxs-lookup"><span data-stu-id="13fd3-174">SendNotification</span></span>](sendnotification.md)
- [<span data-ttu-id="13fd3-175">サブスクライブ操作</span><span class="sxs-lookup"><span data-stu-id="13fd3-175">Subscribe operation</span></span>](subscribe-operation.md)
- [<span data-ttu-id="13fd3-176">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="13fd3-176">Unsubscribe operation</span></span>](unsubscribe-operation.md)

