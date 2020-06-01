---
title: Update受信トレイルールの応答
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateInboxRulesResponse
api_type:
- schema
ms.assetid: 0947b6aa-0d95-421b-aebb-d03021ecc110
description: Update受信トレイの Response 要素は、Update受信トレイルール要求への応答を定義します。
ms.openlocfilehash: 1216a32bdaf2dd5211021add0728844eb62089ed
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455906"
---
# <a name="updateinboxrulesresponse"></a><span data-ttu-id="d597e-103">Update受信トレイルールの応答</span><span class="sxs-lookup"><span data-stu-id="d597e-103">UpdateInboxRulesResponse</span></span>

<span data-ttu-id="d597e-104">**Update受信**トレイの response 要素は、Update受信トレイルール要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="d597e-104">The **UpdateInboxRulesResponse** element defines a response to an UpdateInboxRules request.</span></span> 
  
```XML
<UpdateInboxRulesResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RuleOperationErrors/>
</UpdateInboxRulesResponse>
```

 <span data-ttu-id="d597e-105">**Update受信トレイルール Responsetype**</span><span class="sxs-lookup"><span data-stu-id="d597e-105">**UpdateInboxRulesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d597e-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d597e-106">Attributes and elements</span></span>

<span data-ttu-id="d597e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d597e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d597e-108">属性</span><span class="sxs-lookup"><span data-stu-id="d597e-108">Attributes</span></span>

|<span data-ttu-id="d597e-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="d597e-109">**Attribute**</span></span>|<span data-ttu-id="d597e-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="d597e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d597e-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="d597e-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d597e-112">登録[解除操作](unsubscribe-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="d597e-112">Describes the status of an [Unsubscribe operation](unsubscribe-operation.md) response.</span></span><br/><br/> <span data-ttu-id="d597e-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="d597e-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="d597e-114">-成功</span><span class="sxs-lookup"><span data-stu-id="d597e-114">-  Success</span></span>  <br/><span data-ttu-id="d597e-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="d597e-115">-  Warning</span></span>  <br/><span data-ttu-id="d597e-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="d597e-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d597e-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="d597e-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="d597e-118">**値**</span><span class="sxs-lookup"><span data-stu-id="d597e-118">**Value**</span></span>|<span data-ttu-id="d597e-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="d597e-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d597e-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="d597e-120">**Success**</span></span> <br/> |<span data-ttu-id="d597e-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="d597e-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d597e-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="d597e-122">**Warning**</span></span> <br/> | <span data-ttu-id="d597e-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="d597e-123">Describes a request that was not processed.</span></span> <span data-ttu-id="d597e-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d597e-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="d597e-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d597e-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="d597e-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="d597e-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="d597e-127">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="d597e-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="d597e-128">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="d597e-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="d597e-129">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="d597e-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="d597e-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="d597e-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="d597e-131">-クォータが上限を超えています。</span><span class="sxs-lookup"><span data-stu-id="d597e-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="d597e-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="d597e-132">**Error**</span></span> <br/> | <span data-ttu-id="d597e-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="d597e-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="d597e-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d597e-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="d597e-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="d597e-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d597e-136">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="d597e-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="d597e-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="d597e-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="d597e-138">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="d597e-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="d597e-139">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="d597e-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d597e-140">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="d597e-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="d597e-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d597e-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d597e-142">子要素</span><span class="sxs-lookup"><span data-stu-id="d597e-142">Child elements</span></span>

|<span data-ttu-id="d597e-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="d597e-143">**Element**</span></span>|<span data-ttu-id="d597e-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="d597e-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d597e-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="d597e-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d597e-146">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="d597e-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d597e-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d597e-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d597e-148">要求に関する状態情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="d597e-148">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="d597e-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d597e-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d597e-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="d597e-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="d597e-151">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d597e-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d597e-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d597e-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d597e-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="d597e-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="d597e-154">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="d597e-154">RuleOperationErrors</span></span>](ruleoperationerrors.md) <br/> |<span data-ttu-id="d597e-155">エラーが発生した各ルールフィールドのルール検証エラーの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="d597e-155">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d597e-156">親要素</span><span class="sxs-lookup"><span data-stu-id="d597e-156">Parent elements</span></span>

<span data-ttu-id="d597e-157">なし。</span><span class="sxs-lookup"><span data-stu-id="d597e-157">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="d597e-158">テキスト値</span><span class="sxs-lookup"><span data-stu-id="d597e-158">Text value</span></span>

<span data-ttu-id="d597e-159">なし。</span><span class="sxs-lookup"><span data-stu-id="d597e-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="d597e-160">注釈</span><span class="sxs-lookup"><span data-stu-id="d597e-160">Remarks</span></span>

<span data-ttu-id="d597e-161">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d597e-161">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d597e-162">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d597e-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d597e-163">Namespace</span><span class="sxs-lookup"><span data-stu-id="d597e-163">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d597e-164">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d597e-164">Schema name</span></span>  <br/> |<span data-ttu-id="d597e-165">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d597e-165">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d597e-166">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d597e-166">Validation file</span></span>  <br/> |<span data-ttu-id="d597e-167">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d597e-167">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d597e-168">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="d597e-168">Can be empty</span></span>  <br/> |<span data-ttu-id="d597e-169">正しくない</span><span class="sxs-lookup"><span data-stu-id="d597e-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d597e-170">関連項目</span><span class="sxs-lookup"><span data-stu-id="d597e-170">See also</span></span>

- [<span data-ttu-id="d597e-171">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="d597e-171">UpdateInboxRules</span></span>](updateinboxrules.md)
- [<span data-ttu-id="d597e-172">UpdateInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="d597e-172">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)
- [<span data-ttu-id="d597e-173">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d597e-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

