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
description: PlayOnPhoneResponse 要素は、電話でボイス メールを再生するための要求への応答を指定します。
ms.openlocfilehash: 203309bdd6d17b1c78054e673f8a340c2f069b38
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19832831"
---
# <a name="playonphoneresponse-exchange-web-services"></a><span data-ttu-id="f247b-103">PlayOnPhoneResponse (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="f247b-103">PlayOnPhoneResponse (Exchange Web Services)</span></span>

<span data-ttu-id="f247b-104">**PlayOnPhoneResponse**要素は、電話でボイス メールを再生するための要求への応答を指定します。</span><span class="sxs-lookup"><span data-stu-id="f247b-104">The **PlayOnPhoneResponse** element specifies the response to a request to play a voice mail over the telephone.</span></span> 
  
```xml
<PlayOnPhoneResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <PhoneCallId/>
</PlayOnPhoneResponse>
```

 <span data-ttu-id="f247b-105">**PlayOnPhoneResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="f247b-105">**PlayOnPhoneResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="f247b-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="f247b-106">Attributes and elements</span></span>

<span data-ttu-id="f247b-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="f247b-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="f247b-108">属性</span><span class="sxs-lookup"><span data-stu-id="f247b-108">Attributes</span></span>

|<span data-ttu-id="f247b-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="f247b-109">**Attribute**</span></span>|<span data-ttu-id="f247b-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="f247b-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f247b-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="f247b-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="f247b-112">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="f247b-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="f247b-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="f247b-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="f247b-114">-成功</span><span class="sxs-lookup"><span data-stu-id="f247b-114">-  Success</span></span>  <br/><span data-ttu-id="f247b-115">-警告</span><span class="sxs-lookup"><span data-stu-id="f247b-115">-  Warning</span></span>  <br/><span data-ttu-id="f247b-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="f247b-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="f247b-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="f247b-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="f247b-118">**値**</span><span class="sxs-lookup"><span data-stu-id="f247b-118">**Value**</span></span>|<span data-ttu-id="f247b-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="f247b-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="f247b-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="f247b-120">**Success**</span></span> <br/> |<span data-ttu-id="f247b-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="f247b-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="f247b-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="f247b-122">**Warning**</span></span> <br/> | <span data-ttu-id="f247b-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="f247b-123">Describes a request that was not processed.</span></span> <span data-ttu-id="f247b-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="f247b-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="f247b-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f247b-125">The following are examples of sources of warnings:</span></span> <br/><br/><span data-ttu-id="f247b-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="f247b-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="f247b-127">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="f247b-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="f247b-128">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="f247b-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="f247b-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="f247b-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="f247b-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="f247b-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="f247b-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="f247b-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="f247b-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="f247b-132">**Error**</span></span> <br/> | <span data-ttu-id="f247b-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="f247b-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="f247b-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="f247b-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="f247b-135">-無効な属性または要素。</span><span class="sxs-lookup"><span data-stu-id="f247b-135">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="f247b-136">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="f247b-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="f247b-137">-不明なタグです。</span><span class="sxs-lookup"><span data-stu-id="f247b-137">-  An unknown tag.</span></span>  <br/><span data-ttu-id="f247b-138">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="f247b-138">-  An attribute or element that is not valid in the context.</span></span>  <br/><span data-ttu-id="f247b-139">-任意のクライアントで不正なアクセス試行。</span><span class="sxs-lookup"><span data-stu-id="f247b-139">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="f247b-140">-クライアント側の有効な呼び出しへの応答でサーバー側エラーです。</span><span class="sxs-lookup"><span data-stu-id="f247b-140">-  A server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="f247b-141">エラーに関する情報は、 [ResponseCode](responsecode.md)と[メッセージ テキスト](messagetext.md)要素のトピックにあります。</span><span class="sxs-lookup"><span data-stu-id="f247b-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) element topics.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="f247b-142">子要素</span><span class="sxs-lookup"><span data-stu-id="f247b-142">Child elements</span></span>

|<span data-ttu-id="f247b-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="f247b-143">**Element**</span></span>|<span data-ttu-id="f247b-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="f247b-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="f247b-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="f247b-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="f247b-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="f247b-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="f247b-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f247b-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="f247b-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="f247b-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="f247b-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f247b-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="f247b-150">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="f247b-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="f247b-151">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f247b-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="f247b-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="f247b-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="f247b-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="f247b-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="f247b-154">PhoneCallId</span><span class="sxs-lookup"><span data-stu-id="f247b-154">PhoneCallId</span></span>](phonecallid.md) <br/> |<span data-ttu-id="f247b-155">電話の識別子を指定します。</span><span class="sxs-lookup"><span data-stu-id="f247b-155">Specifies the telephone call identifier.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="f247b-156">親要素</span><span class="sxs-lookup"><span data-stu-id="f247b-156">Parent elements</span></span>

<span data-ttu-id="f247b-157">なし。</span><span class="sxs-lookup"><span data-stu-id="f247b-157">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="f247b-158">備考</span><span class="sxs-lookup"><span data-stu-id="f247b-158">Remarks</span></span>

<span data-ttu-id="f247b-159">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="f247b-159">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="f247b-160">要素情報</span><span class="sxs-lookup"><span data-stu-id="f247b-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="f247b-161">名前空間</span><span class="sxs-lookup"><span data-stu-id="f247b-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="f247b-162">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="f247b-162">Schema Name</span></span>  <br/> |<span data-ttu-id="f247b-163">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="f247b-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="f247b-164">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="f247b-164">Validation File</span></span>  <br/> |<span data-ttu-id="f247b-165">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="f247b-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="f247b-166">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="f247b-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="f247b-167">False</span><span class="sxs-lookup"><span data-stu-id="f247b-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="f247b-168">関連項目</span><span class="sxs-lookup"><span data-stu-id="f247b-168">See also</span></span>

- [<span data-ttu-id="f247b-169">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="f247b-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

