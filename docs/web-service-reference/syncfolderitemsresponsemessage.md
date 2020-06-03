---
title: SyncFolderItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderItemsResponseMessage
api_type:
- schema
ms.assetid: f58e773f-94a7-4729-90f0-ac4c71b4ba59
description: SyncFolderItemsResponseMessage 要素には、単一の SyncFolderItems 操作要求の状態と結果が含まれています。
ms.openlocfilehash: 87de1b679fad4affa29a6dfdea72f5312b9191d5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463042"
---
# <a name="syncfolderitemsresponsemessage"></a><span data-ttu-id="7a77c-103">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7a77c-103">SyncFolderItemsResponseMessage</span></span>

<span data-ttu-id="7a77c-104">**SyncFolderItemsResponseMessage**要素には、単一の[syncfolderitems 操作](syncfolderitems-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7a77c-104">The **SyncFolderItemsResponseMessage** element contains the status and result of a single [SyncFolderItems operation](syncfolderitems-operation.md) request.</span></span> 
  
- [<span data-ttu-id="7a77c-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="7a77c-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md) 
- [<span data-ttu-id="7a77c-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7a77c-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="7a77c-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7a77c-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
```xml
<SyncFolderItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SyncState/>
   <IncludesLastItemInRange/>
   <Changes/>
</SyncFolderItemsResponseMessage>
```

 <span data-ttu-id="7a77c-108">**SyncFolderItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="7a77c-108">**SyncFolderItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7a77c-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="7a77c-109">Attributes and elements</span></span>

<span data-ttu-id="7a77c-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7a77c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7a77c-111">属性</span><span class="sxs-lookup"><span data-stu-id="7a77c-111">Attributes</span></span>

|<span data-ttu-id="7a77c-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="7a77c-112">**Attribute**</span></span>|<span data-ttu-id="7a77c-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="7a77c-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7a77c-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="7a77c-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="7a77c-115">[Syncfolderitems 操作](syncfolderitems-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="7a77c-115">Describes the status of a [SyncFolderItems operation](syncfolderitems-operation.md) response.</span></span> <br/><br/><span data-ttu-id="7a77c-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="7a77c-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="7a77c-117">-成功</span><span class="sxs-lookup"><span data-stu-id="7a77c-117">-  Success</span></span>  <br/><span data-ttu-id="7a77c-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="7a77c-118">-  Warning</span></span>  <br/><span data-ttu-id="7a77c-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="7a77c-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="7a77c-120">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="7a77c-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="7a77c-121">**値**</span><span class="sxs-lookup"><span data-stu-id="7a77c-121">**Value**</span></span>|<span data-ttu-id="7a77c-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="7a77c-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7a77c-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="7a77c-123">**Success**</span></span> <br/> |<span data-ttu-id="7a77c-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="7a77c-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="7a77c-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="7a77c-125">**Warning**</span></span> <br/> | <span data-ttu-id="7a77c-126">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="7a77c-126">Describes a request that was not processed.</span></span> <span data-ttu-id="7a77c-127">要求内のアイテムの処理中にエラーが発生し、後続のアイテムを処理できない場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="7a77c-127">A warning may be returned if an error occurred while processing an item in the request and subsequent items cannot be processed.</span></span> <br/><br/><span data-ttu-id="7a77c-128">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7a77c-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="7a77c-129">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="7a77c-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="7a77c-130">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="7a77c-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="7a77c-131">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="7a77c-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="7a77c-132">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="7a77c-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="7a77c-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="7a77c-133">-  A password has expired.</span></span>  <br/><span data-ttu-id="7a77c-134">-クォータを超過しました。</span><span class="sxs-lookup"><span data-stu-id="7a77c-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="7a77c-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="7a77c-135">**Error**</span></span> <br/> | <span data-ttu-id="7a77c-136">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="7a77c-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="7a77c-137">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7a77c-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="7a77c-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="7a77c-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="7a77c-139">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="7a77c-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="7a77c-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="7a77c-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="7a77c-141">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="7a77c-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="7a77c-142">-クライアントによる承認されていないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="7a77c-142">-  Any unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="7a77c-143">-有効なクライアント側の呼び出しに応答して、サーバー側で障害が発生した</span><span class="sxs-lookup"><span data-stu-id="7a77c-143">-  Any server-side failure in response to a valid client-side call</span></span>  <br/>  <br/><span data-ttu-id="7a77c-144">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7a77c-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7a77c-145">子要素</span><span class="sxs-lookup"><span data-stu-id="7a77c-145">Child elements</span></span>

|<span data-ttu-id="7a77c-146">**Element**</span><span class="sxs-lookup"><span data-stu-id="7a77c-146">**Element**</span></span>|<span data-ttu-id="7a77c-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="7a77c-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a77c-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="7a77c-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7a77c-149">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="7a77c-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7a77c-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7a77c-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7a77c-151">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="7a77c-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="7a77c-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7a77c-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7a77c-153">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="7a77c-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="7a77c-154">値0が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7a77c-154">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="7a77c-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="7a77c-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7a77c-156">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="7a77c-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="7a77c-157">SyncState</span><span class="sxs-lookup"><span data-stu-id="7a77c-157">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="7a77c-158">要求が成功するたびに更新される同期データの base64 でエンコードされた形式が含まれます。</span><span class="sxs-lookup"><span data-stu-id="7a77c-158">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="7a77c-159">これは、同期状態を識別するために使用されます。</span><span class="sxs-lookup"><span data-stu-id="7a77c-159">This is used to identify the synchronization state.</span></span>  <br/> |
|[<span data-ttu-id="7a77c-160">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="7a77c-160">IncludesLastItemInRange</span></span>](includeslastiteminrange.md) <br/> |<span data-ttu-id="7a77c-161">同期する最後の項目が応答に含まれているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="7a77c-161">Indicates whether the last item to synchronize has been included in the response.</span></span>  <br/> |
|[<span data-ttu-id="7a77c-162">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="7a77c-162">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="7a77c-163">クライアント上のアイテムと Exchange サーバー上のアイテムの間の相違点の種類を表す、変更の種類のシーケンス配列を含みます。</span><span class="sxs-lookup"><span data-stu-id="7a77c-163">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7a77c-164">親要素</span><span class="sxs-lookup"><span data-stu-id="7a77c-164">Parent elements</span></span>

|<span data-ttu-id="7a77c-165">**要素**</span><span class="sxs-lookup"><span data-stu-id="7a77c-165">**Element**</span></span>|<span data-ttu-id="7a77c-166">**説明**</span><span class="sxs-lookup"><span data-stu-id="7a77c-166">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7a77c-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7a77c-167">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="7a77c-168">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="7a77c-168">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7a77c-169">注釈</span><span class="sxs-lookup"><span data-stu-id="7a77c-169">Remarks</span></span>

<span data-ttu-id="7a77c-170">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7a77c-170">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7a77c-171">要素の情報</span><span class="sxs-lookup"><span data-stu-id="7a77c-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7a77c-172">Namespace</span><span class="sxs-lookup"><span data-stu-id="7a77c-172">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7a77c-173">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7a77c-173">Schema Name</span></span>  <br/> |<span data-ttu-id="7a77c-174">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="7a77c-174">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7a77c-175">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7a77c-175">Validation File</span></span>  <br/> |<span data-ttu-id="7a77c-176">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="7a77c-176">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7a77c-177">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7a77c-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="7a77c-178">正しくない</span><span class="sxs-lookup"><span data-stu-id="7a77c-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7a77c-179">関連項目</span><span class="sxs-lookup"><span data-stu-id="7a77c-179">See also</span></span>

- [<span data-ttu-id="7a77c-180">SyncFolderItems 操作</span><span class="sxs-lookup"><span data-stu-id="7a77c-180">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="7a77c-181">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="7a77c-181">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

