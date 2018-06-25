---
title: GetItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetItemResponseMessage
api_type:
- schema
ms.assetid: cc583723-54d1-4a17-8c1f-6586f70fdefd
description: GetItemResponseMessage 要素には、状態および 1 つの GetItem 操作要求の結果が含まれています。
ms.openlocfilehash: 0c8527258d4637ede053e189dfb918b910c859d6
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760784"
---
# <a name="getitemresponsemessage"></a><span data-ttu-id="a6210-103">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a6210-103">GetItemResponseMessage</span></span>

<span data-ttu-id="a6210-104">**GetItemResponseMessage**要素には、状態および 1 つの結果が含まれている[GetItem 操作](getitem-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="a6210-104">The **GetItemResponseMessage** element contains the status and result of a single [GetItem operation](getitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="a6210-105">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="a6210-105">GetItemResponse</span></span>](getitemresponse.md) 
- [<span data-ttu-id="a6210-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a6210-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="a6210-107">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="a6210-107">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
  
```xml
<GetItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</GetItemResponseMessage>
```

<span data-ttu-id="a6210-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="a6210-108">**ItemInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="a6210-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="a6210-109">Attributes and elements</span></span>

<span data-ttu-id="a6210-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="a6210-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="a6210-111">属性</span><span class="sxs-lookup"><span data-stu-id="a6210-111">Attributes</span></span>

|<span data-ttu-id="a6210-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="a6210-112">**Attribute**</span></span>|<span data-ttu-id="a6210-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="a6210-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a6210-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="a6210-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="a6210-115">[GetItem 操作](getitem-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="a6210-115">Describes the status of a [GetItem operation](getitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="a6210-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="a6210-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="a6210-117">-成功</span><span class="sxs-lookup"><span data-stu-id="a6210-117">- Success</span></span><br/><span data-ttu-id="a6210-118">-警告</span><span class="sxs-lookup"><span data-stu-id="a6210-118">- Warning</span></span><br/><span data-ttu-id="a6210-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="a6210-119">- Error</span></span> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="a6210-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="a6210-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="a6210-121">**値**</span><span class="sxs-lookup"><span data-stu-id="a6210-121">**Value**</span></span>|<span data-ttu-id="a6210-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="a6210-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="a6210-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="a6210-123">**Success**</span></span> <br/> |<span data-ttu-id="a6210-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="a6210-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="a6210-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="a6210-125">**Warning**</span></span> <br/> | <span data-ttu-id="a6210-126">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="a6210-126">Describes a request that was not processed.</span></span> <span data-ttu-id="a6210-127">警告は、要求内のアイテムの処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される可能性があります。</span><span class="sxs-lookup"><span data-stu-id="a6210-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="a6210-128">次に、警告のソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="a6210-128">The following are examples of sources for warnings:</span></span><br/><br/><span data-ttu-id="a6210-129">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="a6210-129">- The Exchange store is offline during the batch.</span></span><br/><span data-ttu-id="a6210-130">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="a6210-130">- Active Directory Domain Services (AD DS) is offline.</span></span><br/><span data-ttu-id="a6210-131">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="a6210-131">- Mailboxes are moved.</span></span><br/><span data-ttu-id="a6210-132">MDB では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="a6210-132">- MDB is offline.</span></span><br/><span data-ttu-id="a6210-133">-パスワードは有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="a6210-133">- Password is expired.</span></span>  <br/><span data-ttu-id="a6210-134">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="a6210-134">- Quota is exceeded.</span></span> |
|<span data-ttu-id="a6210-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="a6210-135">**Error**</span></span> <br/> | <span data-ttu-id="a6210-136">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="a6210-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="a6210-137">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="a6210-137">The following are examples of sources for errors:</span></span><br/><br/><span data-ttu-id="a6210-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="a6210-138">- Invalid attributes or elements</span></span><br/><span data-ttu-id="a6210-139">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="a6210-139">- Attributes or elements out of range</span></span><br/><span data-ttu-id="a6210-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="a6210-140">- Unknown tag</span></span><br/><span data-ttu-id="a6210-141">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="a6210-141">- Attribute or element not valid in the context</span></span><br/><span data-ttu-id="a6210-142">-承認されていないアクセスをしようとした任意のクライアント</span><span class="sxs-lookup"><span data-stu-id="a6210-142">- Unauthorized access attempted by any client</span></span><br/><span data-ttu-id="a6210-143">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="a6210-143">- Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="a6210-144">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="a6210-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="a6210-145">子要素</span><span class="sxs-lookup"><span data-stu-id="a6210-145">Child elements</span></span>

|<span data-ttu-id="a6210-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="a6210-146">**Element**</span></span>|<span data-ttu-id="a6210-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="a6210-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a6210-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="a6210-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="a6210-149">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="a6210-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="a6210-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a6210-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="a6210-151">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="a6210-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="a6210-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="a6210-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="a6210-153">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="a6210-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="a6210-154">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a6210-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="a6210-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="a6210-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="a6210-156">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="a6210-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="a6210-157">Items</span><span class="sxs-lookup"><span data-stu-id="a6210-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="a6210-158">返された項目の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a6210-158">Contains an array of returned items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="a6210-159">親要素</span><span class="sxs-lookup"><span data-stu-id="a6210-159">Parent elements</span></span>

|<span data-ttu-id="a6210-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="a6210-160">**Element**</span></span>|<span data-ttu-id="a6210-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="a6210-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="a6210-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="a6210-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="a6210-163">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="a6210-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="a6210-164">備考</span><span class="sxs-lookup"><span data-stu-id="a6210-164">Remarks</span></span>

<span data-ttu-id="a6210-165">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="a6210-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="a6210-166">要素情報</span><span class="sxs-lookup"><span data-stu-id="a6210-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="a6210-167">名前空間</span><span class="sxs-lookup"><span data-stu-id="a6210-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="a6210-168">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="a6210-168">Schema Name</span></span>  <br/> |<span data-ttu-id="a6210-169">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="a6210-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="a6210-170">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="a6210-170">Validation File</span></span>  <br/> |<span data-ttu-id="a6210-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="a6210-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="a6210-172">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="a6210-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="a6210-173">False</span><span class="sxs-lookup"><span data-stu-id="a6210-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="a6210-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="a6210-174">See also</span></span>

- [<span data-ttu-id="a6210-175">GetItem</span><span class="sxs-lookup"><span data-stu-id="a6210-175">GetItem</span></span>](getitem.md)
- <span data-ttu-id="a6210-176">
  [GetItem 操作](getitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="a6210-176">[GetItem operation](getitem-operation.md)</span></span>

