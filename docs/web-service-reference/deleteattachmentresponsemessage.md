---
title: DeleteAttachmentResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteAttachmentResponseMessage
api_type:
- schema
ms.assetid: 1edb085f-1674-48e5-8ec3-42351adeac7d
description: DeleteAttachmentResponseMessage 要素には、1つの DeleteAttachment 操作要求の状態と結果が含まれています。
ms.openlocfilehash: 3ff253a5c2b6cbd69b7b976f7f41ca8b83814a74
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464260"
---
# <a name="deleteattachmentresponsemessage"></a><span data-ttu-id="2fbcc-103">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2fbcc-103">DeleteAttachmentResponseMessage</span></span>

<span data-ttu-id="2fbcc-104">**DeleteAttachmentResponseMessage**要素には、1つの[deleteattachment 操作](deleteattachment-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-104">The **DeleteAttachmentResponseMessage** element contains the status and result of a single [DeleteAttachment operation](deleteattachment-operation.md) request.</span></span> 
  
- [<span data-ttu-id="2fbcc-105">DeleteAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="2fbcc-105">DeleteAttachmentResponse</span></span>](deleteattachmentresponse.md)  
- [<span data-ttu-id="2fbcc-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2fbcc-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="2fbcc-107">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="2fbcc-107">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md)
  
```xml
<DeleteAttachmentResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootItemId/>
</DeleteAttachmentResponseMessage>
```

<span data-ttu-id="2fbcc-108">**DeleteAttachmentResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="2fbcc-108">**DeleteAttachmentResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="2fbcc-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="2fbcc-109">Attributes and elements</span></span>

<span data-ttu-id="2fbcc-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="2fbcc-111">属性</span><span class="sxs-lookup"><span data-stu-id="2fbcc-111">Attributes</span></span>

|<span data-ttu-id="2fbcc-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="2fbcc-112">**Attribute**</span></span>|<span data-ttu-id="2fbcc-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="2fbcc-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2fbcc-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="2fbcc-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="2fbcc-115">[Deleteattachment 操作](deleteattachment-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-115">Describes the status of a [DeleteAttachment operation](deleteattachment-operation.md) response.</span></span><br/><br/><span data-ttu-id="2fbcc-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="2fbcc-117">-成功</span><span class="sxs-lookup"><span data-stu-id="2fbcc-117">-  Success</span></span>  <br/><span data-ttu-id="2fbcc-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="2fbcc-118">-  Warning</span></span>  <br/><span data-ttu-id="2fbcc-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="2fbcc-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="2fbcc-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="2fbcc-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="2fbcc-121">**値**</span><span class="sxs-lookup"><span data-stu-id="2fbcc-121">**Value**</span></span>|<span data-ttu-id="2fbcc-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="2fbcc-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="2fbcc-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="2fbcc-123">**Success**</span></span> <br/> |<span data-ttu-id="2fbcc-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="2fbcc-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="2fbcc-125">**Warning**</span></span> <br/> | <span data-ttu-id="2fbcc-126">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-126">Describes a request that was not processed.</span></span> <span data-ttu-id="2fbcc-127">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="2fbcc-128">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="2fbcc-129">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-129">- The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="2fbcc-130">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="2fbcc-131">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="2fbcc-132">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="2fbcc-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="2fbcc-134">-クォータが上限を超えています。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="2fbcc-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="2fbcc-135">**Error**</span></span> <br/> | <span data-ttu-id="2fbcc-136">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="2fbcc-137">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="2fbcc-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="2fbcc-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="2fbcc-139">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="2fbcc-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="2fbcc-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="2fbcc-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="2fbcc-141">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="2fbcc-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="2fbcc-142">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="2fbcc-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="2fbcc-143">-有効なクライアント側の呼び出しに応答した場合のサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="2fbcc-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="2fbcc-144">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="2fbcc-145">子要素</span><span class="sxs-lookup"><span data-stu-id="2fbcc-145">Child elements</span></span>

|<span data-ttu-id="2fbcc-146">**Element**</span><span class="sxs-lookup"><span data-stu-id="2fbcc-146">**Element**</span></span>|<span data-ttu-id="2fbcc-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="2fbcc-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2fbcc-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="2fbcc-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="2fbcc-149">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="2fbcc-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2fbcc-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="2fbcc-151">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="2fbcc-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="2fbcc-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="2fbcc-153">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="2fbcc-154">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="2fbcc-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="2fbcc-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="2fbcc-156">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="2fbcc-157">RootItemId</span><span class="sxs-lookup"><span data-stu-id="2fbcc-157">RootItemId</span></span>](rootitemid.md) <br/> |<span data-ttu-id="2fbcc-158">削除された添付ファイルの親アイテムを識別します。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-158">Identifies the parent item of a deleted attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="2fbcc-159">親要素</span><span class="sxs-lookup"><span data-stu-id="2fbcc-159">Parent elements</span></span>

|<span data-ttu-id="2fbcc-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="2fbcc-160">**Element**</span></span>|<span data-ttu-id="2fbcc-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="2fbcc-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="2fbcc-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="2fbcc-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="2fbcc-163">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="2fbcc-164">注釈</span><span class="sxs-lookup"><span data-stu-id="2fbcc-164">Remarks</span></span>

<span data-ttu-id="2fbcc-165">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされた Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="2fbcc-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="2fbcc-166">要素の情報</span><span class="sxs-lookup"><span data-stu-id="2fbcc-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="2fbcc-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="2fbcc-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="2fbcc-168">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="2fbcc-168">Schema Name</span></span>  <br/> |<span data-ttu-id="2fbcc-169">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="2fbcc-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="2fbcc-170">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="2fbcc-170">Validation File</span></span>  <br/> |<span data-ttu-id="2fbcc-171">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="2fbcc-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="2fbcc-172">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="2fbcc-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="2fbcc-173">正しくない</span><span class="sxs-lookup"><span data-stu-id="2fbcc-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="2fbcc-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="2fbcc-174">See also</span></span>

- [<span data-ttu-id="2fbcc-175">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="2fbcc-175">DeleteAttachment</span></span>](deleteattachment.md) 
- [<span data-ttu-id="2fbcc-176">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="2fbcc-176">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- [<span data-ttu-id="2fbcc-177">Exchange 用 EWS リファレンス</span><span class="sxs-lookup"><span data-stu-id="2fbcc-177">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="2fbcc-178">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="2fbcc-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

