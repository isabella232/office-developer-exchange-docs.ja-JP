---
title: FindItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindItemResponseMessage
api_type:
- schema
ms.assetid: fb2cd399-8a04-4f26-9091-993134ed1d15
description: FindItemResponseMessage 要素には、1つの FindItem 操作要求の状態と結果が含まれています。
ms.openlocfilehash: ca941e0c7e5b9b08f6f495ccae0d634d72b8f429
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462536"
---
# <a name="finditemresponsemessage"></a><span data-ttu-id="cabc5-103">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cabc5-103">FindItemResponseMessage</span></span>

<span data-ttu-id="cabc5-104">**FindItemResponseMessage**要素には、1つの[FindItem 操作](finditem-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cabc5-104">The **FindItemResponseMessage** element contains the status and result of a single [FindItem operation](finditem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="cabc5-105">FindItemResponse</span><span class="sxs-lookup"><span data-stu-id="cabc5-105">FindItemResponse</span></span>](finditemresponse.md) 
- [<span data-ttu-id="cabc5-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cabc5-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="cabc5-107">FindItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cabc5-107">FindItemResponseMessage</span></span>](finditemresponsemessage.md)
  
```xml
<FindItemResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootFolder/>
</FindItemResponseMessage>
```

 <span data-ttu-id="cabc5-108">**FindItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="cabc5-108">**FindItemResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cabc5-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cabc5-109">Attributes and elements</span></span>

<span data-ttu-id="cabc5-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cabc5-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cabc5-111">属性</span><span class="sxs-lookup"><span data-stu-id="cabc5-111">Attributes</span></span>

|<span data-ttu-id="cabc5-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="cabc5-112">**Attribute**</span></span>|<span data-ttu-id="cabc5-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="cabc5-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cabc5-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="cabc5-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="cabc5-115">[FindItem 操作](finditem-operation.md)応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="cabc5-115">Describes the status of a [FindItem operation](finditem-operation.md) response.</span></span><br/><br/> <span data-ttu-id="cabc5-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="cabc5-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="cabc5-117">-成功</span><span class="sxs-lookup"><span data-stu-id="cabc5-117">-  Success</span></span>  <br/><span data-ttu-id="cabc5-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="cabc5-118">-  Warning</span></span>  <br/><span data-ttu-id="cabc5-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="cabc5-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="cabc5-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="cabc5-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="cabc5-121">**値**</span><span class="sxs-lookup"><span data-stu-id="cabc5-121">**Value**</span></span>|<span data-ttu-id="cabc5-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="cabc5-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cabc5-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="cabc5-123">**Success**</span></span> <br/> |<span data-ttu-id="cabc5-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="cabc5-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="cabc5-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="cabc5-125">**Warning**</span></span> <br/> | <span data-ttu-id="cabc5-126">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="cabc5-126">Describes a request that was not processed.</span></span> <span data-ttu-id="cabc5-127">要求内のアイテムの処理中にエラーが発生し、後続のアイテムを処理できなかった場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cabc5-127">A warning may be returned if an error occurred while processing an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="cabc5-128">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cabc5-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="cabc5-129">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="cabc5-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="cabc5-130">-Active Directory ドメインサービス (AD DS) はオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="cabc5-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="cabc5-131">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="cabc5-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="cabc5-132">-メッセージデータベース (MDB) はオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="cabc5-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="cabc5-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="cabc5-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="cabc5-134">-クォータを超過しました。</span><span class="sxs-lookup"><span data-stu-id="cabc5-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="cabc5-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="cabc5-135">**Error**</span></span> <br/> | <span data-ttu-id="cabc5-136">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="cabc5-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="cabc5-137">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cabc5-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="cabc5-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="cabc5-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="cabc5-139">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="cabc5-139">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="cabc5-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="cabc5-140">-  An unknown tag</span></span>  <br/><span data-ttu-id="cabc5-141">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="cabc5-141">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="cabc5-142">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="cabc5-142">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="cabc5-143">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="cabc5-143">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="cabc5-144">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cabc5-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="cabc5-145">子要素</span><span class="sxs-lookup"><span data-stu-id="cabc5-145">Child elements</span></span>

|<span data-ttu-id="cabc5-146">**Element**</span><span class="sxs-lookup"><span data-stu-id="cabc5-146">**Element**</span></span>|<span data-ttu-id="cabc5-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="cabc5-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cabc5-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="cabc5-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="cabc5-149">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="cabc5-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="cabc5-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cabc5-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="cabc5-151">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="cabc5-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="cabc5-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="cabc5-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="cabc5-153">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="cabc5-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="cabc5-154">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cabc5-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="cabc5-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="cabc5-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="cabc5-156">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="cabc5-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="cabc5-157">RootFolder (FindItemResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="cabc5-157">RootFolder (FindItemResponseMessage)</span></span>](rootfolder-finditemresponsemessage.md) <br/> |<span data-ttu-id="cabc5-158">[FindItem 操作](finditem-operation.md)中に1つのルートフォルダの検索結果が含まれます。</span><span class="sxs-lookup"><span data-stu-id="cabc5-158">Contains the results from a search of a single root folder during a [FindItem operation](finditem-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cabc5-159">親要素</span><span class="sxs-lookup"><span data-stu-id="cabc5-159">Parent elements</span></span>

|<span data-ttu-id="cabc5-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="cabc5-160">**Element**</span></span>|<span data-ttu-id="cabc5-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="cabc5-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cabc5-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cabc5-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="cabc5-163">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="cabc5-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="cabc5-164">注釈</span><span class="sxs-lookup"><span data-stu-id="cabc5-164">Remarks</span></span>

<span data-ttu-id="cabc5-165">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="cabc5-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cabc5-166">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cabc5-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cabc5-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="cabc5-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cabc5-168">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cabc5-168">Schema name</span></span>  <br/> |<span data-ttu-id="cabc5-169">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="cabc5-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cabc5-170">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cabc5-170">Validation file</span></span>  <br/> |<span data-ttu-id="cabc5-171">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="cabc5-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cabc5-172">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="cabc5-172">Can be empty</span></span>  <br/> |<span data-ttu-id="cabc5-173">正しくない</span><span class="sxs-lookup"><span data-stu-id="cabc5-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cabc5-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="cabc5-174">See also</span></span>

- <span data-ttu-id="cabc5-175">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="cabc5-175">[FindItem operation](finditem-operation.md)</span></span>
- [<span data-ttu-id="cabc5-176">アイテムの検索</span><span class="sxs-lookup"><span data-stu-id="cabc5-176">Finding Items</span></span>](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

