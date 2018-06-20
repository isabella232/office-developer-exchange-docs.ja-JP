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
description: ExpandDLResponseMessage 要素には、状態および 1 つの ExpandDL 操作要求の結果が含まれています。
ms.openlocfilehash: 62a81574f9c513b905a92876b3d757c635b4f07b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760380"
---
# <a name="expanddlresponsemessage"></a><span data-ttu-id="01bca-103">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="01bca-103">ExpandDLResponseMessage</span></span>

<span data-ttu-id="01bca-104">**ExpandDLResponseMessage**要素には、状態および 1 つの結果が含まれている[ExpandDL の操作](expanddl-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="01bca-104">The **ExpandDLResponseMessage** element contains the status and result of a single [ExpandDL operation](expanddl-operation.md) request.</span></span> 
  
- [<span data-ttu-id="01bca-105">ExpandDLResponse</span><span class="sxs-lookup"><span data-stu-id="01bca-105">ExpandDLResponse</span></span>](expanddlresponse.md)  
- [<span data-ttu-id="01bca-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="01bca-106">ResponseMessages</span></span>](responsemessages.md) 
- [<span data-ttu-id="01bca-107">ExpandDLResponseMessage</span><span class="sxs-lookup"><span data-stu-id="01bca-107">ExpandDLResponseMessage</span></span>](expanddlresponsemessage.md)
  
```xml
<ExpandDLResponseMessage ResponseClass="" IndexedPagingOffset="" NumeratorOffset="" AbsoluteDenominator="" IncludesLastItemInRange="" TotalItemsInView="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <DLExpansion/>
</ExpandDLResponseMessage>
```

<span data-ttu-id="01bca-108">**ExpandDLResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="01bca-108">**ExpandDLResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="01bca-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="01bca-109">Attributes and elements</span></span>

<span data-ttu-id="01bca-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="01bca-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01bca-111">属性</span><span class="sxs-lookup"><span data-stu-id="01bca-111">Attributes</span></span>

|<span data-ttu-id="01bca-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="01bca-112">**Attribute**</span></span>|<span data-ttu-id="01bca-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="01bca-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="01bca-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="01bca-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="01bca-115">[ExpandDL 操作](expanddl-operation.md)応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="01bca-115">Describes the status of an [ExpandDL operation](expanddl-operation.md) response.</span></span><br/><br/><span data-ttu-id="01bca-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="01bca-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="01bca-117">-成功</span><span class="sxs-lookup"><span data-stu-id="01bca-117">-  Success</span></span>  <br/><span data-ttu-id="01bca-118">-警告</span><span class="sxs-lookup"><span data-stu-id="01bca-118">-  Warning</span></span>  <br/><span data-ttu-id="01bca-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="01bca-119">-  Error</span></span>  <br/> |
|<span data-ttu-id="01bca-120">**IndexedPagingOffset**</span><span class="sxs-lookup"><span data-stu-id="01bca-120">**IndexedPagingOffset**</span></span> <br/> |<span data-ttu-id="01bca-121">インデックス付きページング ビューを使用する場合、次の要求に使用する必要があります次のインデックスを表します。</span><span class="sxs-lookup"><span data-stu-id="01bca-121">Represents the next index that should be used for the next request when an indexed paging view is used.</span></span>  <br/> |
|<span data-ttu-id="01bca-122">**NumeratorOffset**</span><span class="sxs-lookup"><span data-stu-id="01bca-122">**NumeratorOffset**</span></span> <br/> |<span data-ttu-id="01bca-123">分数のページ ビューを使用する場合、次の要求に使用する新しい分子の値を表します。</span><span class="sxs-lookup"><span data-stu-id="01bca-123">Represents the new numerator value to use for the next request when fraction page views are used.</span></span>  <br/> |
|<span data-ttu-id="01bca-124">**AbsoluteDenominator**</span><span class="sxs-lookup"><span data-stu-id="01bca-124">**AbsoluteDenominator**</span></span> <br/> |<span data-ttu-id="01bca-125">分数形式のページングを実行する場合、次の要求に使用する分母を表します。</span><span class="sxs-lookup"><span data-stu-id="01bca-125">Represents the next denominator to use for the next request when doing fractional paging.</span></span>  <br/> |
|<span data-ttu-id="01bca-126">**IncludesLastItemInRange**</span><span class="sxs-lookup"><span data-stu-id="01bca-126">**IncludesLastItemInRange**</span></span> <br/> |<span data-ttu-id="01bca-127">追加のページングが必要ないことを示します。</span><span class="sxs-lookup"><span data-stu-id="01bca-127">Indicates that additional paging is not needed.</span></span> <span data-ttu-id="01bca-128">この属性は現在の結果には、クエリの最後の項目が含まれている場合は true になります。</span><span class="sxs-lookup"><span data-stu-id="01bca-128">This attribute will be true if the current results contain the last item in the query.</span></span>  <br/> |
|<span data-ttu-id="01bca-129">**TotalItemsInView**</span><span class="sxs-lookup"><span data-stu-id="01bca-129">**TotalItemsInView**</span></span> <br/> |<span data-ttu-id="01bca-130">制限を満たすアイテムの総数を表します。</span><span class="sxs-lookup"><span data-stu-id="01bca-130">Represents the total number of items that pass the restriction.</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="01bca-131">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="01bca-131">ResponseClass attribute values</span></span>

|<span data-ttu-id="01bca-132">**値**</span><span class="sxs-lookup"><span data-stu-id="01bca-132">**Value**</span></span>|<span data-ttu-id="01bca-133">**説明**</span><span class="sxs-lookup"><span data-stu-id="01bca-133">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="01bca-134">**Success**</span><span class="sxs-lookup"><span data-stu-id="01bca-134">**Success**</span></span> <br/> |<span data-ttu-id="01bca-135">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="01bca-135">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="01bca-136">**Warning**</span><span class="sxs-lookup"><span data-stu-id="01bca-136">**Warning**</span></span> <br/> | <span data-ttu-id="01bca-137">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="01bca-137">Describes a request that was not processed.</span></span> <span data-ttu-id="01bca-138">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="01bca-138">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="01bca-139">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="01bca-139">The following are examples of sources of warnings:</span></span><br/>  <br/><span data-ttu-id="01bca-140">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="01bca-140">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="01bca-141">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="01bca-141">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="01bca-142">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="01bca-142">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="01bca-143">-メールボックス データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="01bca-143">-  The mailbox database (MDB) is offline.</span></span>  <br/><span data-ttu-id="01bca-144">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="01bca-144">-  A password is expired.</span></span>  <br/><span data-ttu-id="01bca-145">クォータを超過しました。</span><span class="sxs-lookup"><span data-stu-id="01bca-145">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="01bca-146">**Error**</span><span class="sxs-lookup"><span data-stu-id="01bca-146">**Error**</span></span> <br/> | <span data-ttu-id="01bca-147">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="01bca-147">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="01bca-148">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="01bca-148">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="01bca-149">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="01bca-149">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="01bca-150">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="01bca-150">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="01bca-151">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="01bca-151">-  An unknown tag</span></span>  <br/><span data-ttu-id="01bca-152">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="01bca-152">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="01bca-153">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="01bca-153">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="01bca-154">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="01bca-154">-  A server-side failure in response to a valid client-side call</span></span> <br/> <br/>  <span data-ttu-id="01bca-155">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="01bca-155">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="01bca-156">子要素</span><span class="sxs-lookup"><span data-stu-id="01bca-156">Child elements</span></span>

|<span data-ttu-id="01bca-157">**要素**</span><span class="sxs-lookup"><span data-stu-id="01bca-157">**Element**</span></span>|<span data-ttu-id="01bca-158">**説明**</span><span class="sxs-lookup"><span data-stu-id="01bca-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01bca-159">MessageText</span><span class="sxs-lookup"><span data-stu-id="01bca-159">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="01bca-160">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="01bca-160">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="01bca-161">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="01bca-161">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="01bca-162">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="01bca-162">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="01bca-163">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="01bca-163">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="01bca-164">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="01bca-164">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="01bca-165">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="01bca-165">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="01bca-166">MessageXml</span><span class="sxs-lookup"><span data-stu-id="01bca-166">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="01bca-167">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="01bca-167">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="01bca-168">DLExpansion</span><span class="sxs-lookup"><span data-stu-id="01bca-168">DLExpansion</span></span>](dlexpansion.md) <br/> |<span data-ttu-id="01bca-169">配布リストに含まれているメールボックスの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="01bca-169">Contains an array of mailboxes that are contained in a distribution list.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="01bca-170">親要素</span><span class="sxs-lookup"><span data-stu-id="01bca-170">Parent elements</span></span>

|<span data-ttu-id="01bca-171">**要素**</span><span class="sxs-lookup"><span data-stu-id="01bca-171">**Element**</span></span>|<span data-ttu-id="01bca-172">**説明**</span><span class="sxs-lookup"><span data-stu-id="01bca-172">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01bca-173">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="01bca-173">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="01bca-174">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="01bca-174">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="01bca-175">備考</span><span class="sxs-lookup"><span data-stu-id="01bca-175">Remarks</span></span>

<span data-ttu-id="01bca-176">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="01bca-176">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01bca-177">要素情報</span><span class="sxs-lookup"><span data-stu-id="01bca-177">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01bca-178">名前空間</span><span class="sxs-lookup"><span data-stu-id="01bca-178">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|<span data-ttu-id="01bca-179">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="01bca-179">Schema Name</span></span>  <br/> |<span data-ttu-id="01bca-180">タイプのスキーマ</span><span class="sxs-lookup"><span data-stu-id="01bca-180">Types schema</span></span>  <br/> |
|<span data-ttu-id="01bca-181">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="01bca-181">Validation File</span></span>  <br/> |<span data-ttu-id="01bca-182">Types.xsd</span><span class="sxs-lookup"><span data-stu-id="01bca-182">Types.xsd</span></span>  <br/> |
|<span data-ttu-id="01bca-183">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="01bca-183">Can be Empty</span></span>  <br/> |<span data-ttu-id="01bca-184">False</span><span class="sxs-lookup"><span data-stu-id="01bca-184">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01bca-185">関連項目</span><span class="sxs-lookup"><span data-stu-id="01bca-185">See also</span></span>

- [<span data-ttu-id="01bca-186">ExpandDL 操作</span><span class="sxs-lookup"><span data-stu-id="01bca-186">ExpandDL operation</span></span>](expanddl-operation.md)
- <span data-ttu-id="01bca-187">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="01bca-187">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>
- [<span data-ttu-id="01bca-188">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="01bca-188">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

