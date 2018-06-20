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
description: SyncFolderItemsResponseMessage 要素には、状態および 1 つの SyncFolderItems 操作要求の結果が含まれています。
ms.openlocfilehash: 9bb32232143df56ad9de93480e10a5941e68025a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839644"
---
# <a name="syncfolderitemsresponsemessage"></a><span data-ttu-id="56def-103">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="56def-103">SyncFolderItemsResponseMessage</span></span>

<span data-ttu-id="56def-104">**SyncFolderItemsResponseMessage**要素には、状態および 1 つの結果が含まれている[SyncFolderItems の操作](syncfolderitems-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="56def-104">The **SyncFolderItemsResponseMessage** element contains the status and result of a single [SyncFolderItems operation](syncfolderitems-operation.md) request.</span></span> 
  
- [<span data-ttu-id="56def-105">SyncFolderItemsResponse</span><span class="sxs-lookup"><span data-stu-id="56def-105">SyncFolderItemsResponse</span></span>](syncfolderitemsresponse.md) 
- [<span data-ttu-id="56def-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="56def-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="56def-107">SyncFolderItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="56def-107">SyncFolderItemsResponseMessage</span></span>](syncfolderitemsresponsemessage.md)
  
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

 <span data-ttu-id="56def-108">**SyncFolderItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="56def-108">**SyncFolderItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="56def-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="56def-109">Attributes and elements</span></span>

<span data-ttu-id="56def-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="56def-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="56def-111">属性</span><span class="sxs-lookup"><span data-stu-id="56def-111">Attributes</span></span>

|<span data-ttu-id="56def-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="56def-112">**Attribute**</span></span>|<span data-ttu-id="56def-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="56def-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="56def-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="56def-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="56def-115">[SyncFolderItems 操作](syncfolderitems-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="56def-115">Describes the status of a [SyncFolderItems operation](syncfolderitems-operation.md) response.</span></span> <br/><br/><span data-ttu-id="56def-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="56def-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="56def-117">-成功</span><span class="sxs-lookup"><span data-stu-id="56def-117">-  Success</span></span>  <br/><span data-ttu-id="56def-118">-警告</span><span class="sxs-lookup"><span data-stu-id="56def-118">-  Warning</span></span>  <br/><span data-ttu-id="56def-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="56def-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="56def-120">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="56def-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="56def-121">**値**</span><span class="sxs-lookup"><span data-stu-id="56def-121">**Value**</span></span>|<span data-ttu-id="56def-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="56def-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="56def-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="56def-123">**Success**</span></span> <br/> |<span data-ttu-id="56def-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="56def-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="56def-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="56def-125">**Warning**</span></span> <br/> | <span data-ttu-id="56def-126">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="56def-126">Describes a request that was not processed.</span></span> <span data-ttu-id="56def-127">警告が表示される場合は、要求内のアイテムの処理中にエラーが発生しましたし、それ以降の項目を処理することはできません。</span><span class="sxs-lookup"><span data-stu-id="56def-127">A warning may be returned if an error occurred while processing an item in the request and subsequent items cannot be processed.</span></span> <br/><br/><span data-ttu-id="56def-128">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="56def-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="56def-129">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="56def-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="56def-130">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="56def-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="56def-131">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="56def-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="56def-132">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="56def-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="56def-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="56def-133">-  A password has expired.</span></span>  <br/><span data-ttu-id="56def-134">クォータを超過しました。</span><span class="sxs-lookup"><span data-stu-id="56def-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="56def-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="56def-135">**Error**</span></span> <br/> | <span data-ttu-id="56def-136">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="56def-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="56def-137">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="56def-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="56def-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="56def-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="56def-139">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="56def-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="56def-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="56def-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="56def-141">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="56def-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="56def-142">-任意のクライアントから許可されていないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="56def-142">-  Any unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="56def-143">-有効なクライアント側の呼び出しへの応答でサーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="56def-143">-  Any server-side failure in response to a valid client-side call</span></span>  <br/>  <br/><span data-ttu-id="56def-144">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="56def-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="56def-145">子要素</span><span class="sxs-lookup"><span data-stu-id="56def-145">Child elements</span></span>

|<span data-ttu-id="56def-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="56def-146">**Element**</span></span>|<span data-ttu-id="56def-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="56def-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56def-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="56def-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="56def-149">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="56def-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="56def-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="56def-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="56def-151">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="56def-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="56def-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="56def-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="56def-153">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="56def-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="56def-154">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="56def-154">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="56def-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="56def-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="56def-156">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="56def-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="56def-157">同期状態</span><span class="sxs-lookup"><span data-stu-id="56def-157">SyncState</span></span>](syncstate-ex15websvcsotherref.md) <br/> |<span data-ttu-id="56def-158">各成功した要求の後に更新された同期データの base64 でエンコードされたフォームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="56def-158">Contains a base64-encoded form of the synchronization data that is updated after each successful request.</span></span> <span data-ttu-id="56def-159">これを使用して、同期の状態を識別します。</span><span class="sxs-lookup"><span data-stu-id="56def-159">This is used to identify the synchronization state.</span></span>  <br/> |
|[<span data-ttu-id="56def-160">IncludesLastItemInRange</span><span class="sxs-lookup"><span data-stu-id="56def-160">IncludesLastItemInRange</span></span>](includeslastiteminrange.md) <br/> |<span data-ttu-id="56def-161">最後の項目を同期するが、応答に含まれているかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="56def-161">Indicates whether the last item to synchronize has been included in the response.</span></span>  <br/> |
|[<span data-ttu-id="56def-162">変更 (アイテム)</span><span class="sxs-lookup"><span data-stu-id="56def-162">Changes (Items)</span></span>](changes-items.md) <br/> |<span data-ttu-id="56def-163">クライアント上のアイテムと、Exchange サーバー上のアイテム間の相違点の種類を表すの種類の変更の順序の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="56def-163">Contains a sequence array of change types that represent the types of differences between the items on the client and the items on the Exchange server.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="56def-164">親要素</span><span class="sxs-lookup"><span data-stu-id="56def-164">Parent elements</span></span>

