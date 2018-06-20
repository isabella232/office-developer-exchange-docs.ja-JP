---
title: UpdateInboxRulesResponse
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
description: UpdateInboxRulesResponse 要素は、UpdateInboxRules 要求への応答を定義します。
ms.openlocfilehash: cd64e4546f8d9bf573062d9c982477be3fa4d925
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839858"
---
# <a name="updateinboxrulesresponse"></a><span data-ttu-id="4e74e-103">UpdateInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="4e74e-103">UpdateInboxRulesResponse</span></span>

<span data-ttu-id="4e74e-104">**UpdateInboxRulesResponse**要素は、UpdateInboxRules 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="4e74e-104">The **UpdateInboxRulesResponse** element defines a response to an UpdateInboxRules request.</span></span> 
  
```XML
<UpdateInboxRulesResponse>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RuleOperationErrors/>
</UpdateInboxRulesResponse>
```

 <span data-ttu-id="4e74e-105">**UpdateInboxRulesResponseType**</span><span class="sxs-lookup"><span data-stu-id="4e74e-105">**UpdateInboxRulesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="4e74e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="4e74e-106">Attributes and elements</span></span>

<span data-ttu-id="4e74e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="4e74e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="4e74e-108">属性</span><span class="sxs-lookup"><span data-stu-id="4e74e-108">Attributes</span></span>

|<span data-ttu-id="4e74e-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="4e74e-109">**Attribute**</span></span>|<span data-ttu-id="4e74e-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="4e74e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4e74e-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="4e74e-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="4e74e-112">[購読の取り消し操作](unsubscribe-operation.md)応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="4e74e-112">Describes the status of an [Unsubscribe operation](unsubscribe-operation.md) response.</span></span><br/><br/> <span data-ttu-id="4e74e-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="4e74e-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="4e74e-114">-成功</span><span class="sxs-lookup"><span data-stu-id="4e74e-114">-  Success</span></span>  <br/><span data-ttu-id="4e74e-115">-警告</span><span class="sxs-lookup"><span data-stu-id="4e74e-115">-  Warning</span></span>  <br/><span data-ttu-id="4e74e-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="4e74e-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="4e74e-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="4e74e-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="4e74e-118">**値**</span><span class="sxs-lookup"><span data-stu-id="4e74e-118">**Value**</span></span>|<span data-ttu-id="4e74e-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="4e74e-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="4e74e-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="4e74e-120">**Success**</span></span> <br/> |<span data-ttu-id="4e74e-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="4e74e-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="4e74e-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="4e74e-122">**Warning**</span></span> <br/> | <span data-ttu-id="4e74e-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="4e74e-123">Describes a request that was not processed.</span></span> <span data-ttu-id="4e74e-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="4e74e-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="4e74e-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4e74e-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="4e74e-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="4e74e-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="4e74e-127">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="4e74e-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="4e74e-128">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="4e74e-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="4e74e-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="4e74e-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="4e74e-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="4e74e-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="4e74e-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="4e74e-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="4e74e-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="4e74e-132">**Error**</span></span> <br/> | <span data-ttu-id="4e74e-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="4e74e-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="4e74e-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="4e74e-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="4e74e-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="4e74e-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="4e74e-136">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="4e74e-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="4e74e-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="4e74e-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="4e74e-138">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="4e74e-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="4e74e-139">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="4e74e-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="4e74e-140">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="4e74e-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="4e74e-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="4e74e-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="4e74e-142">子要素</span><span class="sxs-lookup"><span data-stu-id="4e74e-142">Child elements</span></span>

|<span data-ttu-id="4e74e-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="4e74e-143">**Element**</span></span>|<span data-ttu-id="4e74e-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="4e74e-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="4e74e-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="4e74e-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="4e74e-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="4e74e-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="4e74e-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4e74e-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="4e74e-148">要求に関するステータス情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="4e74e-148">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="4e74e-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="4e74e-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="4e74e-150">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="4e74e-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="4e74e-151">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4e74e-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="4e74e-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="4e74e-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="4e74e-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="4e74e-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="4e74e-154">RuleOperationErrors</span><span class="sxs-lookup"><span data-stu-id="4e74e-154">RuleOperationErrors</span></span>](ruleoperationerrors.md) <br/> |<span data-ttu-id="4e74e-155">エラーが発生したルールの各フィールドの規則の妥当性確認エラーの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="4e74e-155">Represents an array of rule validation errors on each rule field that has an error.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="4e74e-156">親要素</span><span class="sxs-lookup"><span data-stu-id="4e74e-156">Parent elements</span></span>

<span data-ttu-id="4e74e-157">なし。</span><span class="sxs-lookup"><span data-stu-id="4e74e-157">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="4e74e-158">テキスト値</span><span class="sxs-lookup"><span data-stu-id="4e74e-158">Text value</span></span>

<span data-ttu-id="4e74e-159">なし。</span><span class="sxs-lookup"><span data-stu-id="4e74e-159">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="4e74e-160">備考</span><span class="sxs-lookup"><span data-stu-id="4e74e-160">Remarks</span></span>

<span data-ttu-id="4e74e-161">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="4e74e-161">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="4e74e-162">要素情報</span><span class="sxs-lookup"><span data-stu-id="4e74e-162">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="4e74e-163">名前空間</span><span class="sxs-lookup"><span data-stu-id="4e74e-163">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="4e74e-164">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="4e74e-164">Schema name</span></span>  <br/> |<span data-ttu-id="4e74e-165">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="4e74e-165">Messages schema</span></span>  <br/> |
|<span data-ttu-id="4e74e-166">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="4e74e-166">Validation file</span></span>  <br/> |<span data-ttu-id="4e74e-167">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="4e74e-167">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="4e74e-168">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="4e74e-168">Can be empty</span></span>  <br/> |<span data-ttu-id="4e74e-169">False</span><span class="sxs-lookup"><span data-stu-id="4e74e-169">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="4e74e-170">関連項目</span><span class="sxs-lookup"><span data-stu-id="4e74e-170">See also</span></span>

- [<span data-ttu-id="4e74e-171">UpdateInboxRules</span><span class="sxs-lookup"><span data-stu-id="4e74e-171">UpdateInboxRules</span></span>](updateinboxrules.md)
- [<span data-ttu-id="4e74e-172">UpdateInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="4e74e-172">UpdateInboxRules operation</span></span>](updateinboxrules-operation.md)
- [<span data-ttu-id="4e74e-173">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="4e74e-173">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

