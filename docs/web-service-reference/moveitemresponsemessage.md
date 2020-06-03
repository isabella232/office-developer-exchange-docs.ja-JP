---
title: MoveItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveItemResponseMessage
api_type:
- schema
ms.assetid: 1efacb2c-cb76-44ad-b0be-bb47bf2553be
description: MoveItemResponseMessage 要素には、1つの MoveItem 操作要求の状態と結果が含まれています。
ms.openlocfilehash: fd96c34840acd5b6137a2a5d50980dc86202629f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530395"
---
# <a name="moveitemresponsemessage"></a><span data-ttu-id="93ec2-103">MoveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="93ec2-103">MoveItemResponseMessage</span></span>

<span data-ttu-id="93ec2-104">**MoveItemResponseMessage**要素には、1つの[moveitem 操作](moveitem-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="93ec2-104">The **MoveItemResponseMessage** element contains the status and result of a single [MoveItem operation](moveitem-operation.md) request.</span></span> 
  
```xml
<MoveItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</MoveItemResponseMessage>
```

 <span data-ttu-id="93ec2-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="93ec2-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="93ec2-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="93ec2-106">Attributes and elements</span></span>

<span data-ttu-id="93ec2-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="93ec2-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="93ec2-108">属性</span><span class="sxs-lookup"><span data-stu-id="93ec2-108">Attributes</span></span>

|<span data-ttu-id="93ec2-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="93ec2-109">**Attribute**</span></span>|<span data-ttu-id="93ec2-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="93ec2-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="93ec2-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="93ec2-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="93ec2-112">[Moveitem 操作](moveitem-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="93ec2-112">Describes the status of a [MoveItem operation](moveitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="93ec2-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="93ec2-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="93ec2-114">-成功</span><span class="sxs-lookup"><span data-stu-id="93ec2-114">-  Success</span></span>  <br/><span data-ttu-id="93ec2-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="93ec2-115">-  Warning</span></span>  <br/><span data-ttu-id="93ec2-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="93ec2-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="93ec2-117">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="93ec2-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="93ec2-118">**値**</span><span class="sxs-lookup"><span data-stu-id="93ec2-118">**Value**</span></span>|<span data-ttu-id="93ec2-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="93ec2-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="93ec2-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="93ec2-120">**Success**</span></span> <br/> |<span data-ttu-id="93ec2-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="93ec2-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="93ec2-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="93ec2-122">**Warning**</span></span> <br/> | <span data-ttu-id="93ec2-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="93ec2-123">Describes a request that was not processed.</span></span> <span data-ttu-id="93ec2-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="93ec2-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="93ec2-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="93ec2-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="93ec2-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="93ec2-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="93ec2-127">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="93ec2-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="93ec2-128">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="93ec2-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="93ec2-129">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="93ec2-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="93ec2-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="93ec2-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="93ec2-131">-クォータを超過しました。</span><span class="sxs-lookup"><span data-stu-id="93ec2-131">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="93ec2-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="93ec2-132">**Error**</span></span> <br/> | <span data-ttu-id="93ec2-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="93ec2-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="93ec2-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="93ec2-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="93ec2-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="93ec2-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="93ec2-136">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="93ec2-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="93ec2-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="93ec2-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="93ec2-138">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="93ec2-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="93ec2-139">-クライアントによる承認されていないアクセスの試行</span><span class="sxs-lookup"><span data-stu-id="93ec2-139">-  Any unauthorized access attempted by any client</span></span>  <br/><span data-ttu-id="93ec2-140">-有効なクライアント側の呼び出しに応答して、サーバー側で障害が発生した。</span><span class="sxs-lookup"><span data-stu-id="93ec2-140">-  Any server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="93ec2-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="93ec2-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="93ec2-142">子要素</span><span class="sxs-lookup"><span data-stu-id="93ec2-142">Child elements</span></span>

|<span data-ttu-id="93ec2-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="93ec2-143">**Element**</span></span>|<span data-ttu-id="93ec2-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="93ec2-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93ec2-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="93ec2-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="93ec2-146">応答の状態のテキストの説明。</span><span class="sxs-lookup"><span data-stu-id="93ec2-146">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="93ec2-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="93ec2-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="93ec2-148">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="93ec2-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="93ec2-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="93ec2-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="93ec2-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="93ec2-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="93ec2-151">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="93ec2-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="93ec2-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="93ec2-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="93ec2-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="93ec2-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="93ec2-154">Items</span><span class="sxs-lookup"><span data-stu-id="93ec2-154">Items</span></span>](items.md) <br/> |<span data-ttu-id="93ec2-155">移動されたアイテムの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="93ec2-155">Contains an array of moved items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="93ec2-156">親要素</span><span class="sxs-lookup"><span data-stu-id="93ec2-156">Parent elements</span></span>

|<span data-ttu-id="93ec2-157">**要素**</span><span class="sxs-lookup"><span data-stu-id="93ec2-157">**Element**</span></span>|<span data-ttu-id="93ec2-158">**説明**</span><span class="sxs-lookup"><span data-stu-id="93ec2-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="93ec2-159">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="93ec2-159">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="93ec2-160">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="93ec2-160">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="93ec2-161">注釈</span><span class="sxs-lookup"><span data-stu-id="93ec2-161">Remarks</span></span>

<span data-ttu-id="93ec2-162">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされた Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="93ec2-162">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="93ec2-163">要素の情報</span><span class="sxs-lookup"><span data-stu-id="93ec2-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="93ec2-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="93ec2-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="93ec2-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="93ec2-165">Schema Name</span></span>  <br/> |<span data-ttu-id="93ec2-166">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="93ec2-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="93ec2-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="93ec2-167">Validation File</span></span>  <br/> |<span data-ttu-id="93ec2-168">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="93ec2-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="93ec2-169">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="93ec2-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="93ec2-170">正しくない</span><span class="sxs-lookup"><span data-stu-id="93ec2-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="93ec2-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="93ec2-171">See also</span></span>

- [<span data-ttu-id="93ec2-172">MoveItem 操作</span><span class="sxs-lookup"><span data-stu-id="93ec2-172">MoveItem operation</span></span>](moveitem-operation.md)
- [<span data-ttu-id="93ec2-173">MoveItem</span><span class="sxs-lookup"><span data-stu-id="93ec2-173">MoveItem</span></span>](moveitem.md)