|<span data-ttu-id="56def-165">**要素**</span><span class="sxs-lookup"><span data-stu-id="56def-165">**Element**</span></span>|<span data-ttu-id="56def-166">**説明**</span><span class="sxs-lookup"><span data-stu-id="56def-166">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="56def-167">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="56def-167">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="56def-168">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="56def-168">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="56def-169">備考</span><span class="sxs-lookup"><span data-stu-id="56def-169">Remarks</span></span>

<span data-ttu-id="56def-170">MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。</span><span class="sxs-lookup"><span data-stu-id="56def-170">The schema that describes this element is located in the EWS virtual directory of the computer that is running MicrosoftExchange Server 2007 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="56def-171">要素情報</span><span class="sxs-lookup"><span data-stu-id="56def-171">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="56def-172">名前空間</span><span class="sxs-lookup"><span data-stu-id="56def-172">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="56def-173">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="56def-173">Schema Name</span></span>  <br/> |<span data-ttu-id="56def-174">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="56def-174">Messages schema</span></span>  <br/> |
|<span data-ttu-id="56def-175">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="56def-175">Validation File</span></span>  <br/> |<span data-ttu-id="56def-176">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="56def-176">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="56def-177">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="56def-177">Can be Empty</span></span>  <br/> |<span data-ttu-id="56def-178">False</span><span class="sxs-lookup"><span data-stu-id="56def-178">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="56def-179">関連項目</span><span class="sxs-lookup"><span data-stu-id="56def-179">See also</span></span>

- [<span data-ttu-id="56def-180">SyncFolderItems の操作</span><span class="sxs-lookup"><span data-stu-id="56def-180">SyncFolderItems operation</span></span>](syncfolderitems-operation.md)
- [<span data-ttu-id="56def-181">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="56def-181">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

