---
title: SendItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- SendItemResponseMessage
api_type:
- schema
ms.assetid: 264f6a2f-c8cc-4c96-86e1-1aabb6f9d8ab
description: SendItemResponseMessage 要素には、状態および 1 つの SendItem 操作要求の結果が含まれています。
ms.openlocfilehash: 70355aa2b46303bfceafa2cfe89f1c84896f3158
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833344"
---
# <a name="senditemresponsemessage"></a><span data-ttu-id="7f59c-103">SendItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7f59c-103">SendItemResponseMessage</span></span>

<span data-ttu-id="7f59c-104">**SendItemResponseMessage**要素には、状態および 1 つの結果が含まれています[SendItem 操作](senditem-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="7f59c-104">The **SendItemResponseMessage** element contains the status and result of a single [SendItem operation](senditem-operation.md) request.</span></span> 
  
```xml
<SendItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</SendItemResponseMessage>
```

 <span data-ttu-id="7f59c-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="7f59c-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="7f59c-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="7f59c-106">Attributes and elements</span></span>

<span data-ttu-id="7f59c-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="7f59c-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="7f59c-108">属性</span><span class="sxs-lookup"><span data-stu-id="7f59c-108">Attributes</span></span>

|<span data-ttu-id="7f59c-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="7f59c-109">**Attribute**</span></span>|<span data-ttu-id="7f59c-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="7f59c-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7f59c-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="7f59c-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="7f59c-112">[SendItem 操作](senditem-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7f59c-112">Describes the status of a [SendItem operation](senditem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="7f59c-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="7f59c-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="7f59c-114">-成功</span><span class="sxs-lookup"><span data-stu-id="7f59c-114">-  Success</span></span>  <br/><span data-ttu-id="7f59c-115">-警告</span><span class="sxs-lookup"><span data-stu-id="7f59c-115">-  Warning</span></span>  <br/><span data-ttu-id="7f59c-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="7f59c-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="7f59c-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="7f59c-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="7f59c-118">**値**</span><span class="sxs-lookup"><span data-stu-id="7f59c-118">**Value**</span></span>|<span data-ttu-id="7f59c-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="7f59c-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="7f59c-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="7f59c-120">**Success**</span></span> <br/> |<span data-ttu-id="7f59c-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7f59c-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="7f59c-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="7f59c-122">**Warning**</span></span> <br/> | <span data-ttu-id="7f59c-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7f59c-123">Describes a request that was not processed.</span></span> <span data-ttu-id="7f59c-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="7f59c-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="7f59c-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7f59c-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="7f59c-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="7f59c-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="7f59c-127">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="7f59c-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="7f59c-128">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="7f59c-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="7f59c-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="7f59c-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="7f59c-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="7f59c-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="7f59c-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="7f59c-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="7f59c-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="7f59c-132">**Error**</span></span> <br/> | <span data-ttu-id="7f59c-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="7f59c-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="7f59c-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="7f59c-134">The following are examples of sources of errors:</span></span>  <br/> <br/><span data-ttu-id="7f59c-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="7f59c-135">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="7f59c-136">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="7f59c-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="7f59c-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="7f59c-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="7f59c-138">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="7f59c-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="7f59c-139">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="7f59c-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="7f59c-140">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="7f59c-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="7f59c-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="7f59c-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="7f59c-142">子要素</span><span class="sxs-lookup"><span data-stu-id="7f59c-142">Child elements</span></span>

|<span data-ttu-id="7f59c-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="7f59c-143">**Element**</span></span>|<span data-ttu-id="7f59c-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="7f59c-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7f59c-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="7f59c-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="7f59c-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="7f59c-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="7f59c-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7f59c-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="7f59c-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="7f59c-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="7f59c-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7f59c-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="7f59c-150">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="7f59c-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="7f59c-151">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7f59c-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="7f59c-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="7f59c-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="7f59c-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="7f59c-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="7f59c-154">親要素</span><span class="sxs-lookup"><span data-stu-id="7f59c-154">Parent elements</span></span>

|<span data-ttu-id="7f59c-155">**要素**</span><span class="sxs-lookup"><span data-stu-id="7f59c-155">**Element**</span></span>|<span data-ttu-id="7f59c-156">**説明**</span><span class="sxs-lookup"><span data-stu-id="7f59c-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="7f59c-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7f59c-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="7f59c-158">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="7f59c-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="7f59c-159">備考</span><span class="sxs-lookup"><span data-stu-id="7f59c-159">Remarks</span></span>

<span data-ttu-id="7f59c-160">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="7f59c-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="7f59c-161">要素情報</span><span class="sxs-lookup"><span data-stu-id="7f59c-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="7f59c-162">名前空間</span><span class="sxs-lookup"><span data-stu-id="7f59c-162">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="7f59c-163">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="7f59c-163">Schema Name</span></span>  <br/> |<span data-ttu-id="7f59c-164">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="7f59c-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="7f59c-165">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="7f59c-165">Validation File</span></span>  <br/> |<span data-ttu-id="7f59c-166">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="7f59c-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="7f59c-167">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="7f59c-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="7f59c-168">False</span><span class="sxs-lookup"><span data-stu-id="7f59c-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="7f59c-169">関連項目</span><span class="sxs-lookup"><span data-stu-id="7f59c-169">See also</span></span>

- <span data-ttu-id="7f59c-170">
  [SendItem 操作](senditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="7f59c-170">[SendItem operation](senditem-operation.md)</span></span>
- [<span data-ttu-id="7f59c-171">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="7f59c-171">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

