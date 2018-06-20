---
title: GetRoomsResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRoomsResponse
api_type:
- schema
ms.assetid: a8c85f65-bb63-4e7a-b0ca-7c9a04560a58
description: GetRoomsResponse 要素は、GetRooms 操作の要求に対する応答を定義します。
ms.openlocfilehash: 7399ab910a99b39757eb752b11a4771ba81be46a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760849"
---
# <a name="getroomsresponse"></a><span data-ttu-id="faf5b-103">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="faf5b-103">GetRoomsResponse</span></span>

<span data-ttu-id="faf5b-104">**GetRoomsResponse**要素は、 [GetRooms 操作](getrooms-operation.md)の要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="faf5b-104">The **GetRoomsResponse** element defines a response to a [GetRooms operation](getrooms-operation.md) request.</span></span> 
  
- [<span data-ttu-id="faf5b-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="faf5b-105">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="faf5b-106">GetRoomsResponse</span><span class="sxs-lookup"><span data-stu-id="faf5b-106">GetRoomsResponse</span></span>](getroomsresponse.md)
  
```XML
<GetRoomsResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Rooms/>
</GetRoomsResponse>
```

 <span data-ttu-id="faf5b-107">**GetRoomsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="faf5b-107">**GetRoomsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="faf5b-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="faf5b-108">Attributes and elements</span></span>

<span data-ttu-id="faf5b-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="faf5b-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="faf5b-110">属性</span><span class="sxs-lookup"><span data-stu-id="faf5b-110">Attributes</span></span>

|<span data-ttu-id="faf5b-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="faf5b-111">**Attribute**</span></span>|<span data-ttu-id="faf5b-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="faf5b-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="faf5b-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="faf5b-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="faf5b-114">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="faf5b-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="faf5b-115">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="faf5b-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="faf5b-116">-成功</span><span class="sxs-lookup"><span data-stu-id="faf5b-116">-  Success</span></span>  <br/><span data-ttu-id="faf5b-117">-警告</span><span class="sxs-lookup"><span data-stu-id="faf5b-117">-  Warning</span></span>  <br/><span data-ttu-id="faf5b-118">-エラー</span><span class="sxs-lookup"><span data-stu-id="faf5b-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="faf5b-119">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="faf5b-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="faf5b-120">**値**</span><span class="sxs-lookup"><span data-stu-id="faf5b-120">**Value**</span></span>|<span data-ttu-id="faf5b-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="faf5b-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="faf5b-122">**Success**</span><span class="sxs-lookup"><span data-stu-id="faf5b-122">**Success**</span></span> <br/> |<span data-ttu-id="faf5b-123">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="faf5b-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="faf5b-124">**Warning**</span><span class="sxs-lookup"><span data-stu-id="faf5b-124">**Warning**</span></span> <br/> | <span data-ttu-id="faf5b-125">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="faf5b-125">Describes a request that was not processed.</span></span> <span data-ttu-id="faf5b-126">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="faf5b-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="faf5b-127">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="faf5b-127">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="faf5b-128">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="faf5b-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="faf5b-129">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="faf5b-129">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="faf5b-130">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="faf5b-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="faf5b-131">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="faf5b-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="faf5b-132">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="faf5b-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="faf5b-133">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="faf5b-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="faf5b-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="faf5b-134">**Error**</span></span> <br/> | <span data-ttu-id="faf5b-135">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="faf5b-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="faf5b-136">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="faf5b-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="faf5b-137">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="faf5b-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="faf5b-138">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="faf5b-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="faf5b-139">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="faf5b-139">-  An unknown tag</span></span>  <br/><span data-ttu-id="faf5b-140">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="faf5b-140">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="faf5b-141">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="faf5b-141">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="faf5b-142">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="faf5b-142">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="faf5b-143">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="faf5b-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="faf5b-144">子要素</span><span class="sxs-lookup"><span data-stu-id="faf5b-144">Child elements</span></span>

|<span data-ttu-id="faf5b-145">**要素**</span><span class="sxs-lookup"><span data-stu-id="faf5b-145">**Element**</span></span>|<span data-ttu-id="faf5b-146">**説明**</span><span class="sxs-lookup"><span data-stu-id="faf5b-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="faf5b-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="faf5b-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="faf5b-148">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="faf5b-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="faf5b-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="faf5b-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="faf5b-150">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="faf5b-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="faf5b-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="faf5b-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="faf5b-152">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="faf5b-152">Currently unused and reserved for future use.</span></span> <span data-ttu-id="faf5b-153">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="faf5b-153">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="faf5b-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="faf5b-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="faf5b-155">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="faf5b-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="faf5b-156">ルーム</span><span class="sxs-lookup"><span data-stu-id="faf5b-156">Rooms</span></span>](rooms.md) <br/> |<span data-ttu-id="faf5b-157">電子メール アドレス、および会議室を表す表示名の一覧を示します。</span><span class="sxs-lookup"><span data-stu-id="faf5b-157">Provides a list of email addresses and display names that represent meeting rooms.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="faf5b-158">親要素</span><span class="sxs-lookup"><span data-stu-id="faf5b-158">Parent elements</span></span>

|<span data-ttu-id="faf5b-159">**要素**</span><span class="sxs-lookup"><span data-stu-id="faf5b-159">**Element**</span></span>|<span data-ttu-id="faf5b-160">**説明**</span><span class="sxs-lookup"><span data-stu-id="faf5b-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="faf5b-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="faf5b-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="faf5b-162">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="faf5b-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="faf5b-163">備考</span><span class="sxs-lookup"><span data-stu-id="faf5b-163">Remarks</span></span>

<span data-ttu-id="faf5b-164">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="faf5b-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="faf5b-165">要素情報</span><span class="sxs-lookup"><span data-stu-id="faf5b-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="faf5b-166">名前空間</span><span class="sxs-lookup"><span data-stu-id="faf5b-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="faf5b-167">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="faf5b-167">Schema Name</span></span>  <br/> |<span data-ttu-id="faf5b-168">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="faf5b-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="faf5b-169">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="faf5b-169">Validation File</span></span>  <br/> |<span data-ttu-id="faf5b-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="faf5b-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="faf5b-171">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="faf5b-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="faf5b-172">False</span><span class="sxs-lookup"><span data-stu-id="faf5b-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="faf5b-173">関連項目</span><span class="sxs-lookup"><span data-stu-id="faf5b-173">See also</span></span>

- [<span data-ttu-id="faf5b-174">GetRooms 操作</span><span class="sxs-lookup"><span data-stu-id="faf5b-174">GetRooms operation</span></span>](getrooms-operation.md)
- [<span data-ttu-id="faf5b-175">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="faf5b-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

