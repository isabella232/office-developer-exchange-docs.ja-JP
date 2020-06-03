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
description: FindConversationResponse 要素は、FindConversation 操作要求への応答を定義します。
ms.openlocfilehash: 68acc42045b91ab4b574f32ba3fd622057863015
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462641"
---
# <a name="findconversationresponse"></a><span data-ttu-id="362bd-103">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="362bd-103">FindConversationResponse</span></span>

<span data-ttu-id="362bd-104">**FindConversationResponse**要素は、 [findconversation 操作](findconversation-operation.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="362bd-104">The **FindConversationResponse** element defines a response to a [FindConversation operation](findconversation-operation.md) request.</span></span> 
  
[<span data-ttu-id="362bd-105">FindConversationResponse</span><span class="sxs-lookup"><span data-stu-id="362bd-105">FindConversationResponse</span></span>](findconversationresponse.md)
  
```XML
<FindConversationResponse ResponseClass="">
   <Conversations/>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</FindConversationResponse>

```

 <span data-ttu-id="362bd-106">**FindConversationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="362bd-106">**FindConversationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="362bd-107">属性と要素</span><span class="sxs-lookup"><span data-stu-id="362bd-107">Attributes and elements</span></span>

<span data-ttu-id="362bd-108">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="362bd-108">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="362bd-109">属性</span><span class="sxs-lookup"><span data-stu-id="362bd-109">Attributes</span></span>

|<span data-ttu-id="362bd-110">**属性**</span><span class="sxs-lookup"><span data-stu-id="362bd-110">**Attribute**</span></span>|<span data-ttu-id="362bd-111">**説明**</span><span class="sxs-lookup"><span data-stu-id="362bd-111">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="362bd-112">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="362bd-112">**ResponseClass**</span></span> <br/> | <span data-ttu-id="362bd-113">[Findconversation 操作](findconversation-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="362bd-113">Describes the status of a [FindConversation operation](findconversation-operation.md) response.</span></span> <br/><br/><span data-ttu-id="362bd-114">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="362bd-114">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="362bd-115">-成功</span><span class="sxs-lookup"><span data-stu-id="362bd-115">-  Success</span></span>  <br/><span data-ttu-id="362bd-116">-Warning</span><span class="sxs-lookup"><span data-stu-id="362bd-116">-  Warning</span></span>  <br/><span data-ttu-id="362bd-117">-エラー</span><span class="sxs-lookup"><span data-stu-id="362bd-117">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="362bd-118">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="362bd-118">ResponseClass attribute values</span></span>

|<span data-ttu-id="362bd-119">**値**</span><span class="sxs-lookup"><span data-stu-id="362bd-119">**Value**</span></span>|<span data-ttu-id="362bd-120">**説明**</span><span class="sxs-lookup"><span data-stu-id="362bd-120">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="362bd-121">**Success**</span><span class="sxs-lookup"><span data-stu-id="362bd-121">**Success**</span></span> <br/> |<span data-ttu-id="362bd-122">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="362bd-122">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="362bd-123">**Warning**</span><span class="sxs-lookup"><span data-stu-id="362bd-123">**Warning**</span></span> <br/> | <span data-ttu-id="362bd-124">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="362bd-124">Describes a request that was not processed.</span></span> <span data-ttu-id="362bd-125">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="362bd-125">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="362bd-126">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="362bd-126">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="362bd-127">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="362bd-127">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="362bd-128">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="362bd-128">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="362bd-129">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="362bd-129">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="362bd-130">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="362bd-130">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="362bd-131">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="362bd-131">-  A password is expired.</span></span>  <br/><span data-ttu-id="362bd-132">-クォータが限界を超えています。</span><span class="sxs-lookup"><span data-stu-id="362bd-132">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="362bd-133">**Error**</span><span class="sxs-lookup"><span data-stu-id="362bd-133">**Error**</span></span> <br/> | <span data-ttu-id="362bd-134">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="362bd-134">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="362bd-135">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="362bd-135">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="362bd-136">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="362bd-136">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="362bd-137">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="362bd-137">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="362bd-138">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="362bd-138">-  An unknown tag</span></span>  <br/><span data-ttu-id="362bd-139">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="362bd-139">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="362bd-140">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="362bd-140">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="362bd-141">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="362bd-141">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="362bd-142">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="362bd-142">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="362bd-143">子要素</span><span class="sxs-lookup"><span data-stu-id="362bd-143">Child elements</span></span>

|<span data-ttu-id="362bd-144">**Element**</span><span class="sxs-lookup"><span data-stu-id="362bd-144">**Element**</span></span>|<span data-ttu-id="362bd-145">**説明**</span><span class="sxs-lookup"><span data-stu-id="362bd-145">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="362bd-146">会話</span><span class="sxs-lookup"><span data-stu-id="362bd-146">Conversations</span></span>](conversations-ex15websvcsotherref.md) <br/> |<span data-ttu-id="362bd-147">会話の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="362bd-147">Contains an array of conversations.</span></span>  <br/> |
|[<span data-ttu-id="362bd-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="362bd-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="362bd-149">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="362bd-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="362bd-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="362bd-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="362bd-151">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="362bd-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="362bd-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="362bd-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="362bd-153">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="362bd-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="362bd-154">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="362bd-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="362bd-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="362bd-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="362bd-156">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="362bd-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="362bd-157">親要素</span><span class="sxs-lookup"><span data-stu-id="362bd-157">Parent elements</span></span>

<span data-ttu-id="362bd-158">なし。</span><span class="sxs-lookup"><span data-stu-id="362bd-158">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="362bd-159">テキスト値</span><span class="sxs-lookup"><span data-stu-id="362bd-159">Text value</span></span>

<span data-ttu-id="362bd-160">なし。</span><span class="sxs-lookup"><span data-stu-id="362bd-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="362bd-161">注釈</span><span class="sxs-lookup"><span data-stu-id="362bd-161">Remarks</span></span>

<span data-ttu-id="362bd-162">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリにあります。この要素は、Exchange Server 2010 Service Pack 1 (SP1) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="362bd-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.This element was introduced in Exchange Server 2010 Service Pack 1 (SP1).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="362bd-163">要素の情報</span><span class="sxs-lookup"><span data-stu-id="362bd-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="362bd-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="362bd-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="362bd-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="362bd-165">Schema name</span></span>  <br/> |<span data-ttu-id="362bd-166">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="362bd-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="362bd-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="362bd-167">Validation file</span></span>  <br/> |<span data-ttu-id="362bd-168">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="362bd-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="362bd-169">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="362bd-169">Can be empty</span></span>  <br/> |<span data-ttu-id="362bd-170">正しくない</span><span class="sxs-lookup"><span data-stu-id="362bd-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="362bd-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="362bd-171">See also</span></span>

- [<span data-ttu-id="362bd-172">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="362bd-172">FindConversation operation</span></span>](findconversation-operation.md)
- [<span data-ttu-id="362bd-173">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="362bd-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="362bd-174">EWS での会話</span><span class="sxs-lookup"><span data-stu-id="362bd-174">Conversations in EWS</span></span>](https://msdn.microsoft.com/library/91e64629-db6c-4c94-9dcb-d386232e8467%28Office.15%29.aspx)

