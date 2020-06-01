---
title: ExpandDLResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ExpandDLResponseMessage
api_type:
- schema
ms.assetid: 1140601b-98cf-4cb4-a019-321c7f63d5be
description: ExpandDLResponseMessage 要素には、1つの ExpandDL 操作要求の状態と結果が含まれています。
ms.openlocfilehash: e186c4e14cbb9c922a4d262c85c130b9c33ff939
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44460639"
---
# <a name="expanddlresponsemessage"></a><span data-ttu-id="224a4-103">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="224a4-103">ExpandDLResponseMessage</span></span>

<span data-ttu-id="224a4-104">**ExpandDLResponseMessage**要素には、1つの[expanddl 操作](expanddl-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="224a4-104">The **ExpandDLResponseMessage** element contains the status and result of a single [ExpandDL operation](expanddl-operation.md) request.</span></span> 
  
- [<span data-ttu-id="224a4-105">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="224a4-105">ExpandDLResponse</span></span>](expanddlresponse.md)  
- [<span data-ttu-id="224a4-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="224a4-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="224a4-107">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="224a4-107">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
  
```xml
<ExpandDLResponseMessage ResponseClass="" IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DLExpansion/>
</ExpandDLResponseMessage>
```

<span data-ttu-id="224a4-108">**ExpandDLResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="224a4-108">**ExpandDLResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="224a4-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="224a4-109">Attributes and elements</span></span>

<span data-ttu-id="224a4-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="224a4-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="224a4-111">属性</span><span class="sxs-lookup"><span data-stu-id="224a4-111">Attributes</span></span>

|<span data-ttu-id="224a4-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="224a4-112">**Attribute**</span></span>|<span data-ttu-id="224a4-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="224a4-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="224a4-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="224a4-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="224a4-115">[Expanddl 操作](expanddl-operation.md)応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="224a4-115">Describes the status of an [ExpandDL operation](expanddl-operation.md) response.</span></span><br/><br/><span data-ttu-id="224a4-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="224a4-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="224a4-117">-成功</span><span class="sxs-lookup"><span data-stu-id="224a4-117">-  Success</span></span>  <br/><span data-ttu-id="224a4-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="224a4-118">-  Warning</span></span>  <br/><span data-ttu-id="224a4-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="224a4-119">-  Error</span></span>  <br/> |
|<span data-ttu-id="224a4-120">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="224a4-120">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="224a4-121">インデックス付きページングビューが使用されている場合に、次の要求に使用される次のインデックスを表します。</span><span class="sxs-lookup"><span data-stu-id="224a4-121">Represents the next index that should be used for the next request when an indexed paging view is used.</span></span>  <br/> |
|<span data-ttu-id="224a4-122">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="224a4-122">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="224a4-123">分数ページビューが使用されている場合に、次の要求に対して使用する新しい分子の値を表します。</span><span class="sxs-lookup"><span data-stu-id="224a4-123">Represents the new numerator value to use for the next request when fraction page views are used.</span></span>  <br/> |
|<span data-ttu-id="224a4-124">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="224a4-124">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="224a4-125">分数のページングを行うときに、次の要求に対して使用する次の分母を表します。</span><span class="sxs-lookup"><span data-stu-id="224a4-125">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="224a4-126">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="224a4-126">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="224a4-127">追加のページングを必要としないことを示します。</span><span class="sxs-lookup"><span data-stu-id="224a4-127">Indicates that additional paging is not needed.</span></span> <span data-ttu-id="224a4-128">現在の結果にクエリの最後のアイテムが含まれている場合、この属性は true になります。</span><span class="sxs-lookup"><span data-stu-id="224a4-128">This attribute will be true if the current results contain the last item in the query.</span></span>  <br/> |
|<span data-ttu-id="224a4-129">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="224a4-129">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="224a4-130">制限に合格したアイテムの合計数を表します。</span><span class="sxs-lookup"><span data-stu-id="224a4-130">Represents the total number of items that pass the restriction.</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="224a4-131">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="224a4-131">ResponseClass attribute values</span></span>

|<span data-ttu-id="224a4-132">**値**</span><span class="sxs-lookup"><span data-stu-id="224a4-132">**Value**</span></span>|<span data-ttu-id="224a4-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="224a4-133">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="224a4-134">**Success**</span><span class="sxs-lookup"><span data-stu-id="224a4-134">**Success**</span></span> <br/> |<span data-ttu-id="224a4-135">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="224a4-135">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="224a4-136">**Warning**</span><span class="sxs-lookup"><span data-stu-id="224a4-136">**Warning**</span></span> <br/> | <span data-ttu-id="224a4-137">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="224a4-137">Describes a request that was not processed.</span></span> <span data-ttu-id="224a4-138">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="224a4-138">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="224a4-139">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="224a4-139">The following are examples of sources of warnings:</span></span><br/>  <br/><span data-ttu-id="224a4-140">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="224a4-140">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="224a4-141">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="224a4-141">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="224a4-142">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="224a4-142">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="224a4-143">-メールボックスデータベース (MDB) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="224a4-143">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="224a4-144">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="224a4-144">-  A password is expired.</span></span>  <br/><span data-ttu-id="224a4-145">-クォータを超過しました。</span><span class="sxs-lookup"><span data-stu-id="224a4-145">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="224a4-146">**Error**</span><span class="sxs-lookup"><span data-stu-id="224a4-146">**Error**</span></span> <br/> | <span data-ttu-id="224a4-147">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="224a4-147">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="224a4-148">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="224a4-148">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="224a4-149">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="224a4-149">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="224a4-150">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="224a4-150">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="224a4-151">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="224a4-151">-  An unknown tag</span></span>  <br/><span data-ttu-id="224a4-152">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="224a4-152">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="224a4-153">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="224a4-153">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="224a4-154">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="224a4-154">-  A server-side failure in response to a valid client-side call</span></span> <br/> <br/>  <span data-ttu-id="224a4-155">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="224a4-155">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="224a4-156">子要素</span><span class="sxs-lookup"><span data-stu-id="224a4-156">Child elements</span></span>

|<span data-ttu-id="224a4-157">**Element**</span><span class="sxs-lookup"><span data-stu-id="224a4-157">**Element**</span></span>|<span data-ttu-id="224a4-158">**説明**</span><span class="sxs-lookup"><span data-stu-id="224a4-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="224a4-159">MessageText</span><span class="sxs-lookup"><span data-stu-id="224a4-159">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="224a4-160">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="224a4-160">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="224a4-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="224a4-161">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="224a4-162">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="224a4-162">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="224a4-163">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="224a4-163">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="224a4-164">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="224a4-164">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="224a4-165">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="224a4-165">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="224a4-166">MessageXml</span><span class="sxs-lookup"><span data-stu-id="224a4-166">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="224a4-167">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="224a4-167">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="224a4-168">DLExpansion 展開</span><span class="sxs-lookup"><span data-stu-id="224a4-168">DLExpansion</span></span>](dlexpansion.md) <br/> |<span data-ttu-id="224a4-169">配布リストに含まれているメールボックスの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="224a4-169">Contains an array of mailboxes that are contained in a distribution list.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="224a4-170">親要素</span><span class="sxs-lookup"><span data-stu-id="224a4-170">Parent elements</span></span>

|<span data-ttu-id="224a4-171">**要素**</span><span class="sxs-lookup"><span data-stu-id="224a4-171">**Element**</span></span>|<span data-ttu-id="224a4-172">**説明**</span><span class="sxs-lookup"><span data-stu-id="224a4-172">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="224a4-173">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="224a4-173">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="224a4-174">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="224a4-174">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="224a4-175">注釈</span><span class="sxs-lookup"><span data-stu-id="224a4-175">Remarks</span></span>

<span data-ttu-id="224a4-176">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされた Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="224a4-176">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="224a4-177">要素の情報</span><span class="sxs-lookup"><span data-stu-id="224a4-177">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="224a4-178">Namespace</span><span class="sxs-lookup"><span data-stu-id="224a4-178">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="224a4-179">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="224a4-179">Schema Name</span></span>  <br/> |<span data-ttu-id="224a4-180">Types スキーマ</span><span class="sxs-lookup"><span data-stu-id="224a4-180">Types schema</span></span>  <br/> |
|<span data-ttu-id="224a4-181">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="224a4-181">Validation File</span></span>  <br/> |<span data-ttu-id="224a4-182">型 .xsd</span><span class="sxs-lookup"><span data-stu-id="224a4-182">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="224a4-183">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="224a4-183">Can be Empty</span></span>  <br/> |<span data-ttu-id="224a4-184">正しくない</span><span class="sxs-lookup"><span data-stu-id="224a4-184">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="224a4-185">関連項目</span><span class="sxs-lookup"><span data-stu-id="224a4-185">See also</span></span>

- [<span data-ttu-id="224a4-186">ExpandDL 操作</span><span class="sxs-lookup"><span data-stu-id="224a4-186">ExpandDL operation</span></span>](expanddl-operation.md)
- <span data-ttu-id="224a4-187">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="224a4-187">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>
- [<span data-ttu-id="224a4-188">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="224a4-188">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

