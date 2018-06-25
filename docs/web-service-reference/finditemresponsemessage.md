---
title: FindItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItemResponseMessage
api_type:
- schema
ms.assetid: fb2cd399-8a04-4f26-9091-993134ed1d15
description: FindItemResponseMessage 要素には、状態および 1 つの FindItem 操作要求の結果が含まれています。
ms.openlocfilehash: 0a4bfb3ba8d85b0bff0d03f043be865ce7276229
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760520"
---
# <a name="finditemresponsemessage"></a><span data-ttu-id="8efc7-103">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8efc7-103">FindItemResponseMessage</span></span>

<span data-ttu-id="8efc7-104">**FindItemResponseMessage**要素には、状態および 1 つの結果が含まれている[FindItem 操作](finditem-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="8efc7-104">The **FindItemResponseMessage** element contains the status and result of a single [FindItem operation](finditem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="8efc7-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="8efc7-105">FindItemResponse</span></span>](finditemresponse.md) 
- [<span data-ttu-id="8efc7-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8efc7-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="8efc7-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8efc7-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
```xml
<FindItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootFolder/>
</FindItemResponseMessage>
```

 <span data-ttu-id="8efc7-108">**FindItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="8efc7-108">**FindItemResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8efc7-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8efc7-109">Attributes and elements</span></span>

<span data-ttu-id="8efc7-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8efc7-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8efc7-111">属性</span><span class="sxs-lookup"><span data-stu-id="8efc7-111">Attributes</span></span>

|<span data-ttu-id="8efc7-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="8efc7-112">**Attribute**</span></span>|<span data-ttu-id="8efc7-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="8efc7-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8efc7-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="8efc7-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="8efc7-115">[FindItem 操作](finditem-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="8efc7-115">Describes the status of a [FindItem operation](finditem-operation.md) response.</span></span><br/><br/> <span data-ttu-id="8efc7-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="8efc7-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="8efc7-117">-成功</span><span class="sxs-lookup"><span data-stu-id="8efc7-117">-  Success</span></span>  <br/><span data-ttu-id="8efc7-118">-警告</span><span class="sxs-lookup"><span data-stu-id="8efc7-118">-  Warning</span></span>  <br/><span data-ttu-id="8efc7-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="8efc7-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="8efc7-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="8efc7-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="8efc7-121">**値**</span><span class="sxs-lookup"><span data-stu-id="8efc7-121">**Value**</span></span>|<span data-ttu-id="8efc7-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="8efc7-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8efc7-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="8efc7-123">**Success**</span></span> <br/> |<span data-ttu-id="8efc7-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="8efc7-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="8efc7-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="8efc7-125">**Warning**</span></span> <br/> | <span data-ttu-id="8efc7-126">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="8efc7-126">Describes a request that was not processed.</span></span> <span data-ttu-id="8efc7-127">警告は、処理された要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="8efc7-127">A warning may be returned if an error occurred while processing an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="8efc7-128">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8efc7-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="8efc7-129">-Exchange ストアは、バッチの中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="8efc7-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="8efc7-130">-Active Directory ドメイン サービス (AD DS) がオフラインになった。</span><span class="sxs-lookup"><span data-stu-id="8efc7-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="8efc7-131">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="8efc7-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="8efc7-132">-メッセージ データベース (MDB) がオフラインになった。</span><span class="sxs-lookup"><span data-stu-id="8efc7-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="8efc7-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="8efc7-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="8efc7-134">クォータを超過しました。</span><span class="sxs-lookup"><span data-stu-id="8efc7-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="8efc7-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="8efc7-135">**Error**</span></span> <br/> | <span data-ttu-id="8efc7-136">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="8efc7-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="8efc7-137">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="8efc7-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="8efc7-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="8efc7-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="8efc7-139">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="8efc7-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="8efc7-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="8efc7-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="8efc7-141">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="8efc7-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="8efc7-142">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="8efc7-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="8efc7-143">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="8efc7-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="8efc7-144">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="8efc7-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8efc7-145">子要素</span><span class="sxs-lookup"><span data-stu-id="8efc7-145">Child elements</span></span>

|<span data-ttu-id="8efc7-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="8efc7-146">**Element**</span></span>|<span data-ttu-id="8efc7-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="8efc7-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8efc7-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="8efc7-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="8efc7-149">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="8efc7-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="8efc7-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8efc7-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="8efc7-151">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="8efc7-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="8efc7-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8efc7-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="8efc7-153">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="8efc7-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="8efc7-154">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8efc7-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="8efc7-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="8efc7-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="8efc7-156">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="8efc7-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="8efc7-157">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="8efc7-157">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="8efc7-158">[FindItem 操作](finditem-operation.md)時に単一のルート フォルダーの検索の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8efc7-158">Contains the results from a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8efc7-159">親要素</span><span class="sxs-lookup"><span data-stu-id="8efc7-159">Parent elements</span></span>

|<span data-ttu-id="8efc7-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="8efc7-160">**Element**</span></span>|<span data-ttu-id="8efc7-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="8efc7-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8efc7-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8efc7-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="8efc7-163">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8efc7-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8efc7-164">備考</span><span class="sxs-lookup"><span data-stu-id="8efc7-164">Remarks</span></span>

<span data-ttu-id="8efc7-165">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="8efc7-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8efc7-166">要素情報</span><span class="sxs-lookup"><span data-stu-id="8efc7-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8efc7-167">名前空間</span><span class="sxs-lookup"><span data-stu-id="8efc7-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8efc7-168">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8efc7-168">Schema name</span></span>  <br/> |<span data-ttu-id="8efc7-169">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="8efc7-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8efc7-170">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8efc7-170">Validation file</span></span>  <br/> |<span data-ttu-id="8efc7-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8efc7-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8efc7-172">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8efc7-172">Can be empty</span></span>  <br/> |<span data-ttu-id="8efc7-173">False</span><span class="sxs-lookup"><span data-stu-id="8efc7-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8efc7-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="8efc7-174">See also</span></span>

- <span data-ttu-id="8efc7-175">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="8efc7-175">[FindItem operation](finditem-operation.md)</span></span>
- [<span data-ttu-id="8efc7-176">項目を検索します。</span><span class="sxs-lookup"><span data-stu-id="8efc7-176">Finding Items</span></span>](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

