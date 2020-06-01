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
description: GetSharingMetadataResponseMessage 要素には、1つの GetSharingMetadata 操作要求の状態と結果が含まれています。
ms.openlocfilehash: cca06cb12ce48ba182c4ebfe475b2acfcc861d63
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457341"
---
# <a name="getsharingmetadataresponsemessage"></a><span data-ttu-id="1d373-103">GetSharingMetadataResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1d373-103">GetSharingMetadataResponseMessage</span></span>

<span data-ttu-id="1d373-104">**GetSharingMetadataResponseMessage**要素には、1つの[getsharingmetadata 操作](getsharingmetadata-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1d373-104">The **GetSharingMetadataResponseMessage** element contains the status and result of a single [GetSharingMetadata operation](getsharingmetadata-operation.md) request.</span></span> 
  
```xml
<GetSharingMetadataResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <EncryptedSharedFolderDataCollection/>   <InvalidRecipients/>
</GetSharingMetadataResponseMessage>
```

 <span data-ttu-id="1d373-105">**GetSharingMetadataResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1d373-105">**GetSharingMetadataResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="1d373-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="1d373-106">Attributes and elements</span></span>

<span data-ttu-id="1d373-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1d373-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1d373-108">属性</span><span class="sxs-lookup"><span data-stu-id="1d373-108">Attributes</span></span>

|<span data-ttu-id="1d373-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="1d373-109">**Attribute**</span></span>|<span data-ttu-id="1d373-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="1d373-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1d373-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="1d373-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="1d373-112">応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="1d373-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="1d373-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="1d373-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="1d373-114">-成功</span><span class="sxs-lookup"><span data-stu-id="1d373-114">-  Success</span></span>  <br/><span data-ttu-id="1d373-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="1d373-115">-  Warning</span></span>  <br/><span data-ttu-id="1d373-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="1d373-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="1d373-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="1d373-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="1d373-118">**値**</span><span class="sxs-lookup"><span data-stu-id="1d373-118">**Value**</span></span>|<span data-ttu-id="1d373-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="1d373-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1d373-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="1d373-120">**Success**</span></span> <br/> |<span data-ttu-id="1d373-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="1d373-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="1d373-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="1d373-122">**Warning**</span></span> <br/> | <span data-ttu-id="1d373-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="1d373-123">Describes a request that was not processed.</span></span> <span data-ttu-id="1d373-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1d373-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="1d373-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1d373-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="1d373-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="1d373-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="1d373-127">-Active Directory ディレクトリサービスがオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="1d373-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="1d373-128">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="1d373-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="1d373-129">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="1d373-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="1d373-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="1d373-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="1d373-131">-クォータが限界を超えています。</span><span class="sxs-lookup"><span data-stu-id="1d373-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="1d373-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="1d373-132">**Error**</span></span> <br/> | <span data-ttu-id="1d373-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="1d373-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="1d373-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1d373-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="1d373-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="1d373-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="1d373-136">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="1d373-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="1d373-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="1d373-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="1d373-138">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="1d373-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="1d373-139">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="1d373-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="1d373-140">-有効なクライアント側の呼び出しに応答した場合のサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="1d373-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="1d373-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1d373-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1d373-142">子要素</span><span class="sxs-lookup"><span data-stu-id="1d373-142">Child elements</span></span>

|<span data-ttu-id="1d373-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="1d373-143">**Element**</span></span>|<span data-ttu-id="1d373-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="1d373-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d373-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="1d373-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="1d373-146">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="1d373-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="1d373-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1d373-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="1d373-148">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="1d373-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="1d373-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1d373-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="1d373-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="1d373-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="1d373-151">この要素には0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1d373-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="1d373-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="1d373-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="1d373-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="1d373-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="1d373-154">EncryptedSharedFolderDataCollection</span><span class="sxs-lookup"><span data-stu-id="1d373-154">EncryptedSharedFolderDataCollection</span></span>](encryptedsharedfolderdatacollection.md) <br/> |<span data-ttu-id="1d373-155">他のクライアントとの予定表または連絡先データの共有を承認するためにクライアントが使用できるデータ構造のコレクションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1d373-155">Contains a collection of data structures that a client can use to authorize the sharing of its calendar or contact data with other clients.</span></span>  <br/> |
|[<span data-ttu-id="1d373-156">InvalidRecipients</span><span class="sxs-lookup"><span data-stu-id="1d373-156">InvalidRecipients</span></span>](invalidrecipients.md) <br/> |<span data-ttu-id="1d373-157">無効なフォルダー共有要求の受信者を表します。</span><span class="sxs-lookup"><span data-stu-id="1d373-157">Represents recipients of the folder sharing request that are invalid.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1d373-158">親要素</span><span class="sxs-lookup"><span data-stu-id="1d373-158">Parent elements</span></span>

|<span data-ttu-id="1d373-159">**要素**</span><span class="sxs-lookup"><span data-stu-id="1d373-159">**Element**</span></span>|<span data-ttu-id="1d373-160">**説明**</span><span class="sxs-lookup"><span data-stu-id="1d373-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1d373-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1d373-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="1d373-162">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="1d373-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="1d373-163">注釈</span><span class="sxs-lookup"><span data-stu-id="1d373-163">Remarks</span></span>

<span data-ttu-id="1d373-164">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="1d373-164">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1d373-165">要素の情報</span><span class="sxs-lookup"><span data-stu-id="1d373-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1d373-166">Namespace</span><span class="sxs-lookup"><span data-stu-id="1d373-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1d373-167">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1d373-167">Schema Name</span></span>  <br/> |<span data-ttu-id="1d373-168">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="1d373-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1d373-169">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1d373-169">Validation File</span></span>  <br/> |<span data-ttu-id="1d373-170">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="1d373-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1d373-171">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1d373-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="1d373-172">正しくない</span><span class="sxs-lookup"><span data-stu-id="1d373-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1d373-173">関連項目</span><span class="sxs-lookup"><span data-stu-id="1d373-173">See also</span></span>

- [<span data-ttu-id="1d373-174">GetSharingMetadata 操作</span><span class="sxs-lookup"><span data-stu-id="1d373-174">GetSharingMetadata operation</span></span>](getsharingmetadata-operation.md)
- [<span data-ttu-id="1d373-175">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="1d373-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

