---
title: ApplyConversationActionResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ApplyConversationActionResponseMessage
api_type:
- schema
ms.assetid: a09edc89-7f2f-4846-a3a5-06694c97b9f6
description: ApplyConversationActionResponseMessage 要素には、ステータスと ApplyConversationAction の操作要求の結果が含まれています。
ms.openlocfilehash: d8c5571cfc9c2ea6aaf09cb26a0e47e4abfc3f40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759414"
---
# <a name="applyconversationactionresponsemessage"></a><span data-ttu-id="be727-103">ApplyConversationActionResponseMessage</span><span class="sxs-lookup"><span data-stu-id="be727-103">ApplyConversationActionResponseMessage</span></span>

<span data-ttu-id="be727-104">**ApplyConversationActionResponseMessage**要素には、ステータスと[ApplyConversationAction の操作](applyconversationaction-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="be727-104">The **ApplyConversationActionResponseMessage** element contains the status and results of an [ApplyConversationAction operation](applyconversationaction-operation.md) request.</span></span>  
  
- [<span data-ttu-id="be727-105">ApplyConversationActionResponse</span><span class="sxs-lookup"><span data-stu-id="be727-105">ApplyConversationActionResponse</span></span>](applyconversationactionresponse.md)
- [<span data-ttu-id="be727-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="be727-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="be727-107">ApplyConversationActionResponseMessage</span><span class="sxs-lookup"><span data-stu-id="be727-107">ApplyConversationActionResponseMessage</span></span>](applyconversationactionresponsemessage.md)
  
```XML
<ApplyConversationActionResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ApplyConversationActionResponseMessage>
```

 <span data-ttu-id="be727-108">**ApplyConversationActionResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="be727-108">**ApplyConversationActionResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="be727-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="be727-109">Attributes and elements</span></span>

<span data-ttu-id="be727-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="be727-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="be727-111">属性</span><span class="sxs-lookup"><span data-stu-id="be727-111">Attributes</span></span>

|<span data-ttu-id="be727-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="be727-112">**Attribute**</span></span>|<span data-ttu-id="be727-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="be727-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="be727-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="be727-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="be727-115">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="be727-115">Describes the status of the response.</span></span><br/><br/><span data-ttu-id="be727-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="be727-116">The following values are valid for this attribute:</span></span><ul><li><span data-ttu-id="be727-117">成功</span><span class="sxs-lookup"><span data-stu-id="be727-117">Success</span></span></li><li><span data-ttu-id="be727-118">警告</span><span class="sxs-lookup"><span data-stu-id="be727-118">Warning</span></span></li><li><span data-ttu-id="be727-119">エラー</span><span class="sxs-lookup"><span data-stu-id="be727-119">Error</span></span></li></ul> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="be727-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="be727-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="be727-121">**値**</span><span class="sxs-lookup"><span data-stu-id="be727-121">**Value**</span></span>|<span data-ttu-id="be727-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="be727-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="be727-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="be727-123">**Success**</span></span> <br/> |<span data-ttu-id="be727-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="be727-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="be727-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="be727-125">**Warning**</span></span> <br/> | <span data-ttu-id="be727-126">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="be727-126">Describes a request that was not processed.</span></span> <span data-ttu-id="be727-127">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="be727-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="be727-128">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="be727-128">The following are examples of sources of warnings:</span></span><ul><li><span data-ttu-id="be727-129">Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="be727-129">The Exchange store is offline during the batch.</span></span></li><li><span data-ttu-id="be727-130">Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="be727-130">Active Directory Domain Services (AD DS) is offline.</span></span></li><li><span data-ttu-id="be727-131">メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="be727-131">Mailboxes were moved.</span></span></li><li><span data-ttu-id="be727-132">メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="be727-132">The message database (MDB) is offline.</span></span></li><li><span data-ttu-id="be727-133">パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="be727-133">A password is expired.</span></span></li><li><span data-ttu-id="be727-134">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="be727-134">A quota has been exceeded.</span></span></li></ul> |
|<span data-ttu-id="be727-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="be727-135">**Error**</span></span> <br/> | <span data-ttu-id="be727-136">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="be727-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="be727-137">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="be727-137">The following are examples of sources of errors:</span></span>  <ul><li><span data-ttu-id="be727-138">無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="be727-138">Invalid attributes or elements</span></span></li><li><span data-ttu-id="be727-139">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="be727-139">Attributes or elements that are out of range</span></span></li><li><span data-ttu-id="be727-140">不明なタグ</span><span class="sxs-lookup"><span data-stu-id="be727-140">An unknown tag</span></span>  </li><li><span data-ttu-id="be727-141">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="be727-141">An attribute or element that is not valid in the context</span></span></li><li><span data-ttu-id="be727-142">任意のクライアントから不正なアクセスの試行</span><span class="sxs-lookup"><span data-stu-id="be727-142">An unauthorized access attempt by any client</span></span></li><li><span data-ttu-id="be727-143">有効なクライアント側の呼び出しへの応答でサーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="be727-143">A server-side failure in response to a valid client-side call</span></span></li></ul><span data-ttu-id="be727-144">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="be727-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="be727-145">子要素</span><span class="sxs-lookup"><span data-stu-id="be727-145">Child elements</span></span>

|<span data-ttu-id="be727-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="be727-146">**Element**</span></span>|<span data-ttu-id="be727-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="be727-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be727-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="be727-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="be727-149">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="be727-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="be727-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="be727-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="be727-151">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="be727-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="be727-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="be727-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="be727-153">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="be727-153">Currently unused and reserved for future use.</span></span> <span data-ttu-id="be727-154">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="be727-154">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="be727-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="be727-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="be727-156">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="be727-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="be727-157">親要素</span><span class="sxs-lookup"><span data-stu-id="be727-157">Parent elements</span></span>

|<span data-ttu-id="be727-158">**要素**</span><span class="sxs-lookup"><span data-stu-id="be727-158">**Element**</span></span>|<span data-ttu-id="be727-159">**説明**</span><span class="sxs-lookup"><span data-stu-id="be727-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="be727-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="be727-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="be727-161">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="be727-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="be727-162">テキスト値</span><span class="sxs-lookup"><span data-stu-id="be727-162">Text value</span></span>

<span data-ttu-id="be727-163">なし。</span><span class="sxs-lookup"><span data-stu-id="be727-163">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="be727-164">備考</span><span class="sxs-lookup"><span data-stu-id="be727-164">Remarks</span></span>

<span data-ttu-id="be727-165">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="be727-165">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="be727-166">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="be727-166">Version differences</span></span>

<span data-ttu-id="be727-167">Exchange のビルド 15.00.0986.00 以降のバージョンでは、 **ApplyConversationActionResponseMessage**要素は型**ApplyConversationActionResponseMessageType**のです。</span><span class="sxs-lookup"><span data-stu-id="be727-167">In versions of Exchange starting with build 15.00.0986.00, the **ApplyConversationActionResponseMessage** element is of type **ApplyConversationActionResponseMessageType**.</span></span> <span data-ttu-id="be727-168">以前のバージョンでは、型**ResponseMessageType**の要素です。</span><span class="sxs-lookup"><span data-stu-id="be727-168">In previous versions, the element is of type **ResponseMessageType**.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="be727-169">要素情報</span><span class="sxs-lookup"><span data-stu-id="be727-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="be727-170">名前空間</span><span class="sxs-lookup"><span data-stu-id="be727-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="be727-171">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="be727-171">Schema Name</span></span>  <br/> |<span data-ttu-id="be727-172">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="be727-172">Message schema</span></span>  <br/> |
|<span data-ttu-id="be727-173">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="be727-173">Validation File</span></span>  <br/> |<span data-ttu-id="be727-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="be727-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="be727-175">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="be727-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="be727-176">False</span><span class="sxs-lookup"><span data-stu-id="be727-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="be727-177">関連項目</span><span class="sxs-lookup"><span data-stu-id="be727-177">See also</span></span>

- [<span data-ttu-id="be727-178">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="be727-178">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
- [<span data-ttu-id="be727-179">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="be727-179">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

