---
title: GetSharingMetadataResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingMetadataResponseMessage
api_type:
- schema
ms.assetid: d81b8708-ebb2-45c2-861f-b9a814eee6ba
description: GetSharingMetadataResponseMessage 要素には、状態および 1 つの GetSharingMetadata 操作要求の結果が含まれています。
ms.openlocfilehash: 24da0a78870b2c92e0751eba0631d58076b96eae
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831674"
---
# <a name="getsharingmetadataresponsemessage"></a><span data-ttu-id="1f44f-103">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1f44f-103">GetSharingMetadataResponseMessage</span></span>

<span data-ttu-id="1f44f-104">**GetSharingMetadataResponseMessage**要素には、状態および 1 つの結果が含まれている[GetSharingMetadata の操作](getsharingmetadata-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="1f44f-104">The **GetSharingMetadataResponseMessage** element contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span> 
  
```xml
<GetSharingMetadataResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <EncryptedSharedFolderDataCollection/>   <InvalidRecipients/>
</GetSharingMetadataResponseMessage>
```

 <span data-ttu-id="1f44f-105">**GetSharingMetadataResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1f44f-105">**GetSharingMetadataResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1f44f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1f44f-106">Attributes and elements</span></span>

<span data-ttu-id="1f44f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1f44f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1f44f-108">属性</span><span class="sxs-lookup"><span data-stu-id="1f44f-108">Attributes</span></span>

|<span data-ttu-id="1f44f-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="1f44f-109">**Attribute**</span></span>|<span data-ttu-id="1f44f-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f44f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1f44f-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="1f44f-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="1f44f-112">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1f44f-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="1f44f-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="1f44f-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="1f44f-114">-成功</span><span class="sxs-lookup"><span data-stu-id="1f44f-114">-  Success</span></span>  <br/><span data-ttu-id="1f44f-115">-警告</span><span class="sxs-lookup"><span data-stu-id="1f44f-115">-  Warning</span></span>  <br/><span data-ttu-id="1f44f-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="1f44f-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="1f44f-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="1f44f-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="1f44f-118">**値**</span><span class="sxs-lookup"><span data-stu-id="1f44f-118">**Value**</span></span>|<span data-ttu-id="1f44f-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f44f-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1f44f-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="1f44f-120">**Success**</span></span> <br/> |<span data-ttu-id="1f44f-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1f44f-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="1f44f-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="1f44f-122">**Warning**</span></span> <br/> | <span data-ttu-id="1f44f-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1f44f-123">Describes a request that was not processed.</span></span> <span data-ttu-id="1f44f-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="1f44f-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="1f44f-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1f44f-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="1f44f-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="1f44f-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="1f44f-127">-Active Directory ディレクトリ サービスは、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="1f44f-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="1f44f-128">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="1f44f-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="1f44f-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="1f44f-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="1f44f-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="1f44f-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="1f44f-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="1f44f-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="1f44f-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="1f44f-132">**Error**</span></span> <br/> | <span data-ttu-id="1f44f-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1f44f-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="1f44f-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="1f44f-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="1f44f-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="1f44f-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="1f44f-136">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="1f44f-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="1f44f-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="1f44f-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="1f44f-138">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="1f44f-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="1f44f-139">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="1f44f-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="1f44f-140">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="1f44f-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="1f44f-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="1f44f-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1f44f-142">子要素</span><span class="sxs-lookup"><span data-stu-id="1f44f-142">Child elements</span></span>

|<span data-ttu-id="1f44f-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="1f44f-143">**Element**</span></span>|<span data-ttu-id="1f44f-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f44f-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f44f-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="1f44f-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="1f44f-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="1f44f-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="1f44f-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1f44f-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="1f44f-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="1f44f-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="1f44f-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1f44f-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="1f44f-150">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="1f44f-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="1f44f-151">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1f44f-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="1f44f-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="1f44f-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="1f44f-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="1f44f-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="1f44f-154">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="1f44f-154">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="1f44f-155">クライアントを使用してその予定表の共有を承認または連絡先データを他のクライアントとデータ構造体のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1f44f-155">Contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
|[<span data-ttu-id="1f44f-156">InvalidRecipients</span><span class="sxs-lookup"><span data-stu-id="1f44f-156">InvalidRecipients</span></span>](invalidrecipients.md) <br/> |<span data-ttu-id="1f44f-157">無効な要求を共有フォルダーの受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="1f44f-157">Represents recipients of the folder sharing request that are invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1f44f-158">親要素</span><span class="sxs-lookup"><span data-stu-id="1f44f-158">Parent elements</span></span>

|<span data-ttu-id="1f44f-159">**要素**</span><span class="sxs-lookup"><span data-stu-id="1f44f-159">**Element**</span></span>|<span data-ttu-id="1f44f-160">**説明**</span><span class="sxs-lookup"><span data-stu-id="1f44f-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1f44f-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1f44f-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="1f44f-162">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1f44f-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1f44f-163">備考</span><span class="sxs-lookup"><span data-stu-id="1f44f-163">Remarks</span></span>

<span data-ttu-id="1f44f-164">この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1f44f-164">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1f44f-165">要素情報</span><span class="sxs-lookup"><span data-stu-id="1f44f-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1f44f-166">名前空間</span><span class="sxs-lookup"><span data-stu-id="1f44f-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1f44f-167">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1f44f-167">Schema Name</span></span>  <br/> |<span data-ttu-id="1f44f-168">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="1f44f-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1f44f-169">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1f44f-169">Validation File</span></span>  <br/> |<span data-ttu-id="1f44f-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1f44f-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1f44f-171">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1f44f-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="1f44f-172">False</span><span class="sxs-lookup"><span data-stu-id="1f44f-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1f44f-173">関連項目</span><span class="sxs-lookup"><span data-stu-id="1f44f-173">See also</span></span>

- [<span data-ttu-id="1f44f-174">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="1f44f-174">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="1f44f-175">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1f44f-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

