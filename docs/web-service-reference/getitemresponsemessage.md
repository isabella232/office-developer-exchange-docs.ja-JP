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
description: GetItemResponseMessage 要素には、1つの GetItem 操作要求の状態と結果が含まれています。
ms.openlocfilehash: bd25a82641259e1546bad6eef5c2f6f8f03e98cb
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458671"
---
# <a name="getitemresponsemessage"></a><span data-ttu-id="b43cc-103">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b43cc-103">GetItemResponseMessage</span></span>

<span data-ttu-id="b43cc-104">**GetItemResponseMessage**要素には、1つの[GetItem 操作](getitem-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b43cc-104">The **GetItemResponseMessage** element contains the status and result of a single [GetItem operation](getitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="b43cc-105">GetItemResponse</span><span class="sxs-lookup"><span data-stu-id="b43cc-105">GetItemResponse</span></span>](getitemresponse.md) 
- [<span data-ttu-id="b43cc-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b43cc-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="b43cc-107">GetItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b43cc-107">GetItemResponseMessage</span></span>](getitemresponsemessage.md)
  
```xml
<GetItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</GetItemResponseMessage>
```

<span data-ttu-id="b43cc-108">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b43cc-108">**ItemInfoResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="b43cc-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="b43cc-109">Attributes and elements</span></span>

<span data-ttu-id="b43cc-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b43cc-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b43cc-111">属性</span><span class="sxs-lookup"><span data-stu-id="b43cc-111">Attributes</span></span>

|<span data-ttu-id="b43cc-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="b43cc-112">**Attribute**</span></span>|<span data-ttu-id="b43cc-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="b43cc-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b43cc-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="b43cc-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="b43cc-115">[GetItem 操作](getitem-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="b43cc-115">Describes the status of a [GetItem operation](getitem-operation.md) response.</span></span> <br/><br/><span data-ttu-id="b43cc-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="b43cc-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="b43cc-117">-成功</span><span class="sxs-lookup"><span data-stu-id="b43cc-117">- Success</span></span><br/><span data-ttu-id="b43cc-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="b43cc-118">- Warning</span></span><br/><span data-ttu-id="b43cc-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="b43cc-119">- Error</span></span> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="b43cc-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="b43cc-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="b43cc-121">**値**</span><span class="sxs-lookup"><span data-stu-id="b43cc-121">**Value**</span></span>|<span data-ttu-id="b43cc-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="b43cc-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b43cc-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="b43cc-123">**Success**</span></span> <br/> |<span data-ttu-id="b43cc-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="b43cc-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="b43cc-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="b43cc-125">**Warning**</span></span> <br/> | <span data-ttu-id="b43cc-126">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="b43cc-126">Describes a request that was not processed.</span></span> <span data-ttu-id="b43cc-127">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="b43cc-127">A warning may be returned if an error occurred while an item in the request was processed and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="b43cc-128">次に、警告のソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="b43cc-128">The following are examples of sources for warnings:</span></span><br/><br/><span data-ttu-id="b43cc-129">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="b43cc-129">- The Exchange store is offline during the batch.</span></span><br/><span data-ttu-id="b43cc-130">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="b43cc-130">- Active Directory Domain Services (AD DS) is offline.</span></span><br/><span data-ttu-id="b43cc-131">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="b43cc-131">- Mailboxes are moved.</span></span><br/><span data-ttu-id="b43cc-132">-MDB がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="b43cc-132">- MDB is offline.</span></span><br/><span data-ttu-id="b43cc-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="b43cc-133">- Password is expired.</span></span>  <br/><span data-ttu-id="b43cc-134">-クォータを超過しました。</span><span class="sxs-lookup"><span data-stu-id="b43cc-134">- Quota is exceeded.</span></span> |
|<span data-ttu-id="b43cc-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="b43cc-135">**Error**</span></span> <br/> | <span data-ttu-id="b43cc-136">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="b43cc-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="b43cc-137">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b43cc-137">The following are examples of sources for errors:</span></span><br/><br/><span data-ttu-id="b43cc-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="b43cc-138">- Invalid attributes or elements</span></span><br/><span data-ttu-id="b43cc-139">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="b43cc-139">- Attributes or elements out of range</span></span><br/><span data-ttu-id="b43cc-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="b43cc-140">- Unknown tag</span></span><br/><span data-ttu-id="b43cc-141">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="b43cc-141">- Attribute or element not valid in the context</span></span><br/><span data-ttu-id="b43cc-142">-クライアントによる権限のないアクセスの試行</span><span class="sxs-lookup"><span data-stu-id="b43cc-142">- Unauthorized access attempted by any client</span></span><br/><span data-ttu-id="b43cc-143">-有効なクライアント側の呼び出しに応答した場合のサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="b43cc-143">- Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="b43cc-144">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="b43cc-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span> |
   
### <a name="child-elements"></a><span data-ttu-id="b43cc-145">子要素</span><span class="sxs-lookup"><span data-stu-id="b43cc-145">Child elements</span></span>

|<span data-ttu-id="b43cc-146">**Element**</span><span class="sxs-lookup"><span data-stu-id="b43cc-146">**Element**</span></span>|<span data-ttu-id="b43cc-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="b43cc-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b43cc-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="b43cc-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b43cc-149">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="b43cc-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b43cc-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b43cc-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b43cc-151">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="b43cc-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="b43cc-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b43cc-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b43cc-153">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="b43cc-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="b43cc-154">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b43cc-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b43cc-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b43cc-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b43cc-156">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="b43cc-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="b43cc-157">Items</span><span class="sxs-lookup"><span data-stu-id="b43cc-157">Items</span></span>](items.md) <br/> |<span data-ttu-id="b43cc-158">返されるアイテムの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="b43cc-158">Contains an array of returned items.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b43cc-159">親要素</span><span class="sxs-lookup"><span data-stu-id="b43cc-159">Parent elements</span></span>

|<span data-ttu-id="b43cc-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="b43cc-160">**Element**</span></span>|<span data-ttu-id="b43cc-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="b43cc-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b43cc-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b43cc-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b43cc-163">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="b43cc-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b43cc-164">注釈</span><span class="sxs-lookup"><span data-stu-id="b43cc-164">Remarks</span></span>

<span data-ttu-id="b43cc-165">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="b43cc-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b43cc-166">要素の情報</span><span class="sxs-lookup"><span data-stu-id="b43cc-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b43cc-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="b43cc-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b43cc-168">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b43cc-168">Schema Name</span></span>  <br/> |<span data-ttu-id="b43cc-169">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="b43cc-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b43cc-170">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b43cc-170">Validation File</span></span>  <br/> |<span data-ttu-id="b43cc-171">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="b43cc-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b43cc-172">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="b43cc-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="b43cc-173">正しくない</span><span class="sxs-lookup"><span data-stu-id="b43cc-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b43cc-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="b43cc-174">See also</span></span>

- [<span data-ttu-id="b43cc-175">GetItem</span><span class="sxs-lookup"><span data-stu-id="b43cc-175">GetItem</span></span>](getitem.md)
- [<span data-ttu-id="b43cc-176">GetItem 操作</span><span class="sxs-lookup"><span data-stu-id="b43cc-176">GetItem operation</span></span>](getitem-operation.md)

