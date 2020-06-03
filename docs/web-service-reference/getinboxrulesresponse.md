---
title: Get受信規則の応答
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
description: Get受信規則の Response 要素は、Get受信トレイの操作要求への応答を定義します。
ms.openlocfilehash: 0d67d7eaf6ffbeeb790249190a98f252dbdb9c87
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458286"
---
# <a name="getinboxrulesresponse"></a><span data-ttu-id="01433-103">Get受信規則の応答</span><span class="sxs-lookup"><span data-stu-id="01433-103">GetInboxRulesResponse</span></span>

<span data-ttu-id="01433-104">**Get受信**規則の response 要素は、 [get受信トレイの操作](getinboxrules-operation.md)要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="01433-104">The **GetInboxRulesResponse** element defines a response to a [GetInboxRules operation](getinboxrules-operation.md) request.</span></span> 
  
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

 <span data-ttu-id="01433-105">**Get受信規則 Responsetype**</span><span class="sxs-lookup"><span data-stu-id="01433-105">**GetInboxRulesResponseType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="01433-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="01433-106">Attributes and elements</span></span>

<span data-ttu-id="01433-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="01433-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="01433-108">属性</span><span class="sxs-lookup"><span data-stu-id="01433-108">Attributes</span></span>

|<span data-ttu-id="01433-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="01433-109">**Attribute**</span></span>|<span data-ttu-id="01433-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="01433-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="01433-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="01433-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="01433-112">[Get受信トレイの操作](getinboxrules-operation.md)応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="01433-112">Describes the status of a [GetInboxRules operation](getinboxrules-operation.md) response.</span></span> <br/><br/><span data-ttu-id="01433-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="01433-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="01433-114">-成功</span><span class="sxs-lookup"><span data-stu-id="01433-114">-  Success</span></span>  <br/><span data-ttu-id="01433-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="01433-115">-  Warning</span></span>  <br/><span data-ttu-id="01433-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="01433-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="01433-117">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="01433-117">ResponseClass Attribute</span></span>

|<span data-ttu-id="01433-118">**値**</span><span class="sxs-lookup"><span data-stu-id="01433-118">**Value**</span></span>|<span data-ttu-id="01433-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="01433-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="01433-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="01433-120">**Success**</span></span> <br/> |<span data-ttu-id="01433-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="01433-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="01433-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="01433-122">**Warning**</span></span> <br/> | <span data-ttu-id="01433-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="01433-123">Describes a request that was not processed.</span></span> <span data-ttu-id="01433-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="01433-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="01433-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="01433-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="01433-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="01433-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="01433-127">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="01433-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="01433-128">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="01433-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="01433-129">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="01433-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="01433-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="01433-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="01433-131">-クォータが上限を超えています。</span><span class="sxs-lookup"><span data-stu-id="01433-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="01433-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="01433-132">**Error**</span></span> <br/> | <span data-ttu-id="01433-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="01433-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="01433-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="01433-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="01433-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="01433-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="01433-136">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="01433-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="01433-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="01433-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="01433-138">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="01433-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="01433-139">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="01433-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="01433-140">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="01433-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="01433-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="01433-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="01433-142">子要素</span><span class="sxs-lookup"><span data-stu-id="01433-142">Child elements</span></span>

|<span data-ttu-id="01433-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="01433-143">**Element**</span></span>|<span data-ttu-id="01433-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="01433-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="01433-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="01433-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="01433-146">応答の状態の説明をテキストで提供します。</span><span class="sxs-lookup"><span data-stu-id="01433-146">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="01433-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="01433-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="01433-148">要求に関する状態情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="01433-148">Provides status information about the request.</span></span>  <br/> |
|[<span data-ttu-id="01433-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="01433-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="01433-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="01433-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="01433-151">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="01433-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="01433-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="01433-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="01433-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="01433-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="01433-154">OutlookRuleBlobExists</span><span class="sxs-lookup"><span data-stu-id="01433-154">OutlookRuleBlobExists</span></span>](outlookruleblobexists.md) <br/> |<span data-ttu-id="01433-155">ユーザーのメールボックスに Microsoft Outlook のルール blob が存在するかどうかを示します。</span><span class="sxs-lookup"><span data-stu-id="01433-155">Indicates whether a Microsoft Outlook rule blob exists in the user's mailbox.</span></span>  <br/> |
|[<span data-ttu-id="01433-156">受信トレイのルール</span><span class="sxs-lookup"><span data-stu-id="01433-156">InboxRules</span></span>](inboxrules.md) <br/> |<span data-ttu-id="01433-157">ユーザーのメールボックス内のルールの配列を表します。</span><span class="sxs-lookup"><span data-stu-id="01433-157">Represents an array of the rules in the user's mailbox.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="01433-158">親要素</span><span class="sxs-lookup"><span data-stu-id="01433-158">Parent elements</span></span>

<span data-ttu-id="01433-159">なし。</span><span class="sxs-lookup"><span data-stu-id="01433-159">None.</span></span>
  
## <a name="text-value"></a><span data-ttu-id="01433-160">テキスト値</span><span class="sxs-lookup"><span data-stu-id="01433-160">Text value</span></span>

<span data-ttu-id="01433-161">なし。</span><span class="sxs-lookup"><span data-stu-id="01433-161">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="01433-162">注釈</span><span class="sxs-lookup"><span data-stu-id="01433-162">Remarks</span></span>

<span data-ttu-id="01433-163">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="01433-163">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="01433-164">要素の情報</span><span class="sxs-lookup"><span data-stu-id="01433-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="01433-165">Namespace</span><span class="sxs-lookup"><span data-stu-id="01433-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="01433-166">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="01433-166">Schema name</span></span>  <br/> |<span data-ttu-id="01433-167">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="01433-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="01433-168">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="01433-168">Validation file</span></span>  <br/> |<span data-ttu-id="01433-169">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="01433-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="01433-170">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="01433-170">Can be empty</span></span>  <br/> |<span data-ttu-id="01433-171">正しくない</span><span class="sxs-lookup"><span data-stu-id="01433-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="01433-172">関連項目</span><span class="sxs-lookup"><span data-stu-id="01433-172">See also</span></span>

- [<span data-ttu-id="01433-173">GetInboxRules</span><span class="sxs-lookup"><span data-stu-id="01433-173">GetInboxRules</span></span>](getinboxrules.md)
- [<span data-ttu-id="01433-174">GetInboxRules の操作</span><span class="sxs-lookup"><span data-stu-id="01433-174">GetInboxRules operation</span></span>](getinboxrules-operation.md)

