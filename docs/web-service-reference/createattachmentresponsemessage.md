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
description: CreateAttachmentResponseMessage 要素には、状態および 1 つの CreateAttachment 操作要求の結果が含まれています。
ms.openlocfilehash: a6d3adde07dedb7a2533d6e9c7fc6ff0497792bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759808"
---
# <a name="createattachmentresponsemessage"></a><span data-ttu-id="cc7b3-103">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cc7b3-103">CreateAttachmentResponseMessage</span></span>

<span data-ttu-id="cc7b3-104">**CreateAttachmentResponseMessage**要素には、状態および 1 つの結果が含まれています[CreateAttachment 操作](createattachment-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-104">The **CreateAttachmentResponseMessage** element contains the status and result of a single [CreateAttachment operation](createattachment-operation.md) request.</span></span> 
  
- [<span data-ttu-id="cc7b3-105">CreateAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="cc7b3-105">CreateAttachmentResponse</span></span>](createattachmentresponse.md)
- [<span data-ttu-id="cc7b3-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cc7b3-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="cc7b3-107">CreateAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cc7b3-107">CreateAttachmentResponseMessage</span></span>](createattachmentresponsemessage.md)
  
```xml
<CreateAttachmentResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Attachments/>
</CreateAttachmentResponseMessage>
```

<span data-ttu-id="cc7b3-108">**AttachmentInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="cc7b3-108">**AttachmentInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="cc7b3-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="cc7b3-109">Attributes and elements</span></span>

<span data-ttu-id="cc7b3-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cc7b3-111">属性</span><span class="sxs-lookup"><span data-stu-id="cc7b3-111">Attributes</span></span>

|<span data-ttu-id="cc7b3-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="cc7b3-112">**Attribute**</span></span>|<span data-ttu-id="cc7b3-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="cc7b3-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cc7b3-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="cc7b3-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="cc7b3-115">[CreateAttachment 操作](createattachment-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-115">Describes the status of a [CreateAttachment operation](createattachment-operation.md) response.</span></span> <br/><br/><span data-ttu-id="cc7b3-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="cc7b3-117">-成功</span><span class="sxs-lookup"><span data-stu-id="cc7b3-117">-  Success</span></span>  <br/><span data-ttu-id="cc7b3-118">-警告</span><span class="sxs-lookup"><span data-stu-id="cc7b3-118">-  Warning</span></span>  <br/><span data-ttu-id="cc7b3-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="cc7b3-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="cc7b3-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="cc7b3-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="cc7b3-121">**値**</span><span class="sxs-lookup"><span data-stu-id="cc7b3-121">**Value**</span></span>|<span data-ttu-id="cc7b3-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="cc7b3-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cc7b3-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="cc7b3-123">**Success**</span></span> <br/> |<span data-ttu-id="cc7b3-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="cc7b3-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="cc7b3-125">**Warning**</span></span> <br/> | <span data-ttu-id="cc7b3-126">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-126">Describes a request that was not processed.</span></span> <span data-ttu-id="cc7b3-127">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="cc7b3-128">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="cc7b3-129">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="cc7b3-130">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="cc7b3-131">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="cc7b3-132">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="cc7b3-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="cc7b3-134">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="cc7b3-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="cc7b3-135">**Error**</span></span> <br/> | <span data-ttu-id="cc7b3-136">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="cc7b3-137">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="cc7b3-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="cc7b3-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="cc7b3-139">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="cc7b3-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="cc7b3-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="cc7b3-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="cc7b3-141">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="cc7b3-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="cc7b3-142">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="cc7b3-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="cc7b3-143">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="cc7b3-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="cc7b3-144">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="cc7b3-145">子要素</span><span class="sxs-lookup"><span data-stu-id="cc7b3-145">Child elements</span></span>

|<span data-ttu-id="cc7b3-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="cc7b3-146">**Element**</span></span>|<span data-ttu-id="cc7b3-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="cc7b3-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc7b3-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="cc7b3-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="cc7b3-149">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="cc7b3-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cc7b3-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="cc7b3-151">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="cc7b3-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="cc7b3-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="cc7b3-153">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="cc7b3-154">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="cc7b3-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="cc7b3-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="cc7b3-156">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="cc7b3-157">添付ファイル</span><span class="sxs-lookup"><span data-stu-id="cc7b3-157">Attachments</span></span>](attachments-ex15websvcsotherref.md) <br/> |<span data-ttu-id="cc7b3-158">アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-158">Contains the items or files that are attached to an item in the Exchange store.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cc7b3-159">親要素</span><span class="sxs-lookup"><span data-stu-id="cc7b3-159">Parent elements</span></span>

|<span data-ttu-id="cc7b3-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="cc7b3-160">**Element**</span></span>|<span data-ttu-id="cc7b3-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="cc7b3-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cc7b3-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cc7b3-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="cc7b3-163">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cc7b3-164">備考</span><span class="sxs-lookup"><span data-stu-id="cc7b3-164">Remarks</span></span>

<span data-ttu-id="cc7b3-165">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
> [!NOTE]
> <span data-ttu-id="cc7b3-166">複数の添付ファイルはラウンド トリップで 1 つのアイテムに関連付けられている、最後の応答メッセージ内の**RootItemChangeKey**属性が添付ファイルのあるアイテムの新しい変更キーを表す 1 つ。</span><span class="sxs-lookup"><span data-stu-id="cc7b3-166">If multiple attachments are attached to an item in a single round trip, the **RootItemChangeKey** attribute in the last response message is the one that represents the new change key of the item that has the attachments.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="cc7b3-167">要素情報</span><span class="sxs-lookup"><span data-stu-id="cc7b3-167">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cc7b3-168">名前空間</span><span class="sxs-lookup"><span data-stu-id="cc7b3-168">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cc7b3-169">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cc7b3-169">Schema Name</span></span>  <br/> |<span data-ttu-id="cc7b3-170">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="cc7b3-170">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cc7b3-171">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cc7b3-171">Validation File</span></span>  <br/> |<span data-ttu-id="cc7b3-172">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="cc7b3-172">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cc7b3-173">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cc7b3-173">Can be Empty</span></span>  <br/> |<span data-ttu-id="cc7b3-174">False</span><span class="sxs-lookup"><span data-stu-id="cc7b3-174">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cc7b3-175">関連項目</span><span class="sxs-lookup"><span data-stu-id="cc7b3-175">See also</span></span>

- [<span data-ttu-id="cc7b3-176">CreateAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="cc7b3-176">CreateAttachment operation</span></span>](createattachment-operation.md) 
- [<span data-ttu-id="cc7b3-177">CreateAttachment</span><span class="sxs-lookup"><span data-stu-id="cc7b3-177">CreateAttachment</span></span>](createattachment.md)
- <span data-ttu-id="cc7b3-178">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="cc7b3-178">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span> 
- [<span data-ttu-id="cc7b3-179">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="cc7b3-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

