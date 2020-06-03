---
title: ExportItemsResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExportItemsResponseMessage
api_type:
- schema
ms.assetid: 830fb008-3c45-4988-9041-91a3da3fe689
description: ExportItemsResponseMessage 要素には、1つのメールボックスアイテムをエクスポートする要求の状態と結果が含まれています。
ms.openlocfilehash: 3265836ce6d9d6ef97a4e598bbb3f50e7c5047c6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468947"
---
# <a name="exportitemsresponsemessage"></a><span data-ttu-id="bbc15-103">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bbc15-103">ExportItemsResponseMessage</span></span>

<span data-ttu-id="bbc15-104">**ExportItemsResponseMessage**要素には、1つのメールボックスアイテムをエクスポートする要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bbc15-104">The **ExportItemsResponseMessage** element contains the status and results of a request to export a single mailbox item.</span></span> 
  
- [<span data-ttu-id="bbc15-105">ExportItemsResponse</span><span class="sxs-lookup"><span data-stu-id="bbc15-105">ExportItemsResponse</span></span>](exportitemsresponse.md)  
- [<span data-ttu-id="bbc15-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bbc15-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="bbc15-107">ExportItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="bbc15-107">ExportItemsResponseMessage</span></span>](exportitemsresponsemessage.md)
  
```XML
<ExportItemsResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ItemId/>
   <Data/>
</ExportItemsResponseMessage>
```

<span data-ttu-id="bbc15-108">**ExportItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="bbc15-108">**ExportItemsResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="bbc15-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="bbc15-109">Attributes and elements</span></span>

<span data-ttu-id="bbc15-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="bbc15-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="bbc15-111">属性</span><span class="sxs-lookup"><span data-stu-id="bbc15-111">Attributes</span></span>

|<span data-ttu-id="bbc15-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="bbc15-112">**Attribute**</span></span>|<span data-ttu-id="bbc15-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="bbc15-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bbc15-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="bbc15-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="bbc15-115">応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="bbc15-115">Describes the status of the response.</span></span><br/><br/> <span data-ttu-id="bbc15-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="bbc15-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="bbc15-117">-成功</span><span class="sxs-lookup"><span data-stu-id="bbc15-117">-  Success</span></span>  <br/><span data-ttu-id="bbc15-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="bbc15-118">-  Warning</span></span>  <br/><span data-ttu-id="bbc15-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="bbc15-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="bbc15-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="bbc15-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="bbc15-121">**値**</span><span class="sxs-lookup"><span data-stu-id="bbc15-121">**Value**</span></span>|<span data-ttu-id="bbc15-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="bbc15-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="bbc15-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="bbc15-123">**Success**</span></span> <br/> |<span data-ttu-id="bbc15-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="bbc15-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="bbc15-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="bbc15-125">**Warning**</span></span> <br/> | <span data-ttu-id="bbc15-126">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="bbc15-126">Describes a request that was not processed.</span></span> <span data-ttu-id="bbc15-127">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="bbc15-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="bbc15-128">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bbc15-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="bbc15-129">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="bbc15-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="bbc15-130">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="bbc15-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="bbc15-131">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="bbc15-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="bbc15-132">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="bbc15-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="bbc15-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="bbc15-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="bbc15-134">-クォータが限界を超えています。</span><span class="sxs-lookup"><span data-stu-id="bbc15-134">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="bbc15-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="bbc15-135">**Error**</span></span> <br/> | <span data-ttu-id="bbc15-136">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="bbc15-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="bbc15-137">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="bbc15-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="bbc15-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="bbc15-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="bbc15-139">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="bbc15-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="bbc15-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="bbc15-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="bbc15-141">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="bbc15-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="bbc15-142">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="bbc15-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="bbc15-143">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="bbc15-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="bbc15-144">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bbc15-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="bbc15-145">子要素</span><span class="sxs-lookup"><span data-stu-id="bbc15-145">Child elements</span></span>

|<span data-ttu-id="bbc15-146">**Element**</span><span class="sxs-lookup"><span data-stu-id="bbc15-146">**Element**</span></span>|<span data-ttu-id="bbc15-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="bbc15-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bbc15-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="bbc15-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="bbc15-149">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="bbc15-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="bbc15-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="bbc15-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="bbc15-151">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="bbc15-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="bbc15-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="bbc15-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="bbc15-153">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="bbc15-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="bbc15-154">この要素には0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="bbc15-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="bbc15-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="bbc15-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="bbc15-156">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="bbc15-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="bbc15-157">ItemId</span><span class="sxs-lookup"><span data-stu-id="bbc15-157">ItemId</span></span>](itemid.md) <br/> |<span data-ttu-id="bbc15-158">エクスポートされたアイテムのアイテム識別子を含みます。</span><span class="sxs-lookup"><span data-stu-id="bbc15-158">Contains the item identifier of an exported item.</span></span>  <br/> |
|[<span data-ttu-id="bbc15-159">Data (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="bbc15-159">Data (base64Binary)</span></span>](data-base64binary.md) <br/> |<span data-ttu-id="bbc15-160">エクスポートされたアイテムの内容を含みます。</span><span class="sxs-lookup"><span data-stu-id="bbc15-160">Contains the contents of an exported item.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="bbc15-161">親要素</span><span class="sxs-lookup"><span data-stu-id="bbc15-161">Parent elements</span></span>

|<span data-ttu-id="bbc15-162">**要素**</span><span class="sxs-lookup"><span data-stu-id="bbc15-162">**Element**</span></span>|<span data-ttu-id="bbc15-163">**説明**</span><span class="sxs-lookup"><span data-stu-id="bbc15-163">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bbc15-164">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="bbc15-164">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="bbc15-165">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="bbc15-165">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="bbc15-166">テキスト値</span><span class="sxs-lookup"><span data-stu-id="bbc15-166">Text value</span></span>

<span data-ttu-id="bbc15-167">なし。</span><span class="sxs-lookup"><span data-stu-id="bbc15-167">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="bbc15-168">注釈</span><span class="sxs-lookup"><span data-stu-id="bbc15-168">Remarks</span></span>

<span data-ttu-id="bbc15-169">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bbc15-169">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="bbc15-170">要素の情報</span><span class="sxs-lookup"><span data-stu-id="bbc15-170">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="bbc15-171">Namespace</span><span class="sxs-lookup"><span data-stu-id="bbc15-171">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="bbc15-172">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="bbc15-172">Schema Name</span></span>  <br/> |<span data-ttu-id="bbc15-173">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="bbc15-173">Message schema</span></span>  <br/> |
|<span data-ttu-id="bbc15-174">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="bbc15-174">Validation File</span></span>  <br/> |<span data-ttu-id="bbc15-175">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="bbc15-175">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="bbc15-176">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="bbc15-176">Can be Empty</span></span>  <br/> |<span data-ttu-id="bbc15-177">正しくない</span><span class="sxs-lookup"><span data-stu-id="bbc15-177">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="bbc15-178">関連項目</span><span class="sxs-lookup"><span data-stu-id="bbc15-178">See also</span></span>

- [<span data-ttu-id="bbc15-179">ExportItems 操作</span><span class="sxs-lookup"><span data-stu-id="bbc15-179">ExportItems operation</span></span>](exportitems-operation.md) 
- [<span data-ttu-id="bbc15-180">UploadItems 操作</span><span class="sxs-lookup"><span data-stu-id="bbc15-180">UploadItems operation</span></span>](uploaditems-operation.md)

