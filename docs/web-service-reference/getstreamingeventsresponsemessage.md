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
description: GetStreamingEventsResponseMessage 要素には、1つの GetStreamingEvents 操作要求の状態と結果が含まれています。
ms.openlocfilehash: 055fb7eeb12e241739eb860cecbe398b8a322bd2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459147"
---
# <a name="getstreamingeventsresponsemessage"></a><span data-ttu-id="92d48-103">GetStreamingEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="92d48-103">GetStreamingEventsResponseMessage</span></span>

<span data-ttu-id="92d48-104">**GetStreamingEventsResponseMessage**要素には、1つの[Getstreamingevents 操作](getstreamingevents-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="92d48-104">The **GetStreamingEventsResponseMessage** element contains the status and result of a single [GetStreamingEvents operation](getstreamingevents-operation.md) request.</span></span> 
  
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

 <span data-ttu-id="92d48-105">**Getstreamingイベント Responsemessagetype**</span><span class="sxs-lookup"><span data-stu-id="92d48-105">**GetStreamingEventsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="92d48-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="92d48-106">Attributes and elements</span></span>

<span data-ttu-id="92d48-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="92d48-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="92d48-108">属性</span><span class="sxs-lookup"><span data-stu-id="92d48-108">Attributes</span></span>

|<span data-ttu-id="92d48-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="92d48-109">**Attribute**</span></span>|<span data-ttu-id="92d48-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="92d48-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="92d48-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="92d48-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="92d48-112">[Getstreamingevents 操作](getstreamingevents-operation.md)の応答の状態を記述します。</span><span class="sxs-lookup"><span data-stu-id="92d48-112">Describes the status of a [GetStreamingEvents operation](getstreamingevents-operation.md) response.</span></span> <br/><br/><span data-ttu-id="92d48-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="92d48-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="92d48-114">-成功</span><span class="sxs-lookup"><span data-stu-id="92d48-114">-  Success</span></span>  <br/><span data-ttu-id="92d48-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="92d48-115">-  Warning</span></span>  <br/><span data-ttu-id="92d48-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="92d48-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="92d48-117">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="92d48-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="92d48-118">**値**</span><span class="sxs-lookup"><span data-stu-id="92d48-118">**Value**</span></span>|<span data-ttu-id="92d48-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="92d48-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="92d48-120">Success</span><span class="sxs-lookup"><span data-stu-id="92d48-120">Success</span></span>  <br/> |<span data-ttu-id="92d48-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="92d48-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="92d48-122">警告</span><span class="sxs-lookup"><span data-stu-id="92d48-122">Warning</span></span>  <br/> | <span data-ttu-id="92d48-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="92d48-123">Describes a request that was not processed.</span></span> <span data-ttu-id="92d48-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="92d48-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="92d48-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="92d48-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="92d48-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="92d48-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="92d48-127">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="92d48-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="92d48-128">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="92d48-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="92d48-129">-メールボックスデータベース (MDB) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="92d48-129">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="92d48-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="92d48-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="92d48-131">-クォータを超過しました。</span><span class="sxs-lookup"><span data-stu-id="92d48-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="92d48-132">Error</span><span class="sxs-lookup"><span data-stu-id="92d48-132">Error</span></span>  <br/> | <span data-ttu-id="92d48-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="92d48-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="92d48-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="92d48-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="92d48-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="92d48-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="92d48-136">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="92d48-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="92d48-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="92d48-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="92d48-138">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="92d48-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="92d48-139">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="92d48-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="92d48-140">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="92d48-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="92d48-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="92d48-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="92d48-142">子要素</span><span class="sxs-lookup"><span data-stu-id="92d48-142">Child elements</span></span>

|<span data-ttu-id="92d48-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="92d48-143">**Element**</span></span>|<span data-ttu-id="92d48-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="92d48-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92d48-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="92d48-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="92d48-146">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="92d48-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="92d48-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="92d48-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="92d48-148">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="92d48-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="92d48-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="92d48-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="92d48-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="92d48-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="92d48-151">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="92d48-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="92d48-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="92d48-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="92d48-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="92d48-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="92d48-154">通知</span><span class="sxs-lookup"><span data-stu-id="92d48-154">Notifications</span></span>](notifications.md) <br/> |<span data-ttu-id="92d48-155">サブスクリプションに関する情報と、前回の通知以降に発生したイベントの一覧が含まれています。</span><span class="sxs-lookup"><span data-stu-id="92d48-155">Contains a list of information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
|[<span data-ttu-id="92d48-156">ErrorSubscriptionIds</span><span class="sxs-lookup"><span data-stu-id="92d48-156">ErrorSubscriptionIds</span></span>](errorsubscriptionids.md) <br/> |<span data-ttu-id="92d48-157">無効なサブスクリプション Id のリストが含まれています。</span><span class="sxs-lookup"><span data-stu-id="92d48-157">Contains a list of subscription IDs that are invalid.</span></span>  <br/> |
|[<span data-ttu-id="92d48-158">ConnectionStatus</span><span class="sxs-lookup"><span data-stu-id="92d48-158">ConnectionStatus</span></span>](connectionstatus.md) <br/> |<span data-ttu-id="92d48-159">ストリーミングサブスクリプションの状態について説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="92d48-159">Provides a text description of the status of a streaming subscription.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="92d48-160">親要素</span><span class="sxs-lookup"><span data-stu-id="92d48-160">Parent elements</span></span>

|<span data-ttu-id="92d48-161">**要素**</span><span class="sxs-lookup"><span data-stu-id="92d48-161">**Element**</span></span>|<span data-ttu-id="92d48-162">**説明**</span><span class="sxs-lookup"><span data-stu-id="92d48-162">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="92d48-163">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="92d48-163">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="92d48-164">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="92d48-164">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="92d48-165">テキスト値</span><span class="sxs-lookup"><span data-stu-id="92d48-165">Text value</span></span>

<span data-ttu-id="92d48-166">なし。</span><span class="sxs-lookup"><span data-stu-id="92d48-166">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="92d48-167">注釈</span><span class="sxs-lookup"><span data-stu-id="92d48-167">Remarks</span></span>

<span data-ttu-id="92d48-168">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="92d48-168">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="92d48-169">要素の情報</span><span class="sxs-lookup"><span data-stu-id="92d48-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="92d48-170">Namespace</span><span class="sxs-lookup"><span data-stu-id="92d48-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="92d48-171">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="92d48-171">Schema Name</span></span>  <br/> |<span data-ttu-id="92d48-172">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="92d48-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="92d48-173">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="92d48-173">Validation File</span></span>  <br/> |<span data-ttu-id="92d48-174">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="92d48-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="92d48-175">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="92d48-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="92d48-176">正しくない</span><span class="sxs-lookup"><span data-stu-id="92d48-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="92d48-177">関連項目</span><span class="sxs-lookup"><span data-stu-id="92d48-177">See also</span></span>

- [<span data-ttu-id="92d48-178">GetStreamingEvents</span><span class="sxs-lookup"><span data-stu-id="92d48-178">GetStreamingEvents</span></span>](getstreamingevents.md) 
- [<span data-ttu-id="92d48-179">GetStreamingEventsResponse</span><span class="sxs-lookup"><span data-stu-id="92d48-179">GetStreamingEventsResponse</span></span>](getstreamingeventsresponse.md)
- [<span data-ttu-id="92d48-180">GetStreamingEvents の操作</span><span class="sxs-lookup"><span data-stu-id="92d48-180">GetStreamingEvents operation</span></span>](getstreamingevents-operation.md)

