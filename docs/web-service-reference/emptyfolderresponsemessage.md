---
title: EmptyFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 678dd5ce-8d9e-4939-bf1b-a8e148f4f449
description: EmptyFolderResponseMessage 要素には、単一の EmptyFolder 要求の状態と結果が含まれています。
ms.openlocfilehash: fd69df45d7e1d6538a977b79711baa769413ea66
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526215"
---
# <a name="emptyfolderresponsemessage"></a><span data-ttu-id="cb774-103">EmptyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cb774-103">EmptyFolderResponseMessage</span></span>

<span data-ttu-id="cb774-104">**EmptyFolderResponseMessage**要素には、単一の[emptyfolder](emptyfolder.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cb774-104">The **EmptyFolderResponseMessage** element contains the status and result of a single [EmptyFolder](emptyfolder.md) request.</span></span> 
  
```XML
<EmptyFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</EmptyFolderResponseMessage>
```

 <span data-ttu-id="cb774-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="cb774-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="cb774-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="cb774-106">Attributes and elements</span></span>

<span data-ttu-id="cb774-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="cb774-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="cb774-108">属性</span><span class="sxs-lookup"><span data-stu-id="cb774-108">Attributes</span></span>

|<span data-ttu-id="cb774-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="cb774-109">**Attribute**</span></span>|<span data-ttu-id="cb774-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="cb774-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cb774-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="cb774-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="cb774-112">[Emptyfolder 操作](emptyfolder-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="cb774-112">Describes the status of an [EmptyFolder operation](emptyfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="cb774-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="cb774-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="cb774-114">-成功</span><span class="sxs-lookup"><span data-stu-id="cb774-114">-  Success</span></span>  <br/><span data-ttu-id="cb774-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="cb774-115">-  Warning</span></span>  <br/><span data-ttu-id="cb774-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="cb774-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="cb774-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="cb774-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="cb774-118">**値**</span><span class="sxs-lookup"><span data-stu-id="cb774-118">**Value**</span></span>|<span data-ttu-id="cb774-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="cb774-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="cb774-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="cb774-120">**Success**</span></span> <br/> |<span data-ttu-id="cb774-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="cb774-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="cb774-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="cb774-122">**Warning**</span></span> <br/> | <span data-ttu-id="cb774-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="cb774-123">Describes a request that was not processed.</span></span> <span data-ttu-id="cb774-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="cb774-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="cb774-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb774-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="cb774-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="cb774-126">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="cb774-127">-Active Directory ドメインサービス (AD DS) はオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="cb774-127">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="cb774-128">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="cb774-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="cb774-129">-メッセージデータベース (MDB) はオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="cb774-129">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="cb774-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="cb774-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="cb774-131">-クォータが上限を超えています。</span><span class="sxs-lookup"><span data-stu-id="cb774-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="cb774-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="cb774-132">**Error**</span></span> <br/> | <span data-ttu-id="cb774-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="cb774-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="cb774-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="cb774-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="cb774-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="cb774-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="cb774-136">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="cb774-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="cb774-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="cb774-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="cb774-138">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="cb774-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="cb774-139">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="cb774-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="cb774-140">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="cb774-140">-  A server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="cb774-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="cb774-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="cb774-142">子要素</span><span class="sxs-lookup"><span data-stu-id="cb774-142">Child elements</span></span>

|<span data-ttu-id="cb774-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="cb774-143">**Element**</span></span>|<span data-ttu-id="cb774-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="cb774-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb774-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="cb774-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="cb774-146">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="cb774-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="cb774-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cb774-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="cb774-148">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="cb774-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="cb774-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="cb774-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="cb774-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="cb774-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="cb774-151">値0が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cb774-151">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="cb774-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="cb774-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="cb774-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="cb774-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="cb774-154">親要素</span><span class="sxs-lookup"><span data-stu-id="cb774-154">Parent elements</span></span>

|<span data-ttu-id="cb774-155">**要素**</span><span class="sxs-lookup"><span data-stu-id="cb774-155">**Element**</span></span>|<span data-ttu-id="cb774-156">**説明**</span><span class="sxs-lookup"><span data-stu-id="cb774-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="cb774-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cb774-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="cb774-158">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="cb774-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="cb774-159">テキスト値</span><span class="sxs-lookup"><span data-stu-id="cb774-159">Text value</span></span>

<span data-ttu-id="cb774-160">なし。</span><span class="sxs-lookup"><span data-stu-id="cb774-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="cb774-161">注釈</span><span class="sxs-lookup"><span data-stu-id="cb774-161">Remarks</span></span>

<span data-ttu-id="cb774-162">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="cb774-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="cb774-163">要素の情報</span><span class="sxs-lookup"><span data-stu-id="cb774-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="cb774-164">Namespace</span><span class="sxs-lookup"><span data-stu-id="cb774-164">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="cb774-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="cb774-165">Schema Name</span></span>  <br/> |<span data-ttu-id="cb774-166">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="cb774-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="cb774-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="cb774-167">Validation File</span></span>  <br/> |<span data-ttu-id="cb774-168">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="cb774-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="cb774-169">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="cb774-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="cb774-170">正しくない</span><span class="sxs-lookup"><span data-stu-id="cb774-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="cb774-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="cb774-171">See also</span></span>

- [<span data-ttu-id="cb774-172">EmptyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="cb774-172">EmptyFolder operation</span></span>](emptyfolder-operation.md)
- [<span data-ttu-id="cb774-173">Exchange 用 EWS リファレンス</span><span class="sxs-lookup"><span data-stu-id="cb774-173">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="cb774-174">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="cb774-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

