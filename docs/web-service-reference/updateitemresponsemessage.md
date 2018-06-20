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
description: UpdateItemResponseMessage 要素には、状態および 1 つの UpdateItem 操作要求の結果が含まれています。
ms.openlocfilehash: c971657813784e68a01539899e8fabea67847325
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839874"
---
# <a name="updateitemresponsemessage"></a><span data-ttu-id="eb556-103">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="eb556-103">UpdateItemResponseMessage</span></span>

<span data-ttu-id="eb556-104">**UpdateItemResponseMessage**要素には、状態および 1 つの結果が含まれている[UpdateItem 操作](updateitem-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="eb556-104">The **UpdateItemResponseMessage** element contains the status and result of a single [UpdateItem operation](updateitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="eb556-105">UpdateItemResponse</span><span class="sxs-lookup"><span data-stu-id="eb556-105">UpdateItemResponse</span></span>](updateitemresponse.md)
- [<span data-ttu-id="eb556-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="eb556-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="eb556-107">UpdateItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="eb556-107">UpdateItemResponseMessage</span></span>](updateitemresponsemessage.md)
  
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

 <span data-ttu-id="eb556-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="eb556-108">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eb556-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="eb556-109">Attributes and elements</span></span>

<span data-ttu-id="eb556-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="eb556-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eb556-111">属性</span><span class="sxs-lookup"><span data-stu-id="eb556-111">Attributes</span></span>

|<span data-ttu-id="eb556-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="eb556-112">**Attribute**</span></span>|<span data-ttu-id="eb556-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="eb556-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="eb556-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="eb556-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="eb556-115">[UpdateItem 操作](updateitem-operation.md)応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="eb556-115">Describes the status of an [UpdateItem operation](updateitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="eb556-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="eb556-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="eb556-117">-成功</span><span class="sxs-lookup"><span data-stu-id="eb556-117">-  Success</span></span>  <br/><span data-ttu-id="eb556-118">-警告</span><span class="sxs-lookup"><span data-stu-id="eb556-118">-  Warning</span></span>  <br/><span data-ttu-id="eb556-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="eb556-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="eb556-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="eb556-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="eb556-121">**値**</span><span class="sxs-lookup"><span data-stu-id="eb556-121">**Value**</span></span>|<span data-ttu-id="eb556-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="eb556-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="eb556-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="eb556-123">**Success**</span></span> <br/> |<span data-ttu-id="eb556-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="eb556-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="eb556-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="eb556-125">**Warning**</span></span> <br/> | <span data-ttu-id="eb556-126">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="eb556-126">Describes a request that was not processed.</span></span> <span data-ttu-id="eb556-127">警告は、要求内のアイテムの処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="eb556-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="eb556-128">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eb556-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="eb556-129">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="eb556-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="eb556-130">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="eb556-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="eb556-131">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="eb556-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="eb556-132">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="eb556-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="eb556-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="eb556-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="eb556-134">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="eb556-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="eb556-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="eb556-135">**Error**</span></span> <br/> | <span data-ttu-id="eb556-136">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="eb556-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="eb556-137">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="eb556-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="eb556-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="eb556-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="eb556-139">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="eb556-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="eb556-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="eb556-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="eb556-141">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="eb556-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="eb556-142">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="eb556-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="eb556-143">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="eb556-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="eb556-144">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="eb556-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="eb556-145">子要素</span><span class="sxs-lookup"><span data-stu-id="eb556-145">Child elements</span></span>

|<span data-ttu-id="eb556-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="eb556-146">**Element**</span></span>|<span data-ttu-id="eb556-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="eb556-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb556-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="eb556-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="eb556-149">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="eb556-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="eb556-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="eb556-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="eb556-151">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="eb556-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="eb556-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="eb556-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="eb556-153">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="eb556-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="eb556-154">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="eb556-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="eb556-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="eb556-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="eb556-156">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="eb556-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="eb556-157">Items</span><span class="sxs-lookup"><span data-stu-id="eb556-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="eb556-158">更新された項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="eb556-158">Contains an array of updated items.</span></span>  <br/> |
|[<span data-ttu-id="eb556-159">ConflictResults</span><span class="sxs-lookup"><span data-stu-id="eb556-159">ConflictResults</span></span>](conflictresults.md) <br/> |<span data-ttu-id="eb556-160">[UpdateItem 操作](updateitem-operation.md)の応答の競合の数が含まれています。</span><span class="sxs-lookup"><span data-stu-id="eb556-160">Contains the number of conflicts in an [UpdateItem operation](updateitem-operation.md) response.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eb556-161">親要素</span><span class="sxs-lookup"><span data-stu-id="eb556-161">Parent elements</span></span>

|<span data-ttu-id="eb556-162">**要素**</span><span class="sxs-lookup"><span data-stu-id="eb556-162">**Element**</span></span>|<span data-ttu-id="eb556-163">**説明**</span><span class="sxs-lookup"><span data-stu-id="eb556-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb556-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="eb556-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="eb556-165">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="eb556-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="eb556-166">備考</span><span class="sxs-lookup"><span data-stu-id="eb556-166">Remarks</span></span>

<span data-ttu-id="eb556-167">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="eb556-167">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eb556-168">要素情報</span><span class="sxs-lookup"><span data-stu-id="eb556-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb556-169">名前空間</span><span class="sxs-lookup"><span data-stu-id="eb556-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="eb556-170">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="eb556-170">Schema Name</span></span>  <br/> |<span data-ttu-id="eb556-171">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="eb556-171">Messages schema</span></span>  <br/> |
|<span data-ttu-id="eb556-172">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="eb556-172">Validation File</span></span>  <br/> |<span data-ttu-id="eb556-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="eb556-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="eb556-174">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="eb556-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="eb556-175">False</span><span class="sxs-lookup"><span data-stu-id="eb556-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eb556-176">関連項目</span><span class="sxs-lookup"><span data-stu-id="eb556-176">See also</span></span>

- <span data-ttu-id="eb556-177">
  [UpdateItem 操作](updateitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="eb556-177">[UpdateItem operation](updateitem-operation.md)</span></span>
- [<span data-ttu-id="eb556-178">連絡先を更新</span><span class="sxs-lookup"><span data-stu-id="eb556-178">Updating Contacts</span></span>](http://msdn.microsoft.com/library/9a865953-b94a-4229-b632-2dee433314be%28Office.15%29.aspx)
- [<span data-ttu-id="eb556-179">タスクの更新</span><span class="sxs-lookup"><span data-stu-id="eb556-179">Updating Tasks</span></span>](http://msdn.microsoft.com/library/0a1bf360-d40c-4a99-929b-4c73a14394d5%28Office.15%29.aspx)

