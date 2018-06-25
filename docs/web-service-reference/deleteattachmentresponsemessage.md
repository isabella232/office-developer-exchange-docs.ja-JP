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
description: DeleteAttachmentResponseMessage 要素には、状態および 1 つの DeleteAttachment 操作要求の結果が含まれています。
ms.openlocfilehash: 387e998a393c23f416cc5ad8d6c4a7ad4c92ebc7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759971"
---
# <a name="deleteattachmentresponsemessage"></a><span data-ttu-id="76c69-103">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76c69-103">DeleteAttachmentResponseMessage</span></span>

<span data-ttu-id="76c69-104">**DeleteAttachmentResponseMessage**要素には、状態および 1 つの結果が含まれています[DeleteAttachment 操作](deleteattachment-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="76c69-104">The **DeleteAttachmentResponseMessage** element contains the status and result of a single [DeleteAttachment operation](deleteattachment-operation.md) request.</span></span> 
  
- [<span data-ttu-id="76c69-105">DeleteAttachmentResponse</span><span class="sxs-lookup"><span data-stu-id="76c69-105">DeleteAttachmentResponse</span></span>](deleteattachmentresponse.md)  
- [<span data-ttu-id="76c69-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="76c69-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="76c69-107">DeleteAttachmentResponseMessage</span><span class="sxs-lookup"><span data-stu-id="76c69-107">DeleteAttachmentResponseMessage</span></span>](deleteattachmentresponsemessage.md)
  
```xml
<DeleteAttachmentResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootItemId/>
</DeleteAttachmentResponseMessage>
```

<span data-ttu-id="76c69-108">**DeleteAttachmentResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="76c69-108">**DeleteAttachmentResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="76c69-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="76c69-109">Attributes and elements</span></span>

<span data-ttu-id="76c69-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="76c69-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="76c69-111">属性</span><span class="sxs-lookup"><span data-stu-id="76c69-111">Attributes</span></span>

|<span data-ttu-id="76c69-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="76c69-112">**Attribute**</span></span>|<span data-ttu-id="76c69-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="76c69-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="76c69-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="76c69-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="76c69-115">[DeleteAttachment 操作](deleteattachment-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="76c69-115">Describes the status of a [DeleteAttachment operation](deleteattachment-operation.md) response.</span></span><br/><br/><span data-ttu-id="76c69-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="76c69-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="76c69-117">-成功</span><span class="sxs-lookup"><span data-stu-id="76c69-117">-  Success</span></span>  <br/><span data-ttu-id="76c69-118">-警告</span><span class="sxs-lookup"><span data-stu-id="76c69-118">-  Warning</span></span>  <br/><span data-ttu-id="76c69-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="76c69-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="76c69-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="76c69-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="76c69-121">**値**</span><span class="sxs-lookup"><span data-stu-id="76c69-121">**Value**</span></span>|<span data-ttu-id="76c69-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="76c69-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="76c69-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="76c69-123">**Success**</span></span> <br/> |<span data-ttu-id="76c69-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="76c69-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="76c69-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="76c69-125">**Warning**</span></span> <br/> | <span data-ttu-id="76c69-126">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="76c69-126">Describes a request that was not processed.</span></span> <span data-ttu-id="76c69-127">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="76c69-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="76c69-128">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="76c69-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="76c69-129">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="76c69-129">- The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="76c69-130">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="76c69-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="76c69-131">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="76c69-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="76c69-132">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="76c69-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="76c69-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="76c69-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="76c69-134">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="76c69-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="76c69-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="76c69-135">**Error**</span></span> <br/> | <span data-ttu-id="76c69-136">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="76c69-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="76c69-137">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="76c69-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="76c69-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="76c69-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="76c69-139">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="76c69-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="76c69-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="76c69-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="76c69-141">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="76c69-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="76c69-142">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="76c69-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="76c69-143">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="76c69-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="76c69-144">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="76c69-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="76c69-145">子要素</span><span class="sxs-lookup"><span data-stu-id="76c69-145">Child elements</span></span>

|<span data-ttu-id="76c69-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="76c69-146">**Element**</span></span>|<span data-ttu-id="76c69-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="76c69-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76c69-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="76c69-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="76c69-149">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="76c69-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="76c69-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="76c69-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="76c69-151">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="76c69-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="76c69-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="76c69-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="76c69-153">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="76c69-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="76c69-154">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="76c69-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="76c69-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="76c69-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="76c69-156">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="76c69-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="76c69-157">RootItemId</span><span class="sxs-lookup"><span data-stu-id="76c69-157">RootItemId</span></span>](rootitemid.md) <br/> |<span data-ttu-id="76c69-158">削除された添付ファイルの親項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="76c69-158">Identifies the parent item of a deleted attachment.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="76c69-159">親要素</span><span class="sxs-lookup"><span data-stu-id="76c69-159">Parent elements</span></span>

|<span data-ttu-id="76c69-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="76c69-160">**Element**</span></span>|<span data-ttu-id="76c69-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="76c69-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="76c69-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="76c69-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="76c69-163">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="76c69-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="76c69-164">備考</span><span class="sxs-lookup"><span data-stu-id="76c69-164">Remarks</span></span>

<span data-ttu-id="76c69-165">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="76c69-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="76c69-166">要素情報</span><span class="sxs-lookup"><span data-stu-id="76c69-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="76c69-167">名前空間</span><span class="sxs-lookup"><span data-stu-id="76c69-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="76c69-168">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="76c69-168">Schema Name</span></span>  <br/> |<span data-ttu-id="76c69-169">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="76c69-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="76c69-170">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="76c69-170">Validation File</span></span>  <br/> |<span data-ttu-id="76c69-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="76c69-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="76c69-172">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="76c69-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="76c69-173">False</span><span class="sxs-lookup"><span data-stu-id="76c69-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="76c69-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="76c69-174">See also</span></span>

- [<span data-ttu-id="76c69-175">DeleteAttachment</span><span class="sxs-lookup"><span data-stu-id="76c69-175">DeleteAttachment</span></span>](deleteattachment.md) 
- [<span data-ttu-id="76c69-176">DeleteAttachment 操作</span><span class="sxs-lookup"><span data-stu-id="76c69-176">DeleteAttachment operation</span></span>](deleteattachment-operation.md)
- <span data-ttu-id="76c69-177">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="76c69-177">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span> 
- [<span data-ttu-id="76c69-178">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="76c69-178">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

