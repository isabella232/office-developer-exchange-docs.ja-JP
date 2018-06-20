---
title: GetInboxRulesResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetInboxRulesResponse
api_type:
- schema
ms.assetid: 6d6c1950-c328-489a-94bf-a250fdbd5cd9
description: GetInboxRulesResponse 要素は、GetInboxRules 操作の要求に対する応答を定義します。
ms.openlocfilehash: d84064ab777fe13ded7727381842ddd1ee9d047d
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760773"
---
# <a name="getinboxrulesresponse"></a><span data-ttu-id="9671d-103">GetInboxRulesResponse</span><span class="sxs-lookup"><span data-stu-id="9671d-103">GetInboxRulesResponse</span></span>

<span data-ttu-id="9671d-104">**GetInboxRulesResponse**要素は、 [GetInboxRules 操作](getinboxrules-operation.md)の要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="9671d-104">The **GetInboxRulesResponse** element defines a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span> 
  
```XML
<GetInboxRulesResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <OutlookRuleBlobExists/>
   <InboxRules/>
</GetInboxRulesResponse>
```

 <span data-ttu-id="9671d-105">**GetInboxRulesResponseType**</span><span class="sxs-lookup"><span data-stu-id="9671d-105">**GetInboxRulesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="9671d-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="9671d-106">Attributes and elements</span></span>

<span data-ttu-id="9671d-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="9671d-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="9671d-108">属性</span><span class="sxs-lookup"><span data-stu-id="9671d-108">Attributes</span></span>

|<span data-ttu-id="9671d-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="9671d-109">**Attribute**</span></span>|<span data-ttu-id="9671d-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="9671d-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9671d-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="9671d-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="9671d-112">[GetInboxRules 操作](getinboxrules-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="9671d-112">Describes the status of a [GetInboxRules operation](getinboxrules-operation.md) response.</span></span> <br/><br/><span data-ttu-id="9671d-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="9671d-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="9671d-114">-成功</span><span class="sxs-lookup"><span data-stu-id="9671d-114">-  Success</span></span>  <br/><span data-ttu-id="9671d-115">-警告</span><span class="sxs-lookup"><span data-stu-id="9671d-115">-  Warning</span></span>  <br/><span data-ttu-id="9671d-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="9671d-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="9671d-117">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="9671d-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="9671d-118">**値**</span><span class="sxs-lookup"><span data-stu-id="9671d-118">**Value**</span></span>|<span data-ttu-id="9671d-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="9671d-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="9671d-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="9671d-120">**Success**</span></span> <br/> |<span data-ttu-id="9671d-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="9671d-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="9671d-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="9671d-122">**Warning**</span></span> <br/> | <span data-ttu-id="9671d-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="9671d-123">Describes a request that was not processed.</span></span> <span data-ttu-id="9671d-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="9671d-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="9671d-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="9671d-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="9671d-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="9671d-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="9671d-127">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="9671d-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="9671d-128">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="9671d-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="9671d-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="9671d-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="9671d-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="9671d-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="9671d-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="9671d-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="9671d-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="9671d-132">**Error**</span></span> <br/> | <span data-ttu-id="9671d-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="9671d-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="9671d-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="9671d-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="9671d-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="9671d-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="9671d-136">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="9671d-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="9671d-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="9671d-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="9671d-138">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="9671d-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="9671d-139">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="9671d-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="9671d-140">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="9671d-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="9671d-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="9671d-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="9671d-142">子要素</span><span class="sxs-lookup"><span data-stu-id="9671d-142">Child elements</span></span>

|<span data-ttu-id="9671d-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="9671d-143">**Element**</span></span>|<span data-ttu-id="9671d-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="9671d-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="9671d-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="9671d-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="9671d-146">応答のステータスの説明テキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="9671d-146">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="9671d-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9671d-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="9671d-148">要求に関するステータス情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="9671d-148">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="9671d-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9671d-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="9671d-150">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="9671d-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="9671d-151">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9671d-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="9671d-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="9671d-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="9671d-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="9671d-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="9671d-154">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="9671d-154">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md) <br/> |<span data-ttu-id="9671d-155">Outlook ルール blob がユーザーのメールボックスに存在するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="9671d-155">Indicates whether a Microsoft Outlook rule blob exists in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="9671d-156">InboxRules</span><span class="sxs-lookup"><span data-stu-id="9671d-156">InboxRules</span></span>](inboxrules.md) <br/> |<span data-ttu-id="9671d-157">ユーザーのメールボックス内の規則の配列を表します。</span><span class="sxs-lookup"><span data-stu-id="9671d-157">Represents an array of the rules in the user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="9671d-158">親要素</span><span class="sxs-lookup"><span data-stu-id="9671d-158">Parent elements</span></span>

<span data-ttu-id="9671d-159">なし。</span><span class="sxs-lookup"><span data-stu-id="9671d-159">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="9671d-160">テキスト値</span><span class="sxs-lookup"><span data-stu-id="9671d-160">Text value</span></span>

<span data-ttu-id="9671d-161">なし。</span><span class="sxs-lookup"><span data-stu-id="9671d-161">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="9671d-162">備考</span><span class="sxs-lookup"><span data-stu-id="9671d-162">Remarks</span></span>

<span data-ttu-id="9671d-163">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="9671d-163">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="9671d-164">要素情報</span><span class="sxs-lookup"><span data-stu-id="9671d-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="9671d-165">名前空間</span><span class="sxs-lookup"><span data-stu-id="9671d-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="9671d-166">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="9671d-166">Schema name</span></span>  <br/> |<span data-ttu-id="9671d-167">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="9671d-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="9671d-168">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="9671d-168">Validation file</span></span>  <br/> |<span data-ttu-id="9671d-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="9671d-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="9671d-170">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="9671d-170">Can be empty</span></span>  <br/> |<span data-ttu-id="9671d-171">False</span><span class="sxs-lookup"><span data-stu-id="9671d-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="9671d-172">関連項目</span><span class="sxs-lookup"><span data-stu-id="9671d-172">See also</span></span>

- [<span data-ttu-id="9671d-173">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="9671d-173">GetInboxRules</span></span>](getinboxrules.md)
- [<span data-ttu-id="9671d-174">GetInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="9671d-174">GetInboxRules operation</span></span>](getinboxrules-operation.md)

