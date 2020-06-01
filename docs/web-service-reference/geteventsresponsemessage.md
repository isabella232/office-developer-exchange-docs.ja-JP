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
description: GetEventsResponseMessage 要素には、1つの GetEvents 操作要求の状態と結果が含まれています。
ms.openlocfilehash: d307aa1f5234ab5a7a2527c55f5e48814ea2687b
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462858"
---
# <a name="geteventsresponsemessage"></a><span data-ttu-id="2a910-103">GetEventsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2a910-103">GetEventsResponseMessage</span></span>

<span data-ttu-id="2a910-104">**GetEventsResponseMessage**要素には、1つの[GetEvents 操作](getevents-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2a910-104">The **GetEventsResponseMessage** element contains the status and result of a single [GetEvents operation](getevents-operation.md) request.</span></span> 
  
```xml
<GetEventsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Notification/>
</GetEventsResponseMessage>
```

 <span data-ttu-id="2a910-105">**Getイベント Responsemessagetype**</span><span class="sxs-lookup"><span data-stu-id="2a910-105">**GetEventsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2a910-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2a910-106">Attributes and elements</span></span>

<span data-ttu-id="2a910-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2a910-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a910-108">属性</span><span class="sxs-lookup"><span data-stu-id="2a910-108">Attributes</span></span>

|<span data-ttu-id="2a910-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="2a910-109">**Attribute**</span></span>|<span data-ttu-id="2a910-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="2a910-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2a910-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="2a910-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="2a910-112">[GetEvents 操作](getevents-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="2a910-112">Describes the status of a [GetEvents operation](getevents-operation.md) response.</span></span> <br/><br/><span data-ttu-id="2a910-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="2a910-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="2a910-114">-成功</span><span class="sxs-lookup"><span data-stu-id="2a910-114">-  Success</span></span>  <br/><span data-ttu-id="2a910-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="2a910-115">-  Warning</span></span>  <br/><span data-ttu-id="2a910-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="2a910-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="2a910-117">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="2a910-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="2a910-118">**値**</span><span class="sxs-lookup"><span data-stu-id="2a910-118">**Value**</span></span>|<span data-ttu-id="2a910-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="2a910-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2a910-120">Success</span><span class="sxs-lookup"><span data-stu-id="2a910-120">Success</span></span>  <br/> |<span data-ttu-id="2a910-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="2a910-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="2a910-122">警告</span><span class="sxs-lookup"><span data-stu-id="2a910-122">Warning</span></span>  <br/> | <span data-ttu-id="2a910-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="2a910-123">Describes a request that was not processed.</span></span> <span data-ttu-id="2a910-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2a910-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="2a910-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2a910-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="2a910-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="2a910-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="2a910-127">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="2a910-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="2a910-128">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="2a910-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="2a910-129">-メールボックスデータベース (MDB) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="2a910-129">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="2a910-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="2a910-130">-  A password has expired.</span></span>  <br/><span data-ttu-id="2a910-131">-クォータを超過しました。</span><span class="sxs-lookup"><span data-stu-id="2a910-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="2a910-132">Error</span><span class="sxs-lookup"><span data-stu-id="2a910-132">Error</span></span>  <br/> | <span data-ttu-id="2a910-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="2a910-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="2a910-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2a910-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="2a910-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="2a910-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="2a910-136">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="2a910-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="2a910-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="2a910-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="2a910-138">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="2a910-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="2a910-139">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="2a910-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="2a910-140">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="2a910-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="2a910-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2a910-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2a910-142">子要素</span><span class="sxs-lookup"><span data-stu-id="2a910-142">Child elements</span></span>

|<span data-ttu-id="2a910-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="2a910-143">**Element**</span></span>|<span data-ttu-id="2a910-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="2a910-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a910-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="2a910-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="2a910-146">応答の状態の説明をテキストで提供します。</span><span class="sxs-lookup"><span data-stu-id="2a910-146">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="2a910-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2a910-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="2a910-148">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="2a910-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="2a910-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="2a910-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="2a910-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="2a910-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="2a910-151">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2a910-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="2a910-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="2a910-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="2a910-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="2a910-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="2a910-154">通知</span><span class="sxs-lookup"><span data-stu-id="2a910-154">Notification</span></span>](notification-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2a910-155">サブスクリプションに関する情報、および前回の通知以降に発生したイベントに関する情報が含まれます。</span><span class="sxs-lookup"><span data-stu-id="2a910-155">Contains information about the subscription and the events that have occurred since the last notification.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2a910-156">親要素</span><span class="sxs-lookup"><span data-stu-id="2a910-156">Parent elements</span></span>

|<span data-ttu-id="2a910-157">**要素**</span><span class="sxs-lookup"><span data-stu-id="2a910-157">**Element**</span></span>|<span data-ttu-id="2a910-158">**説明**</span><span class="sxs-lookup"><span data-stu-id="2a910-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a910-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2a910-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="2a910-160">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="2a910-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2a910-161">注釈</span><span class="sxs-lookup"><span data-stu-id="2a910-161">Remarks</span></span>

<span data-ttu-id="2a910-162">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="2a910-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2a910-163">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2a910-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2a910-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="2a910-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2a910-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2a910-165">Schema Name</span></span>  <br/> |<span data-ttu-id="2a910-166">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2a910-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2a910-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2a910-167">Validation File</span></span>  <br/> |<span data-ttu-id="2a910-168">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2a910-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2a910-169">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2a910-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="2a910-170">正しくない</span><span class="sxs-lookup"><span data-stu-id="2a910-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2a910-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="2a910-171">See also</span></span>

- [<span data-ttu-id="2a910-172">GetEvents</span><span class="sxs-lookup"><span data-stu-id="2a910-172">GetEvents</span></span>](getevents.md) 
- [<span data-ttu-id="2a910-173">Getイベント応答</span><span class="sxs-lookup"><span data-stu-id="2a910-173">GetEventsResponse</span></span>](geteventsresponse.md)
- [<span data-ttu-id="2a910-174">GetEvents 操作</span><span class="sxs-lookup"><span data-stu-id="2a910-174">GetEvents operation</span></span>](getevents-operation.md)

