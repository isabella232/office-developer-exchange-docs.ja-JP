---
title: た getroomlistsresponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetRoomListsResponse
api_type:
- schema
ms.assetid: 8c736f68-1026-496a-b12f-c169c078abd0
description: た getroomlistsresponse 要素は、GetRoomLists 操作要求からの応答を定義します。
ms.openlocfilehash: b6d7c2baa2861309d72bcbf880eaed2ad0989175
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462944"
---
# <a name="getroomlistsresponse"></a><span data-ttu-id="3edd2-103">た getroomlistsresponse</span><span class="sxs-lookup"><span data-stu-id="3edd2-103">GetRoomListsResponse</span></span>

<span data-ttu-id="3edd2-104">**た getroomlistsresponse**要素は、 [GetRoomLists 操作](getroomlists-operation.md)要求からの応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="3edd2-104">The **GetRoomListsResponse** element defines the response from a [GetRoomLists operation](getroomlists-operation.md) request.</span></span> 
  
- [<span data-ttu-id="3edd2-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3edd2-105">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="3edd2-106">た getroomlistsresponse</span><span class="sxs-lookup"><span data-stu-id="3edd2-106">GetRoomListsResponse</span></span>](getroomlistsresponse.md)
  
```XML
<GetRoomListsResponse ResponseClass="">   
<MessageText/>   
<ResponseCode/>   
<DescriptiveLinkKey/>   
<MessageXml/>   
<RoomLists/>
</GetRoomListsResponse>
```

 <span data-ttu-id="3edd2-107">**GetRoomListsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3edd2-107">**GetRoomListsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3edd2-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="3edd2-108">Attributes and elements</span></span>

<span data-ttu-id="3edd2-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3edd2-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3edd2-110">属性</span><span class="sxs-lookup"><span data-stu-id="3edd2-110">Attributes</span></span>

|<span data-ttu-id="3edd2-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="3edd2-111">**Attribute**</span></span>|<span data-ttu-id="3edd2-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="3edd2-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3edd2-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="3edd2-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="3edd2-114">応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="3edd2-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="3edd2-115">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="3edd2-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="3edd2-116">-成功</span><span class="sxs-lookup"><span data-stu-id="3edd2-116">-  Success</span></span>  <br/><span data-ttu-id="3edd2-117">-Warning</span><span class="sxs-lookup"><span data-stu-id="3edd2-117">-  Warning</span></span>  <br/><span data-ttu-id="3edd2-118">-エラー</span><span class="sxs-lookup"><span data-stu-id="3edd2-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="3edd2-119">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="3edd2-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="3edd2-120">**値**</span><span class="sxs-lookup"><span data-stu-id="3edd2-120">**Value**</span></span>|<span data-ttu-id="3edd2-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="3edd2-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3edd2-122">**Success**</span><span class="sxs-lookup"><span data-stu-id="3edd2-122">**Success**</span></span> <br/> |<span data-ttu-id="3edd2-123">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="3edd2-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="3edd2-124">**Warning**</span><span class="sxs-lookup"><span data-stu-id="3edd2-124">**Warning**</span></span> <br/> | <span data-ttu-id="3edd2-125">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="3edd2-125">Describes a request that was not processed.</span></span> <span data-ttu-id="3edd2-126">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3edd2-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="3edd2-127">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3edd2-127">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="3edd2-128">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="3edd2-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="3edd2-129">-Active Directory ディレクトリサービスがオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="3edd2-129">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="3edd2-130">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="3edd2-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="3edd2-131">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="3edd2-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="3edd2-132">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="3edd2-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="3edd2-133">-クォータが限界を超えています。</span><span class="sxs-lookup"><span data-stu-id="3edd2-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="3edd2-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="3edd2-134">**Error**</span></span> <br/> | <span data-ttu-id="3edd2-135">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="3edd2-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="3edd2-136">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="3edd2-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="3edd2-137">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="3edd2-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="3edd2-138">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="3edd2-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="3edd2-139">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="3edd2-139">-  Unknown tag</span></span>  <br/><span data-ttu-id="3edd2-140">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="3edd2-140">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="3edd2-141">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="3edd2-141">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="3edd2-142">-有効なクライアント側の呼び出しに応答した場合のサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="3edd2-142">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="3edd2-143">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3edd2-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/>- |
   
### <a name="child-elements"></a><span data-ttu-id="3edd2-144">子要素</span><span class="sxs-lookup"><span data-stu-id="3edd2-144">Child elements</span></span>

|<span data-ttu-id="3edd2-145">**Element**</span><span class="sxs-lookup"><span data-stu-id="3edd2-145">**Element**</span></span>|<span data-ttu-id="3edd2-146">**説明**</span><span class="sxs-lookup"><span data-stu-id="3edd2-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3edd2-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="3edd2-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="3edd2-148">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="3edd2-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="3edd2-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3edd2-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="3edd2-150">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="3edd2-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="3edd2-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3edd2-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="3edd2-152">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="3edd2-152">Currently unused and reserved for future use.</span></span> <span data-ttu-id="3edd2-153">この要素には0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3edd2-153">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="3edd2-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="3edd2-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="3edd2-155">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="3edd2-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="3edd2-156">RoomLists</span><span class="sxs-lookup"><span data-stu-id="3edd2-156">RoomLists</span></span>](roomlists.md) <br/> |<span data-ttu-id="3edd2-157">会議室のリストを表す電子メールアドレスと表示名のリストを提供します。</span><span class="sxs-lookup"><span data-stu-id="3edd2-157">Provides a list of e-mail addresses and display names that represent lists of meeting rooms.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3edd2-158">親要素</span><span class="sxs-lookup"><span data-stu-id="3edd2-158">Parent elements</span></span>

|<span data-ttu-id="3edd2-159">**要素**</span><span class="sxs-lookup"><span data-stu-id="3edd2-159">**Element**</span></span>|<span data-ttu-id="3edd2-160">**説明**</span><span class="sxs-lookup"><span data-stu-id="3edd2-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3edd2-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="3edd2-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="3edd2-162">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="3edd2-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="element-information"></a><span data-ttu-id="3edd2-163">要素の情報</span><span class="sxs-lookup"><span data-stu-id="3edd2-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3edd2-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="3edd2-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3edd2-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3edd2-165">Schema Name</span></span>  <br/> |<span data-ttu-id="3edd2-166">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="3edd2-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3edd2-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3edd2-167">Validation File</span></span>  <br/> |<span data-ttu-id="3edd2-168">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="3edd2-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3edd2-169">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3edd2-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="3edd2-170">正しくない</span><span class="sxs-lookup"><span data-stu-id="3edd2-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3edd2-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="3edd2-171">See also</span></span>

- [<span data-ttu-id="3edd2-172">GetRoomLists 操作</span><span class="sxs-lookup"><span data-stu-id="3edd2-172">GetRoomLists operation</span></span>](getroomlists-operation.md)
- [<span data-ttu-id="3edd2-173">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="3edd2-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

