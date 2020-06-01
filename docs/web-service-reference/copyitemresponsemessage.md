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
description: CopyItemResponseMessage 要素には、1つの CopyItem 操作要求の状態と結果が含まれています。
ms.openlocfilehash: 99449a4c05d0b2ea13dfca4235aa5f40d54d1214
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44466445"
---
# <a name="copyitemresponsemessage"></a><span data-ttu-id="34447-103">CopyItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="34447-103">CopyItemResponseMessage</span></span>

<span data-ttu-id="34447-104">**CopyItemResponseMessage**要素には、1つの[copyitem 操作](copyitem-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="34447-104">The **CopyItemResponseMessage** element contains the status and result of a single [CopyItem operation](copyitem-operation.md) request.</span></span> 
  
```xml
<CopyItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Items/>
</CopyItemResponseMessage>
```

 <span data-ttu-id="34447-105">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="34447-105">**ItemInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="34447-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="34447-106">Attributes and elements</span></span>

<span data-ttu-id="34447-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="34447-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="34447-108">属性</span><span class="sxs-lookup"><span data-stu-id="34447-108">Attributes</span></span>

|<span data-ttu-id="34447-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="34447-109">**Attribute**</span></span>|<span data-ttu-id="34447-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="34447-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="34447-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="34447-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="34447-112">[Copyitem 操作](copyitem-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="34447-112">Describes the status of a [CopyItem operation](copyitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="34447-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="34447-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="34447-114">-成功</span><span class="sxs-lookup"><span data-stu-id="34447-114">- Success</span></span>  <br/><span data-ttu-id="34447-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="34447-115">-  Warning</span></span>  <br/><span data-ttu-id="34447-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="34447-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="34447-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="34447-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="34447-118">**値**</span><span class="sxs-lookup"><span data-stu-id="34447-118">**Value**</span></span>|<span data-ttu-id="34447-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="34447-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="34447-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="34447-120">**Success**</span></span> <br/> |<span data-ttu-id="34447-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="34447-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="34447-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="34447-122">**Warning**</span></span> <br/> | <span data-ttu-id="34447-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="34447-123">Describes a request that was not processed.</span></span> <span data-ttu-id="34447-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="34447-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="34447-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="34447-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="34447-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="34447-126">- The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="34447-127">-Active Directory ドメインサービス (AD DS) はオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="34447-127">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="34447-128">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="34447-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="34447-129">-メールボックスデータベース (MDB) はオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="34447-129">-  The mailbox database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="34447-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="34447-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="34447-131">-クォータが上限を超えています。</span><span class="sxs-lookup"><span data-stu-id="34447-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="34447-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="34447-132">**Error**</span></span> <br/> | <span data-ttu-id="34447-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="34447-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="34447-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="34447-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="34447-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="34447-135">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="34447-136">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="34447-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="34447-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="34447-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="34447-138">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="34447-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="34447-139">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="34447-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="34447-140">-有効なクライアント側の呼び出しに応答した場合のサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="34447-140">-  Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="34447-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="34447-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="34447-142">子要素</span><span class="sxs-lookup"><span data-stu-id="34447-142">Child elements</span></span>

|<span data-ttu-id="34447-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="34447-143">**Element**</span></span>|<span data-ttu-id="34447-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="34447-144">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="34447-145">- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="34447-145">- [EWS XML elements in Exchange](ews-xml-elements-in-exchange.md)</span></span> <br/> [<span data-ttu-id="34447-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="34447-146">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="34447-147">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="34447-147">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="34447-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="34447-148">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="34447-149">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="34447-149">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="34447-150">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="34447-150">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="34447-151">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="34447-151">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="34447-152">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="34447-152">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="34447-153">MessageXml</span><span class="sxs-lookup"><span data-stu-id="34447-153">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="34447-154">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="34447-154">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="34447-155">Items</span><span class="sxs-lookup"><span data-stu-id="34447-155">Items</span></span>](items.md) <br/> |<span data-ttu-id="34447-156">コピーされたアイテムの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="34447-156">Contains an array of copied items</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="34447-157">親要素</span><span class="sxs-lookup"><span data-stu-id="34447-157">Parent elements</span></span>

|<span data-ttu-id="34447-158">**要素**</span><span class="sxs-lookup"><span data-stu-id="34447-158">**Element**</span></span>|<span data-ttu-id="34447-159">**説明**</span><span class="sxs-lookup"><span data-stu-id="34447-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="34447-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="34447-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="34447-161">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="34447-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="34447-162">注釈</span><span class="sxs-lookup"><span data-stu-id="34447-162">Remarks</span></span>

<span data-ttu-id="34447-163">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="34447-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="34447-164">要素の情報</span><span class="sxs-lookup"><span data-stu-id="34447-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="34447-165">Namespace</span><span class="sxs-lookup"><span data-stu-id="34447-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="34447-166">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="34447-166">Schema name</span></span>  <br/> |<span data-ttu-id="34447-167">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="34447-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="34447-168">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="34447-168">Validation file</span></span>  <br/> |<span data-ttu-id="34447-169">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="34447-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="34447-170">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="34447-170">Can be empty</span></span>  <br/> |<span data-ttu-id="34447-171">正しくない</span><span class="sxs-lookup"><span data-stu-id="34447-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="34447-172">関連項目</span><span class="sxs-lookup"><span data-stu-id="34447-172">See also</span></span>

- <span data-ttu-id="34447-173">
  [CopyItem 操作](copyitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="34447-173">[CopyItem operation](copyitem-operation.md)</span></span>
- [<span data-ttu-id="34447-174">Exchange 用 EWS リファレンス</span><span class="sxs-lookup"><span data-stu-id="34447-174">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)

