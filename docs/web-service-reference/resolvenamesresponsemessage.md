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
description: ResolveNamesResponseMessage 要素には、ステータスおよび ResolveNames 操作要求の結果が含まれています。
ms.openlocfilehash: 953a1f0b19c078d969ffe175c22df02b58c5e939
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19833170"
---
# <a name="resolvenamesresponsemessage"></a><span data-ttu-id="b7daf-103">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b7daf-103">ResolveNamesResponseMessage</span></span>

<span data-ttu-id="b7daf-104">**ResolveNamesResponseMessage**要素には、ステータスおよび[ResolveNames 操作](resolvenames-operation.md)要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b7daf-104">The **ResolveNamesResponseMessage** element contains the status and result of a [ResolveNames operation](resolvenames-operation.md) request.</span></span> 
  
- [<span data-ttu-id="b7daf-105">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="b7daf-105">ResolveNamesResponse</span></span>](resolvenamesresponse.md) 
- [<span data-ttu-id="b7daf-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b7daf-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="b7daf-107">ResolveNamesResponseMessage</span><span class="sxs-lookup"><span data-stu-id="b7daf-107">ResolveNamesResponseMessage</span></span>](resolvenamesresponsemessage.md)
  
```xml
<ResolveNamesResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <ResolutionSet/>
</ResolveNamesResponseMessage>
```

 <span data-ttu-id="b7daf-108">**ResolveNamesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="b7daf-108">**ResolveNamesResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="b7daf-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="b7daf-109">Attributes and elements</span></span>

<span data-ttu-id="b7daf-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="b7daf-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="b7daf-111">属性</span><span class="sxs-lookup"><span data-stu-id="b7daf-111">Attributes</span></span>

|<span data-ttu-id="b7daf-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="b7daf-112">**Attribute**</span></span>|<span data-ttu-id="b7daf-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="b7daf-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b7daf-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="b7daf-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="b7daf-115">[ResolveNames 操作](resolvenames-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b7daf-115">Describes the status of a [ResolveNames operation](resolvenames-operation.md) response.</span></span> <br/><br/><span data-ttu-id="b7daf-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="b7daf-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="b7daf-117">-成功</span><span class="sxs-lookup"><span data-stu-id="b7daf-117">-  Success</span></span>  <br/><span data-ttu-id="b7daf-118">-警告</span><span class="sxs-lookup"><span data-stu-id="b7daf-118">-  Warning</span></span>  <br/><span data-ttu-id="b7daf-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="b7daf-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="b7daf-120">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="b7daf-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="b7daf-121">**値**</span><span class="sxs-lookup"><span data-stu-id="b7daf-121">**Value**</span></span>|<span data-ttu-id="b7daf-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="b7daf-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="b7daf-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="b7daf-123">**Success**</span></span> <br/> |<span data-ttu-id="b7daf-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b7daf-124">Describes a request that is fulfilled.</span></span> <span data-ttu-id="b7daf-125">これは、要求された名前があいまいではないと、応答には、1 人の受信者が含まれている場合に発生します。</span><span class="sxs-lookup"><span data-stu-id="b7daf-125">This occurs when the requested name is unambiguous and the response contains a single recipient.</span></span>  <br/> |
|<span data-ttu-id="b7daf-126">**Warning**</span><span class="sxs-lookup"><span data-stu-id="b7daf-126">**Warning**</span></span> <br/> | <span data-ttu-id="b7daf-127">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b7daf-127">Describes a request that was not processed.</span></span> <span data-ttu-id="b7daf-128">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="b7daf-128">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="b7daf-129">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="b7daf-129">The following are example of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="b7daf-130">-Exchange ストアは、バッチの中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="b7daf-130">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="b7daf-131">-Active Directory ドメイン サービス (AD DS) がオフラインになった。</span><span class="sxs-lookup"><span data-stu-id="b7daf-131">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="b7daf-132">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="b7daf-132">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="b7daf-133">-メールボックス データベース (MDB) がオフラインになった。</span><span class="sxs-lookup"><span data-stu-id="b7daf-133">-  The mailbox database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="b7daf-134">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="b7daf-134">-  A password is expired.</span></span>  <br/><span data-ttu-id="b7daf-135">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="b7daf-135">-  A quota is exceeded.</span></span>  <br/><span data-ttu-id="b7daf-136">-要求された名前があいまいであり、応答には、複数の受信者が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b7daf-136">-  The requested name is ambiguous and the response contains multiple recipients.</span></span>  <br/> |
|<span data-ttu-id="b7daf-137">**Error**</span><span class="sxs-lookup"><span data-stu-id="b7daf-137">**Error**</span></span> <br/> | <span data-ttu-id="b7daf-138">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="b7daf-138">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="b7daf-139">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="b7daf-139">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="b7daf-140">-要求された名前を解決できませんでした。</span><span class="sxs-lookup"><span data-stu-id="b7daf-140">-  The requested name could not be resolved.</span></span>  <br/><span data-ttu-id="b7daf-141">-属性の要素が有効ではありませんか。</span><span class="sxs-lookup"><span data-stu-id="b7daf-141">-  Attributes or elements are invalid.</span></span>  <br/><span data-ttu-id="b7daf-142">属性または要素が範囲外です。</span><span class="sxs-lookup"><span data-stu-id="b7daf-142">-  Attributes or elements are out of range.</span></span>  <br/><span data-ttu-id="b7daf-143">-タグは不明です。</span><span class="sxs-lookup"><span data-stu-id="b7daf-143">-  A tag is unknown.</span></span>  <br/><span data-ttu-id="b7daf-144">属性または要素は、コンテキスト内で有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="b7daf-144">-  An attribute or element is not valid in the context.</span></span>  <br/><span data-ttu-id="b7daf-145">-任意のクライアントから不正なアクセス試行が発生しました。</span><span class="sxs-lookup"><span data-stu-id="b7daf-145">-  An unauthorized access attempt by any client occurred.</span></span>  <br/><span data-ttu-id="b7daf-146">が有効なクライアント側の呼び出しに応答、サーバー側の障害が発生しました。</span><span class="sxs-lookup"><span data-stu-id="b7daf-146">-  A server-side failure occurred in response to a valid client-side call.</span></span>  <br/>  <br/><span data-ttu-id="b7daf-147">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="b7daf-147">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="b7daf-148">子要素</span><span class="sxs-lookup"><span data-stu-id="b7daf-148">Child elements</span></span>

|<span data-ttu-id="b7daf-149">**要素**</span><span class="sxs-lookup"><span data-stu-id="b7daf-149">**Element**</span></span>|<span data-ttu-id="b7daf-150">**説明**</span><span class="sxs-lookup"><span data-stu-id="b7daf-150">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7daf-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="b7daf-151">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="b7daf-152">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="b7daf-152">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="b7daf-153">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="b7daf-153">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="b7daf-154">要求に関するエラー情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="b7daf-154">Provides error information about the request.</span></span>  <br/> |
|[<span data-ttu-id="b7daf-155">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="b7daf-155">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="b7daf-156">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="b7daf-156">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="b7daf-157">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b7daf-157">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="b7daf-158">MessageXml</span><span class="sxs-lookup"><span data-stu-id="b7daf-158">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="b7daf-159">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="b7daf-159">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="b7daf-160">ResolutionSet</span><span class="sxs-lookup"><span data-stu-id="b7daf-160">ResolutionSet</span></span>](resolutionset.md) <br/> |<span data-ttu-id="b7daf-161">あいまいな名前の解決策の配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b7daf-161">Contains an array of resolutions for an ambiguous name.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="b7daf-162">親要素</span><span class="sxs-lookup"><span data-stu-id="b7daf-162">Parent elements</span></span>

|<span data-ttu-id="b7daf-163">**要素**</span><span class="sxs-lookup"><span data-stu-id="b7daf-163">**Element**</span></span>|<span data-ttu-id="b7daf-164">**説明**</span><span class="sxs-lookup"><span data-stu-id="b7daf-164">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="b7daf-165">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="b7daf-165">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="b7daf-166">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="b7daf-166">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="b7daf-167">備考</span><span class="sxs-lookup"><span data-stu-id="b7daf-167">Remarks</span></span>

<span data-ttu-id="b7daf-168">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="b7daf-168">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="b7daf-169">要素情報</span><span class="sxs-lookup"><span data-stu-id="b7daf-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="b7daf-170">名前空間</span><span class="sxs-lookup"><span data-stu-id="b7daf-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="b7daf-171">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="b7daf-171">Schema name</span></span>  <br/> |<span data-ttu-id="b7daf-172">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="b7daf-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="b7daf-173">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="b7daf-173">Validation file</span></span>  <br/> |<span data-ttu-id="b7daf-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="b7daf-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="b7daf-175">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="b7daf-175">Can be empty</span></span>  <br/> |<span data-ttu-id="b7daf-176">False</span><span class="sxs-lookup"><span data-stu-id="b7daf-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b7daf-177">関連項目</span><span class="sxs-lookup"><span data-stu-id="b7daf-177">See also</span></span>

- [<span data-ttu-id="b7daf-178">ResolveNames</span><span class="sxs-lookup"><span data-stu-id="b7daf-178">ResolveNames</span></span>](resolvenames.md)
- [<span data-ttu-id="b7daf-179">ResolveNamesResponse</span><span class="sxs-lookup"><span data-stu-id="b7daf-179">ResolveNamesResponse</span></span>](resolvenamesresponse.md)
- [<span data-ttu-id="b7daf-180">ResolveNames 操作</span><span class="sxs-lookup"><span data-stu-id="b7daf-180">ResolveNames operation</span></span>](resolvenames-operation.md)

