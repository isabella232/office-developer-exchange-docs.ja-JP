---
title: FindConversationResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindConversationResponse
api_type:
- schema
ms.assetid: a689e29d-5f3d-4deb-81ee-8b6cc60f6dea
description: FindConversationResponse 要素は、FindConversation 操作の要求に対する応答を定義します。
ms.openlocfilehash: 5754ea7540fa6daac8cd725386ca213d5bf05c8e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760499"
---
# <a name="findconversationresponse"></a><span data-ttu-id="c2cc4-103">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="c2cc4-103">FindConversationResponse</span></span>

<span data-ttu-id="c2cc4-104">**FindConversationResponse**要素は、 [FindConversation 操作](findconversation-operation.md)の要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-104">The **FindConversationResponse** element defines a response to a [FindConversation operation](findconversation-operation.md) request.</span></span> 
  
[<span data-ttu-id="c2cc4-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="c2cc4-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
```XML
<FindConversationResponse ResponseClass="">
   <Conversations/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</FindConversationResponse>

```

 <span data-ttu-id="c2cc4-106">**FindConversationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c2cc4-106">**FindConversationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2cc4-107">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c2cc4-107">Attributes and elements</span></span>

<span data-ttu-id="c2cc4-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2cc4-109">属性</span><span class="sxs-lookup"><span data-stu-id="c2cc4-109">Attributes</span></span>

|<span data-ttu-id="c2cc4-110">**属性**</span><span class="sxs-lookup"><span data-stu-id="c2cc4-110">**Attribute**</span></span>|<span data-ttu-id="c2cc4-111">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2cc4-111">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c2cc4-112">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="c2cc4-112">**ResponseClass**</span></span> <br/> | <span data-ttu-id="c2cc4-113">[FindConversation 操作](findconversation-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-113">Describes the status of a [FindConversation operation](findconversation-operation.md) response.</span></span> <br/><br/><span data-ttu-id="c2cc4-114">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-114">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="c2cc4-115">-成功</span><span class="sxs-lookup"><span data-stu-id="c2cc4-115">-  Success</span></span>  <br/><span data-ttu-id="c2cc4-116">-警告</span><span class="sxs-lookup"><span data-stu-id="c2cc4-116">-  Warning</span></span>  <br/><span data-ttu-id="c2cc4-117">-エラー</span><span class="sxs-lookup"><span data-stu-id="c2cc4-117">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="c2cc4-118">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="c2cc4-118">ResponseClass attribute values</span></span>

|<span data-ttu-id="c2cc4-119">**値**</span><span class="sxs-lookup"><span data-stu-id="c2cc4-119">**Value**</span></span>|<span data-ttu-id="c2cc4-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2cc4-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c2cc4-121">**Success**</span><span class="sxs-lookup"><span data-stu-id="c2cc4-121">**Success**</span></span> <br/> |<span data-ttu-id="c2cc4-122">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-122">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="c2cc4-123">**Warning**</span><span class="sxs-lookup"><span data-stu-id="c2cc4-123">**Warning**</span></span> <br/> | <span data-ttu-id="c2cc4-124">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-124">Describes a request that was not processed.</span></span> <span data-ttu-id="c2cc4-125">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-125">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="c2cc4-126">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-126">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="c2cc4-127">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-127">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="c2cc4-128">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-128">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="c2cc4-129">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-129">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="c2cc4-130">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-130">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="c2cc4-131">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-131">-  A password is expired.</span></span>  <br/><span data-ttu-id="c2cc4-132">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-132">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="c2cc4-133">**Error**</span><span class="sxs-lookup"><span data-stu-id="c2cc4-133">**Error**</span></span> <br/> | <span data-ttu-id="c2cc4-134">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-134">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="c2cc4-135">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-135">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="c2cc4-136">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="c2cc4-136">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="c2cc4-137">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-137">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="c2cc4-138">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="c2cc4-138">-  An unknown tag</span></span>  <br/><span data-ttu-id="c2cc4-139">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-139">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="c2cc4-140">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="c2cc4-140">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="c2cc4-141">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="c2cc4-141">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="c2cc4-142">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-142">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c2cc4-143">子要素</span><span class="sxs-lookup"><span data-stu-id="c2cc4-143">Child elements</span></span>

|<span data-ttu-id="c2cc4-144">**要素**</span><span class="sxs-lookup"><span data-stu-id="c2cc4-144">**Element**</span></span>|<span data-ttu-id="c2cc4-145">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2cc4-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2cc4-146">スレッド</span><span class="sxs-lookup"><span data-stu-id="c2cc4-146">Conversations</span></span>](conversations-ex15websvcsotherref.md) <br/> |<span data-ttu-id="c2cc4-147">会話の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-147">Contains an array of conversations.</span></span>  <br/> |
|[<span data-ttu-id="c2cc4-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="c2cc4-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c2cc4-149">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c2cc4-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c2cc4-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c2cc4-151">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="c2cc4-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c2cc4-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c2cc4-153">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="c2cc4-154">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="c2cc4-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c2cc4-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c2cc4-156">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c2cc4-157">親要素</span><span class="sxs-lookup"><span data-stu-id="c2cc4-157">Parent elements</span></span>

<span data-ttu-id="c2cc4-158">なし。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-158">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="c2cc4-159">テキスト値</span><span class="sxs-lookup"><span data-stu-id="c2cc4-159">Text value</span></span>

<span data-ttu-id="c2cc4-160">なし。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c2cc4-161">備考</span><span class="sxs-lookup"><span data-stu-id="c2cc4-161">Remarks</span></span>

<span data-ttu-id="c2cc4-162">この要素を記述するスキーマは、Exchange Web Services.This の要素がホストをで Exchange Server 2010 Service Pack 1 (SP1) を導入する IIS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2cc4-163">要素情報</span><span class="sxs-lookup"><span data-stu-id="c2cc4-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2cc4-164">名前空間</span><span class="sxs-lookup"><span data-stu-id="c2cc4-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c2cc4-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c2cc4-165">Schema name</span></span>  <br/> |<span data-ttu-id="c2cc4-166">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="c2cc4-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c2cc4-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c2cc4-167">Validation file</span></span>  <br/> |<span data-ttu-id="c2cc4-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c2cc4-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c2cc4-169">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c2cc4-169">Can be empty</span></span>  <br/> |<span data-ttu-id="c2cc4-170">False</span><span class="sxs-lookup"><span data-stu-id="c2cc4-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2cc4-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="c2cc4-171">See also</span></span>

- <span data-ttu-id="c2cc4-172">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="c2cc4-172">[FindConversation operation](findconversation-operation.md)</span></span>
- [<span data-ttu-id="c2cc4-173">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="c2cc4-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="c2cc4-174">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="c2cc4-174">Conversations in EWS</span></span>](http://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

