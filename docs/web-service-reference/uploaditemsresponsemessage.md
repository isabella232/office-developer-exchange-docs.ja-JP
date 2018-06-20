---
title: UploadItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UploadItemsResponseMessage
api_type:
- schema
ms.assetid: 03febd08-c015-4009-b291-1b4296182ffe
description: UploadItemsResponseMessage 要素には、ステータスと 1 つのメールボックス アイテムをアップロードするための要求の結果が含まれています。
ms.openlocfilehash: 9a1a33011aa1e240ab7e15794e2e89401238ffda
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839910"
---
# <a name="uploaditemsresponsemessage"></a><span data-ttu-id="8f470-103">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8f470-103">UploadItemsResponseMessage</span></span>

<span data-ttu-id="8f470-104">**UploadItemsResponseMessage**要素には、ステータスと 1 つのメールボックス アイテムをアップロードするための要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8f470-104">The **UploadItemsResponseMessage** element contains the status and results of a request to upload a single mailbox item.</span></span> 
  
- [<span data-ttu-id="8f470-105">UploadItemsResponse</span><span class="sxs-lookup"><span data-stu-id="8f470-105">UploadItemsResponse</span></span>](uploaditemsresponse.md) 
- [<span data-ttu-id="8f470-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8f470-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="8f470-107">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8f470-107">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md)
  
```XML
<UploadItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ItemId/>
</UploadItemsResponseMessage>
```

 <span data-ttu-id="8f470-108">**UploadItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="8f470-108">**UploadItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8f470-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8f470-109">Attributes and elements</span></span>

<span data-ttu-id="8f470-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8f470-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8f470-111">属性</span><span class="sxs-lookup"><span data-stu-id="8f470-111">Attributes</span></span>

|<span data-ttu-id="8f470-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="8f470-112">**Attribute**</span></span>|<span data-ttu-id="8f470-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="8f470-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8f470-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="8f470-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="8f470-115">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="8f470-115">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="8f470-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="8f470-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="8f470-117">-成功</span><span class="sxs-lookup"><span data-stu-id="8f470-117">-  Success</span></span>  <br/><span data-ttu-id="8f470-118">-警告</span><span class="sxs-lookup"><span data-stu-id="8f470-118">-  Warning</span></span>  <br/><span data-ttu-id="8f470-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="8f470-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="8f470-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="8f470-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="8f470-121">**値**</span><span class="sxs-lookup"><span data-stu-id="8f470-121">**Value**</span></span>|<span data-ttu-id="8f470-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="8f470-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8f470-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="8f470-123">**Success**</span></span> <br/> |<span data-ttu-id="8f470-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="8f470-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="8f470-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="8f470-125">**Warning**</span></span> <br/> | <span data-ttu-id="8f470-126">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="8f470-126">Describes a request that was not processed.</span></span> <span data-ttu-id="8f470-127">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="8f470-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="8f470-128">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8f470-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="8f470-129">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="8f470-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="8f470-130">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="8f470-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="8f470-131">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="8f470-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="8f470-132">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="8f470-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="8f470-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="8f470-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="8f470-134">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="8f470-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="8f470-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="8f470-135">**Error**</span></span> <br/> | <span data-ttu-id="8f470-136">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="8f470-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="8f470-137">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="8f470-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="8f470-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="8f470-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="8f470-139">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="8f470-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="8f470-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="8f470-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="8f470-141">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="8f470-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="8f470-142">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="8f470-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="8f470-143">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="8f470-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="8f470-144">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="8f470-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8f470-145">子要素</span><span class="sxs-lookup"><span data-stu-id="8f470-145">Child elements</span></span>

|<span data-ttu-id="8f470-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="8f470-146">**Element**</span></span>|<span data-ttu-id="8f470-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="8f470-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f470-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="8f470-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="8f470-149">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="8f470-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="8f470-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8f470-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="8f470-151">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="8f470-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="8f470-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8f470-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="8f470-153">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="8f470-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="8f470-154">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8f470-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="8f470-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="8f470-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="8f470-156">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="8f470-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="8f470-157">ItemId</span><span class="sxs-lookup"><span data-stu-id="8f470-157">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="8f470-158">アップロードされた項目の項目の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8f470-158">Contains the item identifier of an uploaded item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8f470-159">親要素</span><span class="sxs-lookup"><span data-stu-id="8f470-159">Parent elements</span></span>

|<span data-ttu-id="8f470-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="8f470-160">**Element**</span></span>|<span data-ttu-id="8f470-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="8f470-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8f470-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8f470-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="8f470-163">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8f470-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="8f470-164">テキスト値</span><span class="sxs-lookup"><span data-stu-id="8f470-164">Text value</span></span>

<span data-ttu-id="8f470-165">なし。</span><span class="sxs-lookup"><span data-stu-id="8f470-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8f470-166">備考</span><span class="sxs-lookup"><span data-stu-id="8f470-166">Remarks</span></span>

<span data-ttu-id="8f470-167">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="8f470-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8f470-168">要素情報</span><span class="sxs-lookup"><span data-stu-id="8f470-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8f470-169">名前空間</span><span class="sxs-lookup"><span data-stu-id="8f470-169">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8f470-170">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8f470-170">Schema Name</span></span>  <br/> |<span data-ttu-id="8f470-171">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="8f470-171">Message schema</span></span>  <br/> |
|<span data-ttu-id="8f470-172">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8f470-172">Validation File</span></span>  <br/> |<span data-ttu-id="8f470-173">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8f470-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8f470-174">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8f470-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="8f470-175">False</span><span class="sxs-lookup"><span data-stu-id="8f470-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8f470-176">関連項目</span><span class="sxs-lookup"><span data-stu-id="8f470-176">See also</span></span>

- [<span data-ttu-id="8f470-177">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="8f470-177">ExportItems operation</span></span>](exportitems-operation.md)
- [<span data-ttu-id="8f470-178">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="8f470-178">UploadItems operation</span></span>](uploaditems-operation.md)
- [<span data-ttu-id="8f470-179">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8f470-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

