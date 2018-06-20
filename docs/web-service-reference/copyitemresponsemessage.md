---
title: CopyItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyItemResponseMessage
api_type:
- schema
ms.assetid: a43fe442-12c8-44ab-912c-8a226c9bb3e7
description: CopyItemResponseMessage 要素には、状態および 1 つの CopyItem 操作要求の結果が含まれています。
ms.openlocfilehash: 6c1acaff422fd731ca81a3ab244d76a73f3b5c15
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759787"
---
# <a name="copyitemresponsemessage"></a><span data-ttu-id="95a9e-103">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="95a9e-103">CopyItemResponseMessage</span></span>

<span data-ttu-id="95a9e-104">**CopyItemResponseMessage**要素には、状態および 1 つの結果が含まれている[CopyItem の操作](copyitem-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="95a9e-104">The **CopyItemResponseMessage** element contains the status and result of a single [CopyItem operation](copyitem-operation.md) request.</span></span> 
  
```xml
<CopyItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</CopyItemResponseMessage>
```

 <span data-ttu-id="95a9e-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="95a9e-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="95a9e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="95a9e-106">Attributes and elements</span></span>

<span data-ttu-id="95a9e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="95a9e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="95a9e-108">属性</span><span class="sxs-lookup"><span data-stu-id="95a9e-108">Attributes</span></span>

|<span data-ttu-id="95a9e-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="95a9e-109">**Attribute**</span></span>|<span data-ttu-id="95a9e-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="95a9e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="95a9e-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="95a9e-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="95a9e-112">[CopyItem 操作](copyitem-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="95a9e-112">Describes the status of a [CopyItem operation](copyitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="95a9e-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="95a9e-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="95a9e-114">-成功</span><span class="sxs-lookup"><span data-stu-id="95a9e-114">- Success</span></span>  <br/><span data-ttu-id="95a9e-115">-警告</span><span class="sxs-lookup"><span data-stu-id="95a9e-115">-  Warning</span></span>  <br/><span data-ttu-id="95a9e-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="95a9e-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="95a9e-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="95a9e-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="95a9e-118">**値**</span><span class="sxs-lookup"><span data-stu-id="95a9e-118">**Value**</span></span>|<span data-ttu-id="95a9e-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="95a9e-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="95a9e-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="95a9e-120">**Success**</span></span> <br/> |<span data-ttu-id="95a9e-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="95a9e-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="95a9e-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="95a9e-122">**Warning**</span></span> <br/> | <span data-ttu-id="95a9e-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="95a9e-123">Describes a request that was not processed.</span></span> <span data-ttu-id="95a9e-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="95a9e-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="95a9e-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="95a9e-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="95a9e-126">-Exchange ストアは、バッチの中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="95a9e-126">- The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="95a9e-127">-Active Directory ドメイン サービス (AD DS) がオフラインになった。</span><span class="sxs-lookup"><span data-stu-id="95a9e-127">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="95a9e-128">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="95a9e-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="95a9e-129">-メールボックス データベース (MDB) がオフラインになった。</span><span class="sxs-lookup"><span data-stu-id="95a9e-129">-  The mailbox database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="95a9e-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="95a9e-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="95a9e-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="95a9e-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="95a9e-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="95a9e-132">**Error**</span></span> <br/> | <span data-ttu-id="95a9e-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="95a9e-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="95a9e-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="95a9e-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="95a9e-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="95a9e-135">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="95a9e-136">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="95a9e-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="95a9e-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="95a9e-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="95a9e-138">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="95a9e-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="95a9e-139">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="95a9e-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="95a9e-140">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="95a9e-140">-  Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="95a9e-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="95a9e-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="95a9e-142">子要素</span><span class="sxs-lookup"><span data-stu-id="95a9e-142">Child elements</span></span>

|<span data-ttu-id="95a9e-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="95a9e-143">**Element**</span></span>|<span data-ttu-id="95a9e-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="95a9e-144">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="95a9e-145">- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="95a9e-145">- [EWS XML elements in Exchange](ews-xml-elements-in-exchange.md)</span></span> <br/> [<span data-ttu-id="95a9e-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="95a9e-146">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="95a9e-147">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="95a9e-147">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="95a9e-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="95a9e-148">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="95a9e-149">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="95a9e-149">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="95a9e-150">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="95a9e-150">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="95a9e-151">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="95a9e-151">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="95a9e-152">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="95a9e-152">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="95a9e-153">MessageXml</span><span class="sxs-lookup"><span data-stu-id="95a9e-153">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="95a9e-154">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="95a9e-154">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="95a9e-155">Items</span><span class="sxs-lookup"><span data-stu-id="95a9e-155">Items</span></span>](items.md) <br/> |<span data-ttu-id="95a9e-156">コピーした項目の配列が含まれています</span><span class="sxs-lookup"><span data-stu-id="95a9e-156">Contains an array of copied items</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="95a9e-157">親要素</span><span class="sxs-lookup"><span data-stu-id="95a9e-157">Parent elements</span></span>

|<span data-ttu-id="95a9e-158">**要素**</span><span class="sxs-lookup"><span data-stu-id="95a9e-158">**Element**</span></span>|<span data-ttu-id="95a9e-159">**説明**</span><span class="sxs-lookup"><span data-stu-id="95a9e-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="95a9e-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="95a9e-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="95a9e-161">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="95a9e-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="95a9e-162">備考</span><span class="sxs-lookup"><span data-stu-id="95a9e-162">Remarks</span></span>

<span data-ttu-id="95a9e-163">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="95a9e-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="95a9e-164">要素情報</span><span class="sxs-lookup"><span data-stu-id="95a9e-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="95a9e-165">名前空間</span><span class="sxs-lookup"><span data-stu-id="95a9e-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="95a9e-166">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="95a9e-166">Schema name</span></span>  <br/> |<span data-ttu-id="95a9e-167">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="95a9e-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="95a9e-168">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="95a9e-168">Validation file</span></span>  <br/> |<span data-ttu-id="95a9e-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="95a9e-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="95a9e-170">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="95a9e-170">Can be empty</span></span>  <br/> |<span data-ttu-id="95a9e-171">False</span><span class="sxs-lookup"><span data-stu-id="95a9e-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="95a9e-172">関連項目</span><span class="sxs-lookup"><span data-stu-id="95a9e-172">See also</span></span>

- <span data-ttu-id="95a9e-173">
  [CopyItem 操作](copyitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="95a9e-173">[CopyItem operation](copyitem-operation.md)</span></span>
- <span data-ttu-id="95a9e-174">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="95a9e-174">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>

