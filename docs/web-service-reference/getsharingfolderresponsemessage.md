---
title: GetSharingFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetSharingFolderResponseMessage
api_type:
- schema
ms.assetid: b6f5fd09-09f3-4e34-84b4-2f6c1f10f28f
description: GetSharingFolderResponseMessage 要素には、状態および 1 つの GetSharingFolder 操作要求の結果が含まれています。
ms.openlocfilehash: 13ce3f628ff125140fc7459df5d567a67ddf7bc2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19831672"
---
# <a name="getsharingfolderresponsemessage"></a><span data-ttu-id="eb2f0-103">GetSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="eb2f0-103">GetSharingFolderResponseMessage</span></span>

<span data-ttu-id="eb2f0-104">**GetSharingFolderResponseMessage**要素には、状態および 1 つの結果が含まれている[GetSharingFolder の操作](getsharingfolder-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-104">The **GetSharingFolderResponseMessage** element contains the status and result of a single [GetSharingFolder operation](getsharingfolder-operation.md) request.</span></span> 
  
```xml
<GetSharingFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <SharingFolderId/>
</GetSharingFolderResponseMessage>
```

 <span data-ttu-id="eb2f0-105">**GetSharingFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="eb2f0-105">**GetSharingFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="eb2f0-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="eb2f0-106">Attributes and elements</span></span>

<span data-ttu-id="eb2f0-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="eb2f0-108">属性</span><span class="sxs-lookup"><span data-stu-id="eb2f0-108">Attributes</span></span>

|<span data-ttu-id="eb2f0-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="eb2f0-109">**Attribute**</span></span>|<span data-ttu-id="eb2f0-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="eb2f0-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="eb2f0-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="eb2f0-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="eb2f0-112">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="eb2f0-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="eb2f0-114">-成功</span><span class="sxs-lookup"><span data-stu-id="eb2f0-114">-  Success</span></span>  <br/><span data-ttu-id="eb2f0-115">-警告</span><span class="sxs-lookup"><span data-stu-id="eb2f0-115">-  Warning</span></span>  <br/><span data-ttu-id="eb2f0-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="eb2f0-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="eb2f0-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="eb2f0-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="eb2f0-118">**値**</span><span class="sxs-lookup"><span data-stu-id="eb2f0-118">**Value**</span></span>|<span data-ttu-id="eb2f0-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="eb2f0-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="eb2f0-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="eb2f0-120">**Success**</span></span> <br/> |<span data-ttu-id="eb2f0-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="eb2f0-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="eb2f0-122">**Warning**</span></span> <br/> | <span data-ttu-id="eb2f0-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-123">Describes a request that was not processed.</span></span> <span data-ttu-id="eb2f0-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="eb2f0-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="eb2f0-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="eb2f0-127">-Active Directory ディレクトリ サービスは、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="eb2f0-128">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="eb2f0-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="eb2f0-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="eb2f0-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="eb2f0-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="eb2f0-132">**Error**</span></span> <br/> | <span data-ttu-id="eb2f0-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="eb2f0-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="eb2f0-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="eb2f0-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="eb2f0-136">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="eb2f0-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="eb2f0-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="eb2f0-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="eb2f0-138">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="eb2f0-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="eb2f0-139">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="eb2f0-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="eb2f0-140">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="eb2f0-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="eb2f0-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="eb2f0-142">子要素</span><span class="sxs-lookup"><span data-stu-id="eb2f0-142">Child elements</span></span>

|<span data-ttu-id="eb2f0-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="eb2f0-143">**Element**</span></span>|<span data-ttu-id="eb2f0-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="eb2f0-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb2f0-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="eb2f0-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="eb2f0-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="eb2f0-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="eb2f0-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="eb2f0-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="eb2f0-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="eb2f0-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="eb2f0-150">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="eb2f0-151">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="eb2f0-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="eb2f0-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="eb2f0-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="eb2f0-154">SharingFolderId</span><span class="sxs-lookup"><span data-stu-id="eb2f0-154">SharingFolderId</span></span>](sharingfolderid.md) <br/> |<span data-ttu-id="eb2f0-155">共有関係では、ローカル フォルダーの識別子を表します。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-155">Represents the identifier of the local folder in a sharing relationship.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="eb2f0-156">親要素</span><span class="sxs-lookup"><span data-stu-id="eb2f0-156">Parent elements</span></span>

|<span data-ttu-id="eb2f0-157">**要素**</span><span class="sxs-lookup"><span data-stu-id="eb2f0-157">**Element**</span></span>|<span data-ttu-id="eb2f0-158">**説明**</span><span class="sxs-lookup"><span data-stu-id="eb2f0-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="eb2f0-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="eb2f0-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="eb2f0-160">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="eb2f0-161">備考</span><span class="sxs-lookup"><span data-stu-id="eb2f0-161">Remarks</span></span>

<span data-ttu-id="eb2f0-162">この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="eb2f0-162">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="eb2f0-163">要素情報</span><span class="sxs-lookup"><span data-stu-id="eb2f0-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="eb2f0-164">名前空間</span><span class="sxs-lookup"><span data-stu-id="eb2f0-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="eb2f0-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="eb2f0-165">Schema Name</span></span>  <br/> |<span data-ttu-id="eb2f0-166">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="eb2f0-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="eb2f0-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="eb2f0-167">Validation File</span></span>  <br/> |<span data-ttu-id="eb2f0-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="eb2f0-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="eb2f0-169">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="eb2f0-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="eb2f0-170">False</span><span class="sxs-lookup"><span data-stu-id="eb2f0-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="eb2f0-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="eb2f0-171">See also</span></span>

- [<span data-ttu-id="eb2f0-172">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="eb2f0-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

