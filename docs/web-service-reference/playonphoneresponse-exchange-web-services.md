---
title: PlayOnPhoneResponse (Exchange Web サービス)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- PlayOnPhoneResponse
api_type:
- schema
ms.assetid: 578b70d1-dc9d-4bce-b859-0109b2d2bcec
description: PlayOnPhoneResponse 要素は、電話でボイスメールを再生する要求に対する応答を指定します。
ms.openlocfilehash: 907864d7fe669aac99b2ff6d1c5eba71b9ddf79f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459624"
---
# <a name="playonphoneresponse-exchange-web-services"></a><span data-ttu-id="8bea7-103">PlayOnPhoneResponse (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="8bea7-103">PlayOnPhoneResponse (Exchange Web Services)</span></span>

<span data-ttu-id="8bea7-104">**PlayOnPhoneResponse**要素は、電話でボイスメールを再生する要求に対する応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="8bea7-104">The **PlayOnPhoneResponse** element specifies the response to a request to play a voice mail over the telephone.</span></span> 
  
```xml
<PlayOnPhoneResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <PhoneCallId/>
</PlayOnPhoneResponse>
```

 <span data-ttu-id="8bea7-105">**PlayOnPhoneResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="8bea7-105">**PlayOnPhoneResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8bea7-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="8bea7-106">Attributes and elements</span></span>

<span data-ttu-id="8bea7-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8bea7-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8bea7-108">属性</span><span class="sxs-lookup"><span data-stu-id="8bea7-108">Attributes</span></span>

|<span data-ttu-id="8bea7-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="8bea7-109">**Attribute**</span></span>|<span data-ttu-id="8bea7-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="8bea7-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8bea7-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="8bea7-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="8bea7-112">応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="8bea7-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="8bea7-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="8bea7-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="8bea7-114">-成功</span><span class="sxs-lookup"><span data-stu-id="8bea7-114">-  Success</span></span>  <br/><span data-ttu-id="8bea7-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="8bea7-115">-  Warning</span></span>  <br/><span data-ttu-id="8bea7-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="8bea7-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="8bea7-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="8bea7-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="8bea7-118">**値**</span><span class="sxs-lookup"><span data-stu-id="8bea7-118">**Value**</span></span>|<span data-ttu-id="8bea7-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="8bea7-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8bea7-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="8bea7-120">**Success**</span></span> <br/> |<span data-ttu-id="8bea7-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="8bea7-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="8bea7-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="8bea7-122">**Warning**</span></span> <br/> | <span data-ttu-id="8bea7-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="8bea7-123">Describes a request that was not processed.</span></span> <span data-ttu-id="8bea7-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="8bea7-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="8bea7-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8bea7-125">The following are examples of sources of warnings:</span></span> <br/><br/><span data-ttu-id="8bea7-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="8bea7-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="8bea7-127">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="8bea7-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="8bea7-128">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="8bea7-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="8bea7-129">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="8bea7-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="8bea7-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="8bea7-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="8bea7-131">-クォータが限界を超えています。</span><span class="sxs-lookup"><span data-stu-id="8bea7-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="8bea7-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="8bea7-132">**Error**</span></span> <br/> | <span data-ttu-id="8bea7-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="8bea7-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="8bea7-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8bea7-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="8bea7-135">-属性または要素が無効です。</span><span class="sxs-lookup"><span data-stu-id="8bea7-135">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="8bea7-136">-範囲外の属性または要素</span><span class="sxs-lookup"><span data-stu-id="8bea7-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="8bea7-137">-不明なタグ。</span><span class="sxs-lookup"><span data-stu-id="8bea7-137">-  An unknown tag.</span></span>  <br/><span data-ttu-id="8bea7-138">-コンテキスト内で有効ではない属性または要素。</span><span class="sxs-lookup"><span data-stu-id="8bea7-138">-  An attribute or element that is not valid in the context.</span></span>  <br/><span data-ttu-id="8bea7-139">-クライアントによる権限のないアクセス試行。</span><span class="sxs-lookup"><span data-stu-id="8bea7-139">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="8bea7-140">-有効なクライアント側の呼び出しに応答して、サーバー側で障害が発生した。</span><span class="sxs-lookup"><span data-stu-id="8bea7-140">-  A server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="8bea7-141">エラーに関する情報については、「応答[sec」](responsecode.md)および「 [messagetext](messagetext.md)要素」のトピックを参照してください。</span><span class="sxs-lookup"><span data-stu-id="8bea7-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) element topics.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8bea7-142">子要素</span><span class="sxs-lookup"><span data-stu-id="8bea7-142">Child elements</span></span>

|<span data-ttu-id="8bea7-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="8bea7-143">**Element**</span></span>|<span data-ttu-id="8bea7-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="8bea7-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8bea7-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="8bea7-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="8bea7-146">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="8bea7-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="8bea7-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8bea7-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="8bea7-148">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="8bea7-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="8bea7-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8bea7-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="8bea7-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="8bea7-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="8bea7-151">この要素には0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8bea7-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="8bea7-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="8bea7-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="8bea7-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="8bea7-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="8bea7-154">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="8bea7-154">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="8bea7-155">電話の通話識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="8bea7-155">Specifies the telephone call identifier.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8bea7-156">親要素</span><span class="sxs-lookup"><span data-stu-id="8bea7-156">Parent elements</span></span>

<span data-ttu-id="8bea7-157">なし。</span><span class="sxs-lookup"><span data-stu-id="8bea7-157">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="8bea7-158">注釈</span><span class="sxs-lookup"><span data-stu-id="8bea7-158">Remarks</span></span>

<span data-ttu-id="8bea7-159">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="8bea7-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8bea7-160">要素の情報</span><span class="sxs-lookup"><span data-stu-id="8bea7-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8bea7-161">Namespace</span><span class="sxs-lookup"><span data-stu-id="8bea7-161">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8bea7-162">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8bea7-162">Schema Name</span></span>  <br/> |<span data-ttu-id="8bea7-163">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="8bea7-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8bea7-164">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8bea7-164">Validation File</span></span>  <br/> |<span data-ttu-id="8bea7-165">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="8bea7-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8bea7-166">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="8bea7-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="8bea7-167">正しくない</span><span class="sxs-lookup"><span data-stu-id="8bea7-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8bea7-168">関連項目</span><span class="sxs-lookup"><span data-stu-id="8bea7-168">See also</span></span>

- [<span data-ttu-id="8bea7-169">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="8bea7-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

