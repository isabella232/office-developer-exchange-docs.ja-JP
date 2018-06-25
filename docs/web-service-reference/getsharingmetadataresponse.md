---
title: GetSharingMetadataResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadataResponse
api_type:
- schema
ms.assetid: 1acc2d8f-7104-4b36-9c04-dd4fc4f571bb
description: GetSharingMetadataResponse 要素は、GetSharingMetadata 操作の要求に対する応答を定義します。
ms.openlocfilehash: 820b5bf7aa5528b61aa6649e5b1886885b5f022e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831676"
---
# <a name="getsharingmetadataresponse"></a><span data-ttu-id="9ba6d-103">GetSharingMetadataResponse</span><span class="sxs-lookup"><span data-stu-id="9ba6d-103">GetSharingMetadataResponse</span></span>

<span data-ttu-id="9ba6d-104">**GetSharingMetadataResponse**要素は、 [GetSharingMetadata 操作](getsharingmetadata-operation.md)の要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-104">The **GetSharingMetadataResponse** element defines a response to a [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span> 
  
```xml
<GetSharingMetadataResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <EncryptedSharedFolderDataCollection/>   <InvalidRecipients/>
</GetSharingMetadataResponse>
```

 <span data-ttu-id="9ba6d-105">**GetSharingMetadataResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="9ba6d-105">**GetSharingMetadataResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9ba6d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9ba6d-106">Attributes and elements</span></span>

<span data-ttu-id="9ba6d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9ba6d-108">属性</span><span class="sxs-lookup"><span data-stu-id="9ba6d-108">Attributes</span></span>

|<span data-ttu-id="9ba6d-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="9ba6d-109">**Attribute**</span></span>|<span data-ttu-id="9ba6d-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ba6d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9ba6d-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="9ba6d-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="9ba6d-112">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="9ba6d-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="9ba6d-114">-成功</span><span class="sxs-lookup"><span data-stu-id="9ba6d-114">-  Success</span></span>  <br/><span data-ttu-id="9ba6d-115">-警告</span><span class="sxs-lookup"><span data-stu-id="9ba6d-115">-  Warning</span></span>  <br/><span data-ttu-id="9ba6d-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="9ba6d-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="9ba6d-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="9ba6d-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="9ba6d-118">**値**</span><span class="sxs-lookup"><span data-stu-id="9ba6d-118">**Value**</span></span>|<span data-ttu-id="9ba6d-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ba6d-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9ba6d-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="9ba6d-120">**Success**</span></span> <br/> |<span data-ttu-id="9ba6d-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="9ba6d-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="9ba6d-122">**Warning**</span></span> <br/> | <span data-ttu-id="9ba6d-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-123">Describes a request that was not processed.</span></span> <span data-ttu-id="9ba6d-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="9ba6d-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="9ba6d-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="9ba6d-127">-Active Directory ディレクトリ サービスは、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="9ba6d-128">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="9ba6d-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="9ba6d-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="9ba6d-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="9ba6d-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="9ba6d-132">**Error**</span></span> <br/> | <span data-ttu-id="9ba6d-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="9ba6d-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="9ba6d-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="9ba6d-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="9ba6d-136">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="9ba6d-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="9ba6d-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="9ba6d-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="9ba6d-138">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="9ba6d-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="9ba6d-139">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="9ba6d-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="9ba6d-140">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="9ba6d-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/>  <br/><span data-ttu-id="9ba6d-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9ba6d-142">子要素</span><span class="sxs-lookup"><span data-stu-id="9ba6d-142">Child elements</span></span>

|<span data-ttu-id="9ba6d-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="9ba6d-143">**Element**</span></span>|<span data-ttu-id="9ba6d-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="9ba6d-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9ba6d-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="9ba6d-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="9ba6d-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="9ba6d-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9ba6d-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="9ba6d-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="9ba6d-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9ba6d-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="9ba6d-150">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="9ba6d-151">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="9ba6d-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="9ba6d-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="9ba6d-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="9ba6d-154">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="9ba6d-154">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="9ba6d-155">クライアントを使用してその予定表の共有を承認または連絡先データを他のクライアントとデータ構造体のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-155">Contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
|[<span data-ttu-id="9ba6d-156">InvalidRecipients</span><span class="sxs-lookup"><span data-stu-id="9ba6d-156">InvalidRecipients</span></span>](invalidrecipients.md) <br/> |<span data-ttu-id="9ba6d-157">無効な要求を共有フォルダーの受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-157">Represents recipients of the folder sharing request that are invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9ba6d-158">親要素</span><span class="sxs-lookup"><span data-stu-id="9ba6d-158">Parent elements</span></span>

<span data-ttu-id="9ba6d-159">なし。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9ba6d-160">備考</span><span class="sxs-lookup"><span data-stu-id="9ba6d-160">Remarks</span></span>

<span data-ttu-id="9ba6d-161">この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="9ba6d-161">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9ba6d-162">要素情報</span><span class="sxs-lookup"><span data-stu-id="9ba6d-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9ba6d-163">名前空間</span><span class="sxs-lookup"><span data-stu-id="9ba6d-163">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9ba6d-164">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9ba6d-164">Schema Name</span></span>  <br/> |<span data-ttu-id="9ba6d-165">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9ba6d-165">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9ba6d-166">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9ba6d-166">Validation File</span></span>  <br/> |<span data-ttu-id="9ba6d-167">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9ba6d-167">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9ba6d-168">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9ba6d-168">Can be Empty</span></span>  <br/> |<span data-ttu-id="9ba6d-169">False</span><span class="sxs-lookup"><span data-stu-id="9ba6d-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9ba6d-170">関連項目</span><span class="sxs-lookup"><span data-stu-id="9ba6d-170">See also</span></span>

- [<span data-ttu-id="9ba6d-171">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="9ba6d-171">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="9ba6d-172">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9ba6d-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

