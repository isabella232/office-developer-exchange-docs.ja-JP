---
title: UpdateItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateItemResponseMessage
api_type:
- schema
ms.assetid: dc585b05-5afc-4c74-8763-5a54f9a650ec
description: UpdateItemResponseMessage 要素には、1つの UpdateItem 操作要求の状態と結果が含まれています。
ms.openlocfilehash: ef25dcf26e06f199587cef885d8cbc9e93b52bdb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457943"
---
# <a name="updateitemresponsemessage"></a><span data-ttu-id="0de7d-103">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0de7d-103">UpdateItemResponseMessage</span></span>

<span data-ttu-id="0de7d-104">**UpdateItemResponseMessage**要素には、1つの[updateitem 操作](updateitem-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0de7d-104">The **UpdateItemResponseMessage** element contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="0de7d-105">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="0de7d-105">UpdateItemResponse</span></span>](updateitemresponse.md)
- [<span data-ttu-id="0de7d-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0de7d-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="0de7d-107">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0de7d-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
```xml
<UpdateItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
   <ConflictResults/>
</UpdateItemResponseMessage>
```

 <span data-ttu-id="0de7d-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0de7d-108">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0de7d-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0de7d-109">Attributes and elements</span></span>

<span data-ttu-id="0de7d-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0de7d-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0de7d-111">属性</span><span class="sxs-lookup"><span data-stu-id="0de7d-111">Attributes</span></span>

|<span data-ttu-id="0de7d-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="0de7d-112">**Attribute**</span></span>|<span data-ttu-id="0de7d-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="0de7d-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0de7d-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="0de7d-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="0de7d-115">[Updateitem 操作](updateitem-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="0de7d-115">Describes the status of an [UpdateItem operation](updateitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="0de7d-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="0de7d-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="0de7d-117">-成功</span><span class="sxs-lookup"><span data-stu-id="0de7d-117">-  Success</span></span>  <br/><span data-ttu-id="0de7d-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="0de7d-118">-  Warning</span></span>  <br/><span data-ttu-id="0de7d-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="0de7d-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="0de7d-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="0de7d-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="0de7d-121">**値**</span><span class="sxs-lookup"><span data-stu-id="0de7d-121">**Value**</span></span>|<span data-ttu-id="0de7d-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="0de7d-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0de7d-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="0de7d-123">**Success**</span></span> <br/> |<span data-ttu-id="0de7d-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="0de7d-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="0de7d-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="0de7d-125">**Warning**</span></span> <br/> | <span data-ttu-id="0de7d-126">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="0de7d-126">Describes a request that was not processed.</span></span> <span data-ttu-id="0de7d-127">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0de7d-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="0de7d-128">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0de7d-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="0de7d-129">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="0de7d-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="0de7d-130">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="0de7d-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="0de7d-131">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="0de7d-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="0de7d-132">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="0de7d-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="0de7d-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="0de7d-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="0de7d-134">-クォータが上限を超えています。</span><span class="sxs-lookup"><span data-stu-id="0de7d-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="0de7d-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="0de7d-135">**Error**</span></span> <br/> | <span data-ttu-id="0de7d-136">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="0de7d-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="0de7d-137">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0de7d-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="0de7d-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="0de7d-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="0de7d-139">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="0de7d-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="0de7d-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="0de7d-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="0de7d-141">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="0de7d-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="0de7d-142">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="0de7d-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="0de7d-143">-有効なクライアント側の呼び出しに応答した場合のサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="0de7d-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="0de7d-144">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0de7d-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0de7d-145">子要素</span><span class="sxs-lookup"><span data-stu-id="0de7d-145">Child elements</span></span>

|<span data-ttu-id="0de7d-146">**Element**</span><span class="sxs-lookup"><span data-stu-id="0de7d-146">**Element**</span></span>|<span data-ttu-id="0de7d-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="0de7d-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0de7d-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="0de7d-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0de7d-149">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="0de7d-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0de7d-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0de7d-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0de7d-151">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="0de7d-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="0de7d-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0de7d-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0de7d-153">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="0de7d-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="0de7d-154">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0de7d-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="0de7d-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0de7d-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0de7d-156">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="0de7d-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="0de7d-157">Items</span><span class="sxs-lookup"><span data-stu-id="0de7d-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="0de7d-158">更新されたアイテムの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="0de7d-158">Contains an array of updated items.</span></span>  <br/> |
|[<span data-ttu-id="0de7d-159">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="0de7d-159">ConflictResults</span></span>](conflictresults.md) <br/> |<span data-ttu-id="0de7d-160">[Updateitem 操作](updateitem-operation.md)応答の競合の数を格納します。</span><span class="sxs-lookup"><span data-stu-id="0de7d-160">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0de7d-161">親要素</span><span class="sxs-lookup"><span data-stu-id="0de7d-161">Parent elements</span></span>

|<span data-ttu-id="0de7d-162">**要素**</span><span class="sxs-lookup"><span data-stu-id="0de7d-162">**Element**</span></span>|<span data-ttu-id="0de7d-163">**説明**</span><span class="sxs-lookup"><span data-stu-id="0de7d-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0de7d-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0de7d-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0de7d-165">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="0de7d-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0de7d-166">注釈</span><span class="sxs-lookup"><span data-stu-id="0de7d-166">Remarks</span></span>

<span data-ttu-id="0de7d-167">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="0de7d-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0de7d-168">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0de7d-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0de7d-169">Namespace</span><span class="sxs-lookup"><span data-stu-id="0de7d-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0de7d-170">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0de7d-170">Schema Name</span></span>  <br/> |<span data-ttu-id="0de7d-171">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="0de7d-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0de7d-172">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0de7d-172">Validation File</span></span>  <br/> |<span data-ttu-id="0de7d-173">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0de7d-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0de7d-174">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0de7d-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="0de7d-175">正しくない</span><span class="sxs-lookup"><span data-stu-id="0de7d-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0de7d-176">関連項目</span><span class="sxs-lookup"><span data-stu-id="0de7d-176">See also</span></span>

- [<span data-ttu-id="0de7d-177">UpdateItem 操作</span><span class="sxs-lookup"><span data-stu-id="0de7d-177">UpdateItem operation</span></span>](updateitem-operation.md)
- [<span data-ttu-id="0de7d-178">連絡先の更新</span><span class="sxs-lookup"><span data-stu-id="0de7d-178">Updating Contacts</span></span>](https://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
- [<span data-ttu-id="0de7d-179">タスクの更新</span><span class="sxs-lookup"><span data-stu-id="0de7d-179">Updating Tasks</span></span>](https://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

