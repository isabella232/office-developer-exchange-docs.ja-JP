---
title: ResolveNamesResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResolveNamesResponseMessage
api_type:
- schema
ms.assetid: edcdaf58-ef63-412e-8c58-409213e6ab0d
description: ResolveNamesResponseMessage 要素には、ResolveNames 操作要求の状態と結果が含まれています。
ms.openlocfilehash: 12f32008dbbc603fca7adf26057f1f1904d3cfb2
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455598"
---
# <a name="resolvenamesresponsemessage"></a><span data-ttu-id="0476d-103">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0476d-103">ResolveNamesResponseMessage</span></span>

<span data-ttu-id="0476d-104">**ResolveNamesResponseMessage**要素には、 [ResolveNames 操作](resolvenames-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0476d-104">The **ResolveNamesResponseMessage** element contains the status and result of a [ResolveNames operation](resolvenames-operation.md) request.</span></span> 
  
- [<span data-ttu-id="0476d-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="0476d-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md) 
- [<span data-ttu-id="0476d-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0476d-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="0476d-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="0476d-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
```xml
<ResolveNamesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ResolutionSet/>
</ResolveNamesResponseMessage>
```

 <span data-ttu-id="0476d-108">**ResolveNamesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0476d-108">**ResolveNamesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0476d-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="0476d-109">Attributes and elements</span></span>

<span data-ttu-id="0476d-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0476d-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0476d-111">属性</span><span class="sxs-lookup"><span data-stu-id="0476d-111">Attributes</span></span>

|<span data-ttu-id="0476d-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="0476d-112">**Attribute**</span></span>|<span data-ttu-id="0476d-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="0476d-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0476d-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="0476d-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="0476d-115">[ResolveNames 操作](resolvenames-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="0476d-115">Describes the status of a [ResolveNames operation](resolvenames-operation.md) response.</span></span> <br/><br/><span data-ttu-id="0476d-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="0476d-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="0476d-117">-成功</span><span class="sxs-lookup"><span data-stu-id="0476d-117">-  Success</span></span>  <br/><span data-ttu-id="0476d-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="0476d-118">-  Warning</span></span>  <br/><span data-ttu-id="0476d-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="0476d-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="0476d-120">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="0476d-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="0476d-121">**値**</span><span class="sxs-lookup"><span data-stu-id="0476d-121">**Value**</span></span>|<span data-ttu-id="0476d-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="0476d-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0476d-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="0476d-123">**Success**</span></span> <br/> |<span data-ttu-id="0476d-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="0476d-124">Describes a request that is fulfilled.</span></span> <span data-ttu-id="0476d-125">これは、要求された名前があいまいで、応答に1人の受信者が含まれている場合に発生します。</span><span class="sxs-lookup"><span data-stu-id="0476d-125">This occurs when the requested name is unambiguous and the response contains a single recipient.</span></span>  <br/> |
|<span data-ttu-id="0476d-126">**Warning**</span><span class="sxs-lookup"><span data-stu-id="0476d-126">**Warning**</span></span> <br/> | <span data-ttu-id="0476d-127">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="0476d-127">Describes a request that was not processed.</span></span> <span data-ttu-id="0476d-128">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="0476d-128">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="0476d-129">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0476d-129">The following are example of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="0476d-130">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="0476d-130">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="0476d-131">-Active Directory ドメインサービス (AD DS) はオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="0476d-131">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="0476d-132">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="0476d-132">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="0476d-133">-メールボックスデータベース (MDB) はオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="0476d-133">-  The mailbox database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="0476d-134">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="0476d-134">-  A password is expired.</span></span>  <br/><span data-ttu-id="0476d-135">-クォータが上限を超えています。</span><span class="sxs-lookup"><span data-stu-id="0476d-135">-  A quota is exceeded.</span></span>  <br/><span data-ttu-id="0476d-136">-要求された名前はあいまいで、応答には複数の受信者が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0476d-136">-  The requested name is ambiguous and the response contains multiple recipients.</span></span>  <br/> |
|<span data-ttu-id="0476d-137">**Error**</span><span class="sxs-lookup"><span data-stu-id="0476d-137">**Error**</span></span> <br/> | <span data-ttu-id="0476d-138">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="0476d-138">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="0476d-139">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0476d-139">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="0476d-140">-要求された名前を解決できませんでした。</span><span class="sxs-lookup"><span data-stu-id="0476d-140">-  The requested name could not be resolved.</span></span>  <br/><span data-ttu-id="0476d-141">-属性または要素が無効です。</span><span class="sxs-lookup"><span data-stu-id="0476d-141">-  Attributes or elements are invalid.</span></span>  <br/><span data-ttu-id="0476d-142">-属性または要素が範囲外です。</span><span class="sxs-lookup"><span data-stu-id="0476d-142">-  Attributes or elements are out of range.</span></span>  <br/><span data-ttu-id="0476d-143">-タグが不明です。</span><span class="sxs-lookup"><span data-stu-id="0476d-143">-  A tag is unknown.</span></span>  <br/><span data-ttu-id="0476d-144">-属性または要素がコンテキスト内で有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="0476d-144">-  An attribute or element is not valid in the context.</span></span>  <br/><span data-ttu-id="0476d-145">-クライアントによる権限のないアクセス試行が行われました。</span><span class="sxs-lookup"><span data-stu-id="0476d-145">-  An unauthorized access attempt by any client occurred.</span></span>  <br/><span data-ttu-id="0476d-146">-有効なクライアント側の呼び出しに応答して、サーバー側でエラーが発生しました。</span><span class="sxs-lookup"><span data-stu-id="0476d-146">-  A server-side failure occurred in response to a valid client-side call.</span></span>  <br/>  <br/><span data-ttu-id="0476d-147">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="0476d-147">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0476d-148">子要素</span><span class="sxs-lookup"><span data-stu-id="0476d-148">Child elements</span></span>

|<span data-ttu-id="0476d-149">**Element**</span><span class="sxs-lookup"><span data-stu-id="0476d-149">**Element**</span></span>|<span data-ttu-id="0476d-150">**説明**</span><span class="sxs-lookup"><span data-stu-id="0476d-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0476d-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="0476d-151">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="0476d-152">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="0476d-152">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="0476d-153">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0476d-153">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="0476d-154">要求に関するエラー情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="0476d-154">Provides error information about the request.</span></span>  <br/> |
|[<span data-ttu-id="0476d-155">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0476d-155">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="0476d-156">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="0476d-156">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="0476d-157">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0476d-157">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="0476d-158">MessageXml</span><span class="sxs-lookup"><span data-stu-id="0476d-158">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="0476d-159">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="0476d-159">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="0476d-160">解像度セット</span><span class="sxs-lookup"><span data-stu-id="0476d-160">ResolutionSet</span></span>](resolutionset.md) <br/> |<span data-ttu-id="0476d-161">あいまいな名前の解決方法の配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="0476d-161">Contains an array of resolutions for an ambiguous name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0476d-162">親要素</span><span class="sxs-lookup"><span data-stu-id="0476d-162">Parent elements</span></span>

|<span data-ttu-id="0476d-163">**要素**</span><span class="sxs-lookup"><span data-stu-id="0476d-163">**Element**</span></span>|<span data-ttu-id="0476d-164">**説明**</span><span class="sxs-lookup"><span data-stu-id="0476d-164">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0476d-165">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0476d-165">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0476d-166">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="0476d-166">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0476d-167">注釈</span><span class="sxs-lookup"><span data-stu-id="0476d-167">Remarks</span></span>

<span data-ttu-id="0476d-168">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="0476d-168">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0476d-169">要素の情報</span><span class="sxs-lookup"><span data-stu-id="0476d-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0476d-170">Namespace</span><span class="sxs-lookup"><span data-stu-id="0476d-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0476d-171">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0476d-171">Schema name</span></span>  <br/> |<span data-ttu-id="0476d-172">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="0476d-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0476d-173">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0476d-173">Validation file</span></span>  <br/> |<span data-ttu-id="0476d-174">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="0476d-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0476d-175">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="0476d-175">Can be empty</span></span>  <br/> |<span data-ttu-id="0476d-176">正しくない</span><span class="sxs-lookup"><span data-stu-id="0476d-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0476d-177">関連項目</span><span class="sxs-lookup"><span data-stu-id="0476d-177">See also</span></span>

- [<span data-ttu-id="0476d-178">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="0476d-178">ResolveNames</span></span>](resolvenames.md)
- [<span data-ttu-id="0476d-179">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="0476d-179">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
- [<span data-ttu-id="0476d-180">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="0476d-180">ResolveNames operation</span></span>](resolvenames-operation.md)

