---
title: た getroomsresponse
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
description: た getroomsresponse 要素は、GetRooms 操作要求への応答を定義します。
ms.openlocfilehash: 661e143a9edd30f12ab83fb0666e2832422e280a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458587"
---
# <a name="getroomsresponse"></a><span data-ttu-id="74744-103">た getroomsresponse</span><span class="sxs-lookup"><span data-stu-id="74744-103">GetRoomsResponse</span></span>

<span data-ttu-id="74744-104">**た getroomsresponse**要素は、 [getrooms 操作](getrooms-operation.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="74744-104">The **GetRoomsResponse** element defines a response to a [GetRooms operation](getrooms-operation.md) request.</span></span> 
  
- [<span data-ttu-id="74744-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="74744-105">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="74744-106">た getroomsresponse</span><span class="sxs-lookup"><span data-stu-id="74744-106">GetRoomsResponse</span></span>](getroomsresponse.md)
  
```XML
<GetRoomsResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Rooms/>
</GetRoomsResponse>
```

 <span data-ttu-id="74744-107">**GetRoomsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="74744-107">**GetRoomsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="74744-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="74744-108">Attributes and elements</span></span>

<span data-ttu-id="74744-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="74744-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="74744-110">属性</span><span class="sxs-lookup"><span data-stu-id="74744-110">Attributes</span></span>

|<span data-ttu-id="74744-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="74744-111">**Attribute**</span></span>|<span data-ttu-id="74744-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="74744-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="74744-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="74744-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="74744-114">応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="74744-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="74744-115">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="74744-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="74744-116">-成功</span><span class="sxs-lookup"><span data-stu-id="74744-116">-  Success</span></span>  <br/><span data-ttu-id="74744-117">-Warning</span><span class="sxs-lookup"><span data-stu-id="74744-117">-  Warning</span></span>  <br/><span data-ttu-id="74744-118">-エラー</span><span class="sxs-lookup"><span data-stu-id="74744-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="74744-119">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="74744-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="74744-120">**値**</span><span class="sxs-lookup"><span data-stu-id="74744-120">**Value**</span></span>|<span data-ttu-id="74744-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="74744-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="74744-122">**Success**</span><span class="sxs-lookup"><span data-stu-id="74744-122">**Success**</span></span> <br/> |<span data-ttu-id="74744-123">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="74744-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="74744-124">**Warning**</span><span class="sxs-lookup"><span data-stu-id="74744-124">**Warning**</span></span> <br/> | <span data-ttu-id="74744-125">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="74744-125">Describes a request that was not processed.</span></span> <span data-ttu-id="74744-126">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="74744-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="74744-127">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74744-127">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="74744-128">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="74744-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="74744-129">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="74744-129">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="74744-130">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="74744-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="74744-131">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="74744-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="74744-132">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="74744-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="74744-133">-クォータが限界を超えています。</span><span class="sxs-lookup"><span data-stu-id="74744-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="74744-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="74744-134">**Error**</span></span> <br/> | <span data-ttu-id="74744-135">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="74744-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="74744-136">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="74744-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="74744-137">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="74744-137">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="74744-138">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="74744-138">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="74744-139">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="74744-139">-  An unknown tag</span></span>  <br/><span data-ttu-id="74744-140">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="74744-140">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="74744-141">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="74744-141">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="74744-142">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="74744-142">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="74744-143">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="74744-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="74744-144">子要素</span><span class="sxs-lookup"><span data-stu-id="74744-144">Child elements</span></span>

|<span data-ttu-id="74744-145">**Element**</span><span class="sxs-lookup"><span data-stu-id="74744-145">**Element**</span></span>|<span data-ttu-id="74744-146">**説明**</span><span class="sxs-lookup"><span data-stu-id="74744-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74744-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="74744-147">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="74744-148">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="74744-148">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="74744-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="74744-149">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="74744-150">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="74744-150">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="74744-151">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="74744-151">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="74744-152">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="74744-152">Currently unused and reserved for future use.</span></span> <span data-ttu-id="74744-153">この要素には0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="74744-153">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="74744-154">MessageXml</span><span class="sxs-lookup"><span data-stu-id="74744-154">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="74744-155">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="74744-155">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="74744-156">ルーム</span><span class="sxs-lookup"><span data-stu-id="74744-156">Rooms</span></span>](rooms.md) <br/> |<span data-ttu-id="74744-157">会議室を表す電子メールアドレスと表示名の一覧を提供します。</span><span class="sxs-lookup"><span data-stu-id="74744-157">Provides a list of email addresses and display names that represent meeting rooms.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="74744-158">親要素</span><span class="sxs-lookup"><span data-stu-id="74744-158">Parent elements</span></span>

|<span data-ttu-id="74744-159">**要素**</span><span class="sxs-lookup"><span data-stu-id="74744-159">**Element**</span></span>|<span data-ttu-id="74744-160">**説明**</span><span class="sxs-lookup"><span data-stu-id="74744-160">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="74744-161">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="74744-161">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="74744-162">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="74744-162">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="74744-163">注釈</span><span class="sxs-lookup"><span data-stu-id="74744-163">Remarks</span></span>

<span data-ttu-id="74744-164">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="74744-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="74744-165">要素の情報</span><span class="sxs-lookup"><span data-stu-id="74744-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="74744-166">Namespace</span><span class="sxs-lookup"><span data-stu-id="74744-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="74744-167">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="74744-167">Schema Name</span></span>  <br/> |<span data-ttu-id="74744-168">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="74744-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="74744-169">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="74744-169">Validation File</span></span>  <br/> |<span data-ttu-id="74744-170">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="74744-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="74744-171">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="74744-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="74744-172">正しくない</span><span class="sxs-lookup"><span data-stu-id="74744-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="74744-173">関連項目</span><span class="sxs-lookup"><span data-stu-id="74744-173">See also</span></span>

- [<span data-ttu-id="74744-174">GetRooms 操作</span><span class="sxs-lookup"><span data-stu-id="74744-174">GetRooms operation</span></span>](getrooms-operation.md)
- [<span data-ttu-id="74744-175">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="74744-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

