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
description: UploadItemsResponseMessage 要素には、1つのメールボックスアイテムをアップロードする要求の状態と結果が含まれています。
ms.openlocfilehash: 4049772c560f3d54a31351fe1fbed77fe5780bf8
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468496"
---
# <a name="uploaditemsresponsemessage"></a><span data-ttu-id="59dbe-103">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="59dbe-103">UploadItemsResponseMessage</span></span>

<span data-ttu-id="59dbe-104">**UploadItemsResponseMessage**要素には、1つのメールボックスアイテムをアップロードする要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="59dbe-104">The **UploadItemsResponseMessage** element contains the status and results of a request to upload a single mailbox item.</span></span> 
  
- [<span data-ttu-id="59dbe-105">UploadItemsResponse</span><span class="sxs-lookup"><span data-stu-id="59dbe-105">UploadItemsResponse</span></span>](uploaditemsresponse.md) 
- [<span data-ttu-id="59dbe-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="59dbe-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="59dbe-107">UploadItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="59dbe-107">UploadItemsResponseMessage</span></span>](uploaditemsresponsemessage.md)
  
```XML
<UploadItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ItemId/>
</UploadItemsResponseMessage>
```

 <span data-ttu-id="59dbe-108">**UploadItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="59dbe-108">**UploadItemsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59dbe-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="59dbe-109">Attributes and elements</span></span>

<span data-ttu-id="59dbe-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="59dbe-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59dbe-111">属性</span><span class="sxs-lookup"><span data-stu-id="59dbe-111">Attributes</span></span>

|<span data-ttu-id="59dbe-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="59dbe-112">**Attribute**</span></span>|<span data-ttu-id="59dbe-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="59dbe-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="59dbe-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="59dbe-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="59dbe-115">応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="59dbe-115">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="59dbe-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="59dbe-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="59dbe-117">-成功</span><span class="sxs-lookup"><span data-stu-id="59dbe-117">-  Success</span></span>  <br/><span data-ttu-id="59dbe-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="59dbe-118">-  Warning</span></span>  <br/><span data-ttu-id="59dbe-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="59dbe-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="59dbe-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="59dbe-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="59dbe-121">**値**</span><span class="sxs-lookup"><span data-stu-id="59dbe-121">**Value**</span></span>|<span data-ttu-id="59dbe-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="59dbe-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="59dbe-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="59dbe-123">**Success**</span></span> <br/> |<span data-ttu-id="59dbe-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="59dbe-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="59dbe-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="59dbe-125">**Warning**</span></span> <br/> | <span data-ttu-id="59dbe-126">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="59dbe-126">Describes a request that was not processed.</span></span> <span data-ttu-id="59dbe-127">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="59dbe-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="59dbe-128">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="59dbe-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="59dbe-129">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="59dbe-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="59dbe-130">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="59dbe-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="59dbe-131">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="59dbe-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="59dbe-132">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="59dbe-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="59dbe-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="59dbe-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="59dbe-134">-クォータが限界を超えています。</span><span class="sxs-lookup"><span data-stu-id="59dbe-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="59dbe-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="59dbe-135">**Error**</span></span> <br/> | <span data-ttu-id="59dbe-136">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="59dbe-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="59dbe-137">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="59dbe-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="59dbe-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="59dbe-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="59dbe-139">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="59dbe-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="59dbe-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="59dbe-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="59dbe-141">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="59dbe-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="59dbe-142">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="59dbe-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="59dbe-143">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="59dbe-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="59dbe-144">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="59dbe-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="59dbe-145">子要素</span><span class="sxs-lookup"><span data-stu-id="59dbe-145">Child elements</span></span>

|<span data-ttu-id="59dbe-146">**Element**</span><span class="sxs-lookup"><span data-stu-id="59dbe-146">**Element**</span></span>|<span data-ttu-id="59dbe-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="59dbe-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59dbe-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="59dbe-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="59dbe-149">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="59dbe-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="59dbe-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="59dbe-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="59dbe-151">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="59dbe-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="59dbe-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="59dbe-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="59dbe-153">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="59dbe-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="59dbe-154">この要素には0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="59dbe-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="59dbe-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="59dbe-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="59dbe-156">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="59dbe-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="59dbe-157">ItemId</span><span class="sxs-lookup"><span data-stu-id="59dbe-157">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="59dbe-158">アップロードされたアイテムのアイテム識別子を含みます。</span><span class="sxs-lookup"><span data-stu-id="59dbe-158">Contains the item identifier of an uploaded item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="59dbe-159">親要素</span><span class="sxs-lookup"><span data-stu-id="59dbe-159">Parent elements</span></span>

|<span data-ttu-id="59dbe-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="59dbe-160">**Element**</span></span>|<span data-ttu-id="59dbe-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="59dbe-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59dbe-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="59dbe-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="59dbe-163">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="59dbe-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="59dbe-164">テキスト値</span><span class="sxs-lookup"><span data-stu-id="59dbe-164">Text value</span></span>

<span data-ttu-id="59dbe-165">なし。</span><span class="sxs-lookup"><span data-stu-id="59dbe-165">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="59dbe-166">注釈</span><span class="sxs-lookup"><span data-stu-id="59dbe-166">Remarks</span></span>

<span data-ttu-id="59dbe-167">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="59dbe-167">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59dbe-168">要素の情報</span><span class="sxs-lookup"><span data-stu-id="59dbe-168">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59dbe-169">Namespace</span><span class="sxs-lookup"><span data-stu-id="59dbe-169">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="59dbe-170">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="59dbe-170">Schema Name</span></span>  <br/> |<span data-ttu-id="59dbe-171">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="59dbe-171">Message schema</span></span>  <br/> |
|<span data-ttu-id="59dbe-172">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="59dbe-172">Validation File</span></span>  <br/> |<span data-ttu-id="59dbe-173">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="59dbe-173">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="59dbe-174">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="59dbe-174">Can be Empty</span></span>  <br/> |<span data-ttu-id="59dbe-175">正しくない</span><span class="sxs-lookup"><span data-stu-id="59dbe-175">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59dbe-176">関連項目</span><span class="sxs-lookup"><span data-stu-id="59dbe-176">See also</span></span>

- [<span data-ttu-id="59dbe-177">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="59dbe-177">ExportItems operation</span></span>](exportitems-operation.md)
- [<span data-ttu-id="59dbe-178">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="59dbe-178">UploadItems operation</span></span>](uploaditems-operation.md)
- [<span data-ttu-id="59dbe-179">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="59dbe-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

