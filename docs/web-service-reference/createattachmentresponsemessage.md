---
title: CreateAttachmentResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateAttachmentResponseMessage
api_type:
- schema
ms.assetid: b326e616-3ce0-4dcb-ba75-4ce4b9867211
description: CreateAttachmentResponseMessage 要素には、1つの CreateAttachment 操作要求の状態と結果が含まれています。
ms.openlocfilehash: 14d8d1936b3cfd52bdb816343c86606cb8ccf76f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458923"
---
# <a name="createattachmentresponsemessage"></a><span data-ttu-id="de7ff-103">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="de7ff-103">CreateAttachmentResponseMessage</span></span>

<span data-ttu-id="de7ff-104">**CreateAttachmentResponseMessage**要素には、1つの[createattachment 操作](createattachment-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de7ff-104">The **CreateAttachmentResponseMessage** element contains the status and result of a single [CreateAttachment operation](createattachment-operation.md) request.</span></span> 
  
- [<span data-ttu-id="de7ff-105">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="de7ff-105">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
- [<span data-ttu-id="de7ff-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="de7ff-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="de7ff-107">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="de7ff-107">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
  
```xml
<CreateAttachmentResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Attachments/>
</CreateAttachmentResponseMessage>
```

<span data-ttu-id="de7ff-108">**AttachmentInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="de7ff-108">**AttachmentInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="de7ff-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="de7ff-109">Attributes and elements</span></span>

<span data-ttu-id="de7ff-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="de7ff-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="de7ff-111">属性</span><span class="sxs-lookup"><span data-stu-id="de7ff-111">Attributes</span></span>

|<span data-ttu-id="de7ff-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="de7ff-112">**Attribute**</span></span>|<span data-ttu-id="de7ff-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="de7ff-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="de7ff-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="de7ff-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="de7ff-115">[Createattachment 操作](createattachment-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="de7ff-115">Describes the status of a [CreateAttachment operation](createattachment-operation.md) response.</span></span> <br/><br/><span data-ttu-id="de7ff-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="de7ff-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="de7ff-117">-成功</span><span class="sxs-lookup"><span data-stu-id="de7ff-117">-  Success</span></span>  <br/><span data-ttu-id="de7ff-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="de7ff-118">-  Warning</span></span>  <br/><span data-ttu-id="de7ff-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="de7ff-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="de7ff-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="de7ff-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="de7ff-121">**値**</span><span class="sxs-lookup"><span data-stu-id="de7ff-121">**Value**</span></span>|<span data-ttu-id="de7ff-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="de7ff-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="de7ff-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="de7ff-123">**Success**</span></span> <br/> |<span data-ttu-id="de7ff-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="de7ff-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="de7ff-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="de7ff-125">**Warning**</span></span> <br/> | <span data-ttu-id="de7ff-126">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="de7ff-126">Describes a request that was not processed.</span></span> <span data-ttu-id="de7ff-127">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="de7ff-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="de7ff-128">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="de7ff-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="de7ff-129">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="de7ff-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="de7ff-130">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="de7ff-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="de7ff-131">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="de7ff-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="de7ff-132">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="de7ff-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="de7ff-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="de7ff-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="de7ff-134">-クォータが上限を超えています。</span><span class="sxs-lookup"><span data-stu-id="de7ff-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="de7ff-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="de7ff-135">**Error**</span></span> <br/> | <span data-ttu-id="de7ff-136">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="de7ff-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="de7ff-137">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="de7ff-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="de7ff-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="de7ff-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="de7ff-139">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="de7ff-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="de7ff-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="de7ff-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="de7ff-141">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="de7ff-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="de7ff-142">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="de7ff-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="de7ff-143">-有効なクライアント側の呼び出しに応答した場合のサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="de7ff-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="de7ff-144">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="de7ff-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="de7ff-145">子要素</span><span class="sxs-lookup"><span data-stu-id="de7ff-145">Child elements</span></span>

|<span data-ttu-id="de7ff-146">**Element**</span><span class="sxs-lookup"><span data-stu-id="de7ff-146">**Element**</span></span>|<span data-ttu-id="de7ff-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="de7ff-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de7ff-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="de7ff-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="de7ff-149">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="de7ff-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="de7ff-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="de7ff-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="de7ff-151">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="de7ff-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="de7ff-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="de7ff-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="de7ff-153">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="de7ff-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="de7ff-154">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de7ff-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="de7ff-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="de7ff-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="de7ff-156">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="de7ff-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="de7ff-157">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="de7ff-157">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="de7ff-158">Exchange ストア内のアイテムに添付されているアイテムまたはファイルが保存されています。</span><span class="sxs-lookup"><span data-stu-id="de7ff-158">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="de7ff-159">親要素</span><span class="sxs-lookup"><span data-stu-id="de7ff-159">Parent elements</span></span>

|<span data-ttu-id="de7ff-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="de7ff-160">**Element**</span></span>|<span data-ttu-id="de7ff-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="de7ff-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="de7ff-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="de7ff-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="de7ff-163">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="de7ff-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="de7ff-164">注釈</span><span class="sxs-lookup"><span data-stu-id="de7ff-164">Remarks</span></span>

<span data-ttu-id="de7ff-165">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="de7ff-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="de7ff-166">1回のラウンドトリップで複数の添付ファイルがアイテムに添付されている場合、最後の応答メッセージの**RootItemChangeKey**属性は、添付ファイルがあるアイテムの新しい変更キーを表す属性です。</span><span class="sxs-lookup"><span data-stu-id="de7ff-166">If multiple attachments are attached to an item in a single round trip, the **RootItemChangeKey** attribute in the last response message is the one that represents the new change key of the item that has the attachments.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="de7ff-167">要素の情報</span><span class="sxs-lookup"><span data-stu-id="de7ff-167">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="de7ff-168">Namespace</span><span class="sxs-lookup"><span data-stu-id="de7ff-168">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="de7ff-169">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="de7ff-169">Schema Name</span></span>  <br/> |<span data-ttu-id="de7ff-170">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="de7ff-170">Messages schema</span></span>  <br/> |
|<span data-ttu-id="de7ff-171">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="de7ff-171">Validation File</span></span>  <br/> |<span data-ttu-id="de7ff-172">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="de7ff-172">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="de7ff-173">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="de7ff-173">Can be Empty</span></span>  <br/> |<span data-ttu-id="de7ff-174">正しくない</span><span class="sxs-lookup"><span data-stu-id="de7ff-174">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="de7ff-175">関連項目</span><span class="sxs-lookup"><span data-stu-id="de7ff-175">See also</span></span>

- [<span data-ttu-id="de7ff-176">CreateAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="de7ff-176">CreateAttachment operation</span></span>](createattachment-operation.md) 
- [<span data-ttu-id="de7ff-177">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="de7ff-177">CreateAttachment</span></span>](createattachment.md)
- <span data-ttu-id="de7ff-178">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="de7ff-178">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span> 
- [<span data-ttu-id="de7ff-179">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="de7ff-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

