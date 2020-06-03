---
title: Mailヒント Responsemessagetype
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MailTipsResponseMessageType
api_type:
- schema
ms.assetid: 532cb9d9-1232-4e88-80aa-4cf163eb05da
description: Mailヒント Responsemessagetype 要素は、メールヒントの設定を表します。
ms.openlocfilehash: 5244f26ef927a817a9087c299fd1124acb828aa0
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44454037"
---
# <a name="mailtipsresponsemessagetype"></a><span data-ttu-id="49198-103">Mailヒント Responsemessagetype</span><span class="sxs-lookup"><span data-stu-id="49198-103">MailTipsResponseMessageType</span></span>

<span data-ttu-id="49198-104">**Mailヒント Responsemessagetype**要素は、メールヒントの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="49198-104">The **MailTipsResponseMessageType** element represents mail tips settings.</span></span> 
  
```XML
<MailTipsResponseMessageType ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailTips/>
</MailTipsResponseMessageType>
```

 <span data-ttu-id="49198-105">**Mailヒント Responsemessagetype**</span><span class="sxs-lookup"><span data-stu-id="49198-105">**MailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="49198-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="49198-106">Attributes and elements</span></span>

<span data-ttu-id="49198-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="49198-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="49198-108">属性</span><span class="sxs-lookup"><span data-stu-id="49198-108">Attributes</span></span>

|<span data-ttu-id="49198-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="49198-109">**Attribute**</span></span>|<span data-ttu-id="49198-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="49198-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="49198-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="49198-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="49198-112">応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="49198-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="49198-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="49198-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="49198-114">-成功</span><span class="sxs-lookup"><span data-stu-id="49198-114">-  Success</span></span>  <br/><span data-ttu-id="49198-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="49198-115">-  Warning</span></span>  <br/><span data-ttu-id="49198-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="49198-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="49198-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="49198-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="49198-118">**値**</span><span class="sxs-lookup"><span data-stu-id="49198-118">**Value**</span></span>|<span data-ttu-id="49198-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="49198-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="49198-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="49198-120">**Success**</span></span> <br/> |<span data-ttu-id="49198-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="49198-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="49198-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="49198-122">**Warning**</span></span> <br/> | <span data-ttu-id="49198-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="49198-123">Describes a request that was not processed.</span></span> <span data-ttu-id="49198-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="49198-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="49198-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="49198-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="49198-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="49198-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="49198-127">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="49198-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="49198-128">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="49198-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="49198-129">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="49198-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="49198-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="49198-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="49198-131">-クォータが限界を超えています。</span><span class="sxs-lookup"><span data-stu-id="49198-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="49198-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="49198-132">**Error**</span></span> <br/> | <span data-ttu-id="49198-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="49198-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="49198-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="49198-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="49198-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="49198-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="49198-136">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="49198-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="49198-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="49198-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="49198-138">-コンテキスト内で有効ではない属性または要素</span><span class="sxs-lookup"><span data-stu-id="49198-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="49198-139">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="49198-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="49198-140">-有効なクライアント側の呼び出しに応答した場合のサーバー側障害</span><span class="sxs-lookup"><span data-stu-id="49198-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="49198-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="49198-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="49198-142">子要素</span><span class="sxs-lookup"><span data-stu-id="49198-142">Child elements</span></span>

|<span data-ttu-id="49198-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="49198-143">**Element**</span></span>|<span data-ttu-id="49198-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="49198-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49198-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="49198-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="49198-146">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="49198-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="49198-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="49198-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="49198-148">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="49198-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="49198-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="49198-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="49198-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="49198-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="49198-151">この要素には0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="49198-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="49198-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="49198-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="49198-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="49198-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="49198-154">メールヒント</span><span class="sxs-lookup"><span data-stu-id="49198-154">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="49198-155">さまざまな種類のメールヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="49198-155">Represents values for various types of mail tips.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="49198-156">親要素</span><span class="sxs-lookup"><span data-stu-id="49198-156">Parent elements</span></span>

|<span data-ttu-id="49198-157">**要素**</span><span class="sxs-lookup"><span data-stu-id="49198-157">**Element**</span></span>|<span data-ttu-id="49198-158">**説明**</span><span class="sxs-lookup"><span data-stu-id="49198-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="49198-159">ResponseMessages (Arrayofmailヒント Responsemessages)</span><span class="sxs-lookup"><span data-stu-id="49198-159">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="49198-160">メールヒント応答メッセージのリストを表します。</span><span class="sxs-lookup"><span data-stu-id="49198-160">Represents a list of mail tips response messages.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="49198-161">テキスト値</span><span class="sxs-lookup"><span data-stu-id="49198-161">Text value</span></span>

<span data-ttu-id="49198-162">なし。</span><span class="sxs-lookup"><span data-stu-id="49198-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="49198-163">注釈</span><span class="sxs-lookup"><span data-stu-id="49198-163">Remarks</span></span>

<span data-ttu-id="49198-164">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="49198-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="49198-165">要素の情報</span><span class="sxs-lookup"><span data-stu-id="49198-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="49198-166">Namespace</span><span class="sxs-lookup"><span data-stu-id="49198-166">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="49198-167">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="49198-167">Schema Name</span></span>  <br/> |<span data-ttu-id="49198-168">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="49198-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="49198-169">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="49198-169">Validation File</span></span>  <br/> |<span data-ttu-id="49198-170">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="49198-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="49198-171">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="49198-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="49198-172">正しくない</span><span class="sxs-lookup"><span data-stu-id="49198-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="49198-173">関連項目</span><span class="sxs-lookup"><span data-stu-id="49198-173">See also</span></span>

- [<span data-ttu-id="49198-174">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="49198-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

