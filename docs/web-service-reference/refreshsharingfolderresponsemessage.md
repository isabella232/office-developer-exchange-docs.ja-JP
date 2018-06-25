---
title: RefreshSharingFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolderResponseMessage
api_type:
- schema
ms.assetid: 53ee65bd-cf75-4e04-9b27-eff1b040ae82
description: RefreshSharingFolderResponseMessage 要素には、状態および 1 つの RefreshSharingFolder 操作要求の結果が含まれています。
ms.openlocfilehash: 9dbb66c294439f33a9307d51c03dd1cd127e95e2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833052"
---
# <a name="refreshsharingfolderresponsemessage"></a><span data-ttu-id="c47b1-103">RefreshSharingFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c47b1-103">RefreshSharingFolderResponseMessage</span></span>

<span data-ttu-id="c47b1-104">**RefreshSharingFolderResponseMessage**要素には、状態および 1 つの結果が含まれている[RefreshSharingFolder の操作](refreshsharingfolder-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="c47b1-104">The **RefreshSharingFolderResponseMessage** element contains the status and result of a single [RefreshSharingFolder operation](refreshsharingfolder-operation.md) request.</span></span> 
  
```xml
<RefreshSharingFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RefreshSharingFolderResponseMessage>
```

 <span data-ttu-id="c47b1-105">**RefreshSharingFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c47b1-105">**RefreshSharingFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c47b1-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c47b1-106">Attributes and elements</span></span>

<span data-ttu-id="c47b1-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c47b1-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c47b1-108">属性</span><span class="sxs-lookup"><span data-stu-id="c47b1-108">Attributes</span></span>

|<span data-ttu-id="c47b1-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="c47b1-109">**Attribute**</span></span>|<span data-ttu-id="c47b1-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="c47b1-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c47b1-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="c47b1-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="c47b1-112">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c47b1-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="c47b1-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="c47b1-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="c47b1-114">-成功</span><span class="sxs-lookup"><span data-stu-id="c47b1-114">-  Success</span></span>  <br/><span data-ttu-id="c47b1-115">-警告</span><span class="sxs-lookup"><span data-stu-id="c47b1-115">-  Warning</span></span>  <br/><span data-ttu-id="c47b1-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="c47b1-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="c47b1-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="c47b1-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="c47b1-118">**値**</span><span class="sxs-lookup"><span data-stu-id="c47b1-118">**Value**</span></span>|<span data-ttu-id="c47b1-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="c47b1-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c47b1-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="c47b1-120">**Success**</span></span> <br/> |<span data-ttu-id="c47b1-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c47b1-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="c47b1-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="c47b1-122">**Warning**</span></span> <br/> | <span data-ttu-id="c47b1-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c47b1-123">Describes a request that was not processed.</span></span> <span data-ttu-id="c47b1-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="c47b1-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="c47b1-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c47b1-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="c47b1-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="c47b1-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="c47b1-127">-Active Directory ディレクトリ サービスは、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="c47b1-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="c47b1-128">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="c47b1-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="c47b1-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="c47b1-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="c47b1-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="c47b1-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="c47b1-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="c47b1-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="c47b1-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="c47b1-132">**Error**</span></span> <br/> | <span data-ttu-id="c47b1-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c47b1-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="c47b1-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="c47b1-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="c47b1-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="c47b1-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="c47b1-136">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="c47b1-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="c47b1-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="c47b1-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="c47b1-138">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="c47b1-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="c47b1-139">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="c47b1-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="c47b1-140">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="c47b1-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="c47b1-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="c47b1-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c47b1-142">子要素</span><span class="sxs-lookup"><span data-stu-id="c47b1-142">Child elements</span></span>

|<span data-ttu-id="c47b1-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="c47b1-143">**Element**</span></span>|<span data-ttu-id="c47b1-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="c47b1-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c47b1-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="c47b1-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c47b1-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="c47b1-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c47b1-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c47b1-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c47b1-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="c47b1-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="c47b1-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c47b1-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c47b1-150">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="c47b1-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="c47b1-151">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c47b1-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="c47b1-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c47b1-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c47b1-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="c47b1-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c47b1-154">親要素</span><span class="sxs-lookup"><span data-stu-id="c47b1-154">Parent elements</span></span>

|<span data-ttu-id="c47b1-155">**要素**</span><span class="sxs-lookup"><span data-stu-id="c47b1-155">**Element**</span></span>|<span data-ttu-id="c47b1-156">**説明**</span><span class="sxs-lookup"><span data-stu-id="c47b1-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c47b1-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c47b1-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="c47b1-158">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c47b1-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c47b1-159">備考</span><span class="sxs-lookup"><span data-stu-id="c47b1-159">Remarks</span></span>

<span data-ttu-id="c47b1-160">この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c47b1-160">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c47b1-161">要素情報</span><span class="sxs-lookup"><span data-stu-id="c47b1-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c47b1-162">名前空間</span><span class="sxs-lookup"><span data-stu-id="c47b1-162">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c47b1-163">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c47b1-163">Schema Name</span></span>  <br/> |<span data-ttu-id="c47b1-164">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="c47b1-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c47b1-165">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c47b1-165">Validation File</span></span>  <br/> |<span data-ttu-id="c47b1-166">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c47b1-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c47b1-167">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c47b1-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="c47b1-168">False</span><span class="sxs-lookup"><span data-stu-id="c47b1-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c47b1-169">関連項目</span><span class="sxs-lookup"><span data-stu-id="c47b1-169">See also</span></span>

- [<span data-ttu-id="c47b1-170">RefreshSharingFolder 操作</span><span class="sxs-lookup"><span data-stu-id="c47b1-170">RefreshSharingFolder operation</span></span>](refreshsharingfolder-operation.md)
- [<span data-ttu-id="c47b1-171">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c47b1-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

