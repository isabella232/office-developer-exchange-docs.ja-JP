---
title: RefreshSharingFolderResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- RefreshSharingFolderResponse
api_type:
- schema
ms.assetid: 951ab681-f2d5-4f10-933e-ff199685ff8e
description: RefreshSharingFolderResponse 要素は、RefreshSharingFolder 操作の要求に対する応答を定義します。
ms.openlocfilehash: 4ef7a63b2153c6106dae988439f499046689c2b4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833048"
---
# <a name="refreshsharingfolderresponse"></a><span data-ttu-id="59142-103">RefreshSharingFolderResponse</span><span class="sxs-lookup"><span data-stu-id="59142-103">RefreshSharingFolderResponse</span></span>

<span data-ttu-id="59142-104">**RefreshSharingFolderResponse**要素は、 [RefreshSharingFolder 操作](refreshsharingfolder-operation.md)の要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="59142-104">The **RefreshSharingFolderResponse** element defines a response to a [RefreshSharingFolder operation](refreshsharingfolder-operation.md) request.</span></span> 
  
```xml
<RefreshSharingFolderResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</RefreshSharingFolderResponse>
```

 <span data-ttu-id="59142-105">**RefreshSharingFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="59142-105">**RefreshSharingFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="59142-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="59142-106">Attributes and elements</span></span>

<span data-ttu-id="59142-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="59142-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="59142-108">属性</span><span class="sxs-lookup"><span data-stu-id="59142-108">Attributes</span></span>

|<span data-ttu-id="59142-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="59142-109">**Attribute**</span></span>|<span data-ttu-id="59142-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="59142-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="59142-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="59142-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="59142-112">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="59142-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="59142-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="59142-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="59142-114">-成功</span><span class="sxs-lookup"><span data-stu-id="59142-114">-  Success</span></span>  <br/><span data-ttu-id="59142-115">-警告</span><span class="sxs-lookup"><span data-stu-id="59142-115">-  Warning</span></span>  <br/><span data-ttu-id="59142-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="59142-116">-  Error</span></span>  <br/>- |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="59142-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="59142-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="59142-118">**値**</span><span class="sxs-lookup"><span data-stu-id="59142-118">**Value**</span></span>|<span data-ttu-id="59142-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="59142-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="59142-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="59142-120">**Success**</span></span> <br/> |<span data-ttu-id="59142-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="59142-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="59142-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="59142-122">**Warning**</span></span> <br/> | <span data-ttu-id="59142-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="59142-123">Describes a request that was not processed.</span></span> <span data-ttu-id="59142-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="59142-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="59142-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="59142-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="59142-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="59142-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="59142-127">-Active Directory ディレクトリ サービスは、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="59142-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="59142-128">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="59142-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="59142-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="59142-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="59142-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="59142-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="59142-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="59142-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="59142-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="59142-132">**Error**</span></span> <br/> | <span data-ttu-id="59142-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="59142-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="59142-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="59142-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="59142-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="59142-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="59142-136">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="59142-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="59142-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="59142-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="59142-138">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="59142-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="59142-139">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="59142-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="59142-140">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="59142-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/>  <br/><span data-ttu-id="59142-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="59142-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="59142-142">子要素</span><span class="sxs-lookup"><span data-stu-id="59142-142">Child elements</span></span>

|<span data-ttu-id="59142-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="59142-143">**Element**</span></span>|<span data-ttu-id="59142-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="59142-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="59142-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="59142-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="59142-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="59142-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="59142-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="59142-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="59142-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="59142-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="59142-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="59142-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="59142-150">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="59142-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="59142-151">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="59142-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="59142-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="59142-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="59142-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="59142-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="59142-154">親要素</span><span class="sxs-lookup"><span data-stu-id="59142-154">Parent elements</span></span>

<span data-ttu-id="59142-155">なし。</span><span class="sxs-lookup"><span data-stu-id="59142-155">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="59142-156">備考</span><span class="sxs-lookup"><span data-stu-id="59142-156">Remarks</span></span>

<span data-ttu-id="59142-157">この要素を記述するスキーマは、Microsoft Exchange Server を実行しているコンピューターの Exchange Web サービスをホストにクライアント アクセス サーバーの役割がインストールされている IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="59142-157">The schema that describes this element is located in the IIS Virtual directory that hosts Exchange Web Services of the computer that is running Microsoft Exchange Server that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="59142-158">要素情報</span><span class="sxs-lookup"><span data-stu-id="59142-158">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="59142-159">名前空間</span><span class="sxs-lookup"><span data-stu-id="59142-159">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="59142-160">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="59142-160">Schema Name</span></span>  <br/> |<span data-ttu-id="59142-161">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="59142-161">Messages schema</span></span>  <br/> |
|<span data-ttu-id="59142-162">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="59142-162">Validation File</span></span>  <br/> |<span data-ttu-id="59142-163">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="59142-163">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="59142-164">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="59142-164">Can be Empty</span></span>  <br/> |<span data-ttu-id="59142-165">False</span><span class="sxs-lookup"><span data-stu-id="59142-165">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="59142-166">関連項目</span><span class="sxs-lookup"><span data-stu-id="59142-166">See also</span></span>

- [<span data-ttu-id="59142-167">RefreshSharingFolder 操作</span><span class="sxs-lookup"><span data-stu-id="59142-167">RefreshSharingFolder operation</span></span>](refreshsharingfolder-operation.md)
- [<span data-ttu-id="59142-168">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="59142-168">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

