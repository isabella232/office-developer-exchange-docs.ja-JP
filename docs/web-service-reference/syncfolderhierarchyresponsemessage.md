---
title: SyncFolderHierarchyResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SyncFolderHierarchyResponseMessage
api_type:
- schema
ms.assetid: ab96c649-1005-401c-9d1c-9917f0b19a60
description: SyncFolderHierarchyResponseMessage 要素には、状態および 1 つの SyncFolderHierarchy 操作要求の結果が含まれています。
ms.openlocfilehash: e4141299b128ffb7f67c55bbb09390b77a79e043
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839637"
---
# <a name="syncfolderhierarchyresponsemessage"></a><span data-ttu-id="2a3cf-103">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2a3cf-103">SyncFolderHierarchyResponseMessage</span></span>

<span data-ttu-id="2a3cf-104">**SyncFolderHierarchyResponseMessage**要素には、状態および 1 つの結果が含まれています[SyncFolderHierarchy 操作](syncfolderhierarchy-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-104">The **SyncFolderHierarchyResponseMessage** element contains the status and result of a single [SyncFolderHierarchy operation](syncfolderhierarchy-operation.md) request.</span></span> 
  
- [<span data-ttu-id="2a3cf-105">SyncFolderHierarchyResponse</span><span class="sxs-lookup"><span data-stu-id="2a3cf-105">SyncFolderHierarchyResponse</span></span>](syncfolderhierarchyresponse.md) 
- [<span data-ttu-id="2a3cf-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2a3cf-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="2a3cf-107">SyncFolderHierarchyResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2a3cf-107">SyncFolderHierarchyResponseMessage</span></span>](syncfolderhierarchyresponsemessage.md)
  
```xml
<SyncFolderHierarchyResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <SyncState/>
   <IncludesLastFolderInRange/>
   <Changes/>
</SyncFolderHierarchyResponseMessage>
```

 <span data-ttu-id="2a3cf-108">**SyncFolderHierarchyResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="2a3cf-108">**SyncFolderHierarchyResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="2a3cf-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="2a3cf-109">Attributes and elements</span></span>

<span data-ttu-id="2a3cf-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2a3cf-111">属性</span><span class="sxs-lookup"><span data-stu-id="2a3cf-111">Attributes</span></span>

|<span data-ttu-id="2a3cf-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="2a3cf-112">**Attribute**</span></span>|<span data-ttu-id="2a3cf-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="2a3cf-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2a3cf-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="2a3cf-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="2a3cf-115">[SyncFolderHierarchy 操作](syncfolderhierarchy-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-115">Describes the status of a [SyncFolderHierarchy operation](syncfolderhierarchy-operation.md) response.</span></span> <br/><br/><span data-ttu-id="2a3cf-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-116">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="2a3cf-117">-成功</span><span class="sxs-lookup"><span data-stu-id="2a3cf-117">-  Success</span></span>  <br/><span data-ttu-id="2a3cf-118">-警告</span><span class="sxs-lookup"><span data-stu-id="2a3cf-118">-  Warning</span></span>  <br/><span data-ttu-id="2a3cf-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="2a3cf-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="2a3cf-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="2a3cf-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="2a3cf-121">**値**</span><span class="sxs-lookup"><span data-stu-id="2a3cf-121">**Value**</span></span>|<span data-ttu-id="2a3cf-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="2a3cf-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2a3cf-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="2a3cf-123">**Success**</span></span> <br/> |<span data-ttu-id="2a3cf-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="2a3cf-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="2a3cf-125">**Warning**</span></span> <br/> | <span data-ttu-id="2a3cf-126">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-126">Describes a request that was not processed.</span></span> <span data-ttu-id="2a3cf-127">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="2a3cf-128">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="2a3cf-129">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="2a3cf-130">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="2a3cf-131">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="2a3cf-132">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="2a3cf-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-133">-  A password has expired.</span></span>  <br/><span data-ttu-id="2a3cf-134">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="2a3cf-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="2a3cf-135">**Error**</span></span> <br/> | <span data-ttu-id="2a3cf-136">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="2a3cf-137">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="2a3cf-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="2a3cf-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="2a3cf-139">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="2a3cf-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="2a3cf-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="2a3cf-141">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="2a3cf-142">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="2a3cf-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="2a3cf-143">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="2a3cf-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="2a3cf-144">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2a3cf-145">子要素</span><span class="sxs-lookup"><span data-stu-id="2a3cf-145">Child elements</span></span>

|<span data-ttu-id="2a3cf-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="2a3cf-146">**Element**</span></span>|<span data-ttu-id="2a3cf-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="2a3cf-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a3cf-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="2a3cf-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="2a3cf-149">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="2a3cf-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2a3cf-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="2a3cf-151">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="2a3cf-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="2a3cf-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="2a3cf-153">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="2a3cf-154">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="2a3cf-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="2a3cf-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="2a3cf-156">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="2a3cf-157">同期状態</span><span class="sxs-lookup"><span data-stu-id="2a3cf-157">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="2a3cf-158">各成功した要求の後に更新された同期データの base64 でエンコードされたフォームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-158">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="2a3cf-159">これを使用して、同期の状態を識別します。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-159">This is used to identify the synchronization state.</span></span>  <br/> |
|[<span data-ttu-id="2a3cf-160">IncludesLastFolderInRange</span><span class="sxs-lookup"><span data-stu-id="2a3cf-160">IncludesLastFolderInRange</span></span>](includeslastfolderinrange.md) <br/> |<span data-ttu-id="2a3cf-161">最後の項目を同期するが、応答に含まれているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-161">Indicates whether the last item to synchronize has been included in the response.</span></span>  <br/> |
|[<span data-ttu-id="2a3cf-162">(階層) の変更</span><span class="sxs-lookup"><span data-stu-id="2a3cf-162">Changes (Hierarchy)</span></span>](changes-hierarchy.md) <br/> |<span data-ttu-id="2a3cf-163">クライアント上のアイテムと、Exchange サーバー上のアイテム間の相違点の種類を表すの種類の変更の順序の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-163">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2a3cf-164">親要素</span><span class="sxs-lookup"><span data-stu-id="2a3cf-164">Parent elements</span></span>

|<span data-ttu-id="2a3cf-165">**要素**</span><span class="sxs-lookup"><span data-stu-id="2a3cf-165">**Element**</span></span>|<span data-ttu-id="2a3cf-166">**説明**</span><span class="sxs-lookup"><span data-stu-id="2a3cf-166">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2a3cf-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2a3cf-167">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="2a3cf-168">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-168">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2a3cf-169">備考</span><span class="sxs-lookup"><span data-stu-id="2a3cf-169">Remarks</span></span>

<span data-ttu-id="2a3cf-170">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2a3cf-170">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2a3cf-171">要素情報</span><span class="sxs-lookup"><span data-stu-id="2a3cf-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2a3cf-172">名前空間</span><span class="sxs-lookup"><span data-stu-id="2a3cf-172">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2a3cf-173">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2a3cf-173">Schema Name</span></span>  <br/> |<span data-ttu-id="2a3cf-174">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="2a3cf-174">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2a3cf-175">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2a3cf-175">Validation File</span></span>  <br/> |<span data-ttu-id="2a3cf-176">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="2a3cf-176">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2a3cf-177">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2a3cf-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="2a3cf-178">False</span><span class="sxs-lookup"><span data-stu-id="2a3cf-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2a3cf-179">関連項目</span><span class="sxs-lookup"><span data-stu-id="2a3cf-179">See also</span></span>

- [<span data-ttu-id="2a3cf-180">SyncFolderHierarchy 操作</span><span class="sxs-lookup"><span data-stu-id="2a3cf-180">SyncFolderHierarchy operation</span></span>](syncfolderhierarchy-operation.md)
- [<span data-ttu-id="2a3cf-181">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="2a3cf-181">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

