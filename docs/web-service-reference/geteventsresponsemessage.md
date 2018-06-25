---
title: GetEventsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetEventsResponseMessage
api_type:
- schema
ms.assetid: d433977f-b86a-499e-b9c3-f405ac229358
description: GetEventsResponseMessage 要素には、状態および 1 つの GetEvents 操作要求の結果が含まれています。
ms.openlocfilehash: 90e79194182f61ba7298ef67b1070b1aa239073d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760715"
---
# <a name="geteventsresponsemessage"></a><span data-ttu-id="7e25e-103">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7e25e-103">GetEventsResponseMessage</span></span>

<span data-ttu-id="7e25e-104">**GetEventsResponseMessage**要素には、状態および 1 つの結果が含まれている[GetEvents 操作](getevents-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="7e25e-104">The **GetEventsResponseMessage** element contains the status and result of a single [GetEvents operation](getevents-operation.md) request.</span></span> 
  
```xml
<GetEventsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notification/>
</GetEventsResponseMessage>
```

 <span data-ttu-id="7e25e-105">**GetEventsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="7e25e-105">**GetEventsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7e25e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7e25e-106">Attributes and elements</span></span>

<span data-ttu-id="7e25e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7e25e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7e25e-108">属性</span><span class="sxs-lookup"><span data-stu-id="7e25e-108">Attributes</span></span>

|<span data-ttu-id="7e25e-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="7e25e-109">**Attribute**</span></span>|<span data-ttu-id="7e25e-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e25e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7e25e-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="7e25e-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="7e25e-112">[GetEvents 操作](getevents-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7e25e-112">Describes the status of a [GetEvents operation](getevents-operation.md) response.</span></span> <br/><br/><span data-ttu-id="7e25e-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="7e25e-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="7e25e-114">-成功</span><span class="sxs-lookup"><span data-stu-id="7e25e-114">-  Success</span></span>  <br/><span data-ttu-id="7e25e-115">-警告</span><span class="sxs-lookup"><span data-stu-id="7e25e-115">-  Warning</span></span>  <br/><span data-ttu-id="7e25e-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="7e25e-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="7e25e-117">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="7e25e-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="7e25e-118">**値**</span><span class="sxs-lookup"><span data-stu-id="7e25e-118">**Value**</span></span>|<span data-ttu-id="7e25e-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e25e-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7e25e-120">成功</span><span class="sxs-lookup"><span data-stu-id="7e25e-120">Success</span></span>  <br/> |<span data-ttu-id="7e25e-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7e25e-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="7e25e-122">警告</span><span class="sxs-lookup"><span data-stu-id="7e25e-122">Warning</span></span>  <br/> | <span data-ttu-id="7e25e-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7e25e-123">Describes a request that was not processed.</span></span> <span data-ttu-id="7e25e-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="7e25e-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="7e25e-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7e25e-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="7e25e-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="7e25e-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="7e25e-127">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="7e25e-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="7e25e-128">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="7e25e-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="7e25e-129">-メールボックス データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="7e25e-129">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="7e25e-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="7e25e-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="7e25e-131">クォータを超過しました。</span><span class="sxs-lookup"><span data-stu-id="7e25e-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="7e25e-132">エラー</span><span class="sxs-lookup"><span data-stu-id="7e25e-132">Error</span></span>  <br/> | <span data-ttu-id="7e25e-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7e25e-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="7e25e-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="7e25e-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="7e25e-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="7e25e-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="7e25e-136">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="7e25e-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="7e25e-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="7e25e-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="7e25e-138">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="7e25e-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="7e25e-139">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="7e25e-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="7e25e-140">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="7e25e-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="7e25e-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="7e25e-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7e25e-142">子要素</span><span class="sxs-lookup"><span data-stu-id="7e25e-142">Child elements</span></span>

|<span data-ttu-id="7e25e-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="7e25e-143">**Element**</span></span>|<span data-ttu-id="7e25e-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e25e-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e25e-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="7e25e-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7e25e-146">応答のステータスの説明テキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="7e25e-146">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7e25e-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7e25e-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7e25e-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="7e25e-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="7e25e-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7e25e-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7e25e-150">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="7e25e-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="7e25e-151">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e25e-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="7e25e-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="7e25e-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7e25e-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="7e25e-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="7e25e-154">通知</span><span class="sxs-lookup"><span data-stu-id="7e25e-154">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7e25e-155">サブスクリプションおよび最後の通知以降に発生したイベントに関する情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e25e-155">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7e25e-156">親要素</span><span class="sxs-lookup"><span data-stu-id="7e25e-156">Parent elements</span></span>

|<span data-ttu-id="7e25e-157">**要素**</span><span class="sxs-lookup"><span data-stu-id="7e25e-157">**Element**</span></span>|<span data-ttu-id="7e25e-158">**説明**</span><span class="sxs-lookup"><span data-stu-id="7e25e-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7e25e-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7e25e-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="7e25e-160">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7e25e-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7e25e-161">備考</span><span class="sxs-lookup"><span data-stu-id="7e25e-161">Remarks</span></span>

<span data-ttu-id="7e25e-162">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7e25e-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7e25e-163">要素情報</span><span class="sxs-lookup"><span data-stu-id="7e25e-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7e25e-164">名前空間</span><span class="sxs-lookup"><span data-stu-id="7e25e-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7e25e-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7e25e-165">Schema Name</span></span>  <br/> |<span data-ttu-id="7e25e-166">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="7e25e-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7e25e-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7e25e-167">Validation File</span></span>  <br/> |<span data-ttu-id="7e25e-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7e25e-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7e25e-169">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7e25e-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="7e25e-170">False</span><span class="sxs-lookup"><span data-stu-id="7e25e-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7e25e-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="7e25e-171">See also</span></span>

- [<span data-ttu-id="7e25e-172">GetEvents</span><span class="sxs-lookup"><span data-stu-id="7e25e-172">GetEvents</span></span>](getevents.md) 
- [<span data-ttu-id="7e25e-173">GetEventsResponse</span><span class="sxs-lookup"><span data-stu-id="7e25e-173">GetEventsResponse</span></span>](geteventsresponse.md)
- [<span data-ttu-id="7e25e-174">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="7e25e-174">GetEvents operation</span></span>](getevents-operation.md)

