---
title: EmptyFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 678dd5ce-8d9e-4939-bf1b-a8e148f4f449
description: EmptyFolderResponseMessage 要素には、状態および 1 つの EmptyFolder 要求の結果が含まれています。
ms.openlocfilehash: ebdaac28cdd16a55811276ef0d11c03b00d3897a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760271"
---
# <a name="emptyfolderresponsemessage"></a><span data-ttu-id="9e2d8-103">EmptyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9e2d8-103">EmptyFolderResponseMessage</span></span>

<span data-ttu-id="9e2d8-104">**EmptyFolderResponseMessage**要素には、状態および 1 つの[EmptyFolder](emptyfolder.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-104">The **EmptyFolderResponseMessage** element contains the status and result of a single [EmptyFolder](emptyfolder.md) request.</span></span> 
  
```XML
<EmptyFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</EmptyFolderResponseMessage>
```

 <span data-ttu-id="9e2d8-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="9e2d8-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9e2d8-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9e2d8-106">Attributes and elements</span></span>

<span data-ttu-id="9e2d8-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9e2d8-108">属性</span><span class="sxs-lookup"><span data-stu-id="9e2d8-108">Attributes</span></span>

|<span data-ttu-id="9e2d8-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="9e2d8-109">**Attribute**</span></span>|<span data-ttu-id="9e2d8-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="9e2d8-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9e2d8-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="9e2d8-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="9e2d8-112">[EmptyFolder 操作](emptyfolder-operation.md)応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-112">Describes the status of an [EmptyFolder operation](emptyfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="9e2d8-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="9e2d8-114">-成功</span><span class="sxs-lookup"><span data-stu-id="9e2d8-114">-  Success</span></span>  <br/><span data-ttu-id="9e2d8-115">-警告</span><span class="sxs-lookup"><span data-stu-id="9e2d8-115">-  Warning</span></span>  <br/><span data-ttu-id="9e2d8-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="9e2d8-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="9e2d8-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="9e2d8-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="9e2d8-118">**値**</span><span class="sxs-lookup"><span data-stu-id="9e2d8-118">**Value**</span></span>|<span data-ttu-id="9e2d8-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="9e2d8-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9e2d8-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="9e2d8-120">**Success**</span></span> <br/> |<span data-ttu-id="9e2d8-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="9e2d8-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="9e2d8-122">**Warning**</span></span> <br/> | <span data-ttu-id="9e2d8-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-123">Describes a request that was not processed.</span></span> <span data-ttu-id="9e2d8-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="9e2d8-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="9e2d8-126">-Exchange ストアは、バッチの中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-126">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="9e2d8-127">-Active Directory ドメイン サービス (AD DS) がオフラインになった。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-127">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="9e2d8-128">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="9e2d8-129">-メッセージ データベース (MDB) がオフラインになった。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-129">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="9e2d8-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="9e2d8-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="9e2d8-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="9e2d8-132">**Error**</span></span> <br/> | <span data-ttu-id="9e2d8-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="9e2d8-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="9e2d8-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="9e2d8-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="9e2d8-136">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="9e2d8-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="9e2d8-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="9e2d8-138">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="9e2d8-139">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="9e2d8-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="9e2d8-140">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="9e2d8-140">-  A server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="9e2d8-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9e2d8-142">子要素</span><span class="sxs-lookup"><span data-stu-id="9e2d8-142">Child elements</span></span>

|<span data-ttu-id="9e2d8-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="9e2d8-143">**Element**</span></span>|<span data-ttu-id="9e2d8-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="9e2d8-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e2d8-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="9e2d8-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="9e2d8-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="9e2d8-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9e2d8-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="9e2d8-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="9e2d8-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9e2d8-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="9e2d8-150">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="9e2d8-151">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-151">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="9e2d8-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="9e2d8-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="9e2d8-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9e2d8-154">親要素</span><span class="sxs-lookup"><span data-stu-id="9e2d8-154">Parent elements</span></span>

|<span data-ttu-id="9e2d8-155">**要素**</span><span class="sxs-lookup"><span data-stu-id="9e2d8-155">**Element**</span></span>|<span data-ttu-id="9e2d8-156">**説明**</span><span class="sxs-lookup"><span data-stu-id="9e2d8-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9e2d8-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="9e2d8-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="9e2d8-158">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="9e2d8-159">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9e2d8-159">Text value</span></span>

<span data-ttu-id="9e2d8-160">なし。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9e2d8-161">備考</span><span class="sxs-lookup"><span data-stu-id="9e2d8-161">Remarks</span></span>

<span data-ttu-id="9e2d8-162">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9e2d8-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9e2d8-163">要素情報</span><span class="sxs-lookup"><span data-stu-id="9e2d8-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9e2d8-164">名前空間</span><span class="sxs-lookup"><span data-stu-id="9e2d8-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9e2d8-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9e2d8-165">Schema Name</span></span>  <br/> |<span data-ttu-id="9e2d8-166">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9e2d8-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9e2d8-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9e2d8-167">Validation File</span></span>  <br/> |<span data-ttu-id="9e2d8-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9e2d8-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9e2d8-169">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="9e2d8-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="9e2d8-170">False</span><span class="sxs-lookup"><span data-stu-id="9e2d8-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9e2d8-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="9e2d8-171">See also</span></span>

- [<span data-ttu-id="9e2d8-172">EmptyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="9e2d8-172">EmptyFolder operation</span></span>](emptyfolder-operation.md)
- <span data-ttu-id="9e2d8-173">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="9e2d8-173">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span> 
- [<span data-ttu-id="9e2d8-174">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="9e2d8-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

