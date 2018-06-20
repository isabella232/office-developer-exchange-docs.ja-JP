---
title: MailTipsResponseMessageType
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
description: MailTipsResponseMessageType 要素では、メール ヒントの設定を表します。
ms.openlocfilehash: 76a1e33ae189b96a96a41d1bc7a8f79116761c4f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832334"
---
# <a name="mailtipsresponsemessagetype"></a><span data-ttu-id="57762-103">MailTipsResponseMessageType</span><span class="sxs-lookup"><span data-stu-id="57762-103">MailTipsResponseMessageType</span></span>

<span data-ttu-id="57762-104">**MailTipsResponseMessageType**要素では、メール ヒントの設定を表します。</span><span class="sxs-lookup"><span data-stu-id="57762-104">The **MailTipsResponseMessageType** element represents mail tips settings.</span></span> 
  
```XML
<MailTipsResponseMessageType ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <MailTips/>
</MailTipsResponseMessageType>
```

 <span data-ttu-id="57762-105">**MailTipsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="57762-105">**MailTipsResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="57762-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="57762-106">Attributes and elements</span></span>

<span data-ttu-id="57762-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="57762-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="57762-108">属性</span><span class="sxs-lookup"><span data-stu-id="57762-108">Attributes</span></span>

|<span data-ttu-id="57762-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="57762-109">**Attribute**</span></span>|<span data-ttu-id="57762-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="57762-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="57762-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="57762-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="57762-112">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="57762-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="57762-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="57762-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="57762-114">-成功</span><span class="sxs-lookup"><span data-stu-id="57762-114">-  Success</span></span>  <br/><span data-ttu-id="57762-115">-警告</span><span class="sxs-lookup"><span data-stu-id="57762-115">-  Warning</span></span>  <br/><span data-ttu-id="57762-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="57762-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="57762-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="57762-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="57762-118">**値**</span><span class="sxs-lookup"><span data-stu-id="57762-118">**Value**</span></span>|<span data-ttu-id="57762-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="57762-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="57762-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="57762-120">**Success**</span></span> <br/> |<span data-ttu-id="57762-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="57762-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="57762-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="57762-122">**Warning**</span></span> <br/> | <span data-ttu-id="57762-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="57762-123">Describes a request that was not processed.</span></span> <span data-ttu-id="57762-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="57762-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="57762-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="57762-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="57762-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="57762-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="57762-127">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="57762-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="57762-128">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="57762-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="57762-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="57762-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="57762-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="57762-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="57762-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="57762-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="57762-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="57762-132">**Error**</span></span> <br/> | <span data-ttu-id="57762-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="57762-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="57762-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="57762-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="57762-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="57762-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="57762-136">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="57762-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="57762-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="57762-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="57762-138">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="57762-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="57762-139">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="57762-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="57762-140">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="57762-140">-  A server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="57762-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="57762-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="57762-142">子要素</span><span class="sxs-lookup"><span data-stu-id="57762-142">Child elements</span></span>

|<span data-ttu-id="57762-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="57762-143">**Element**</span></span>|<span data-ttu-id="57762-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="57762-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57762-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="57762-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="57762-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="57762-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="57762-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="57762-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="57762-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="57762-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="57762-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="57762-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="57762-150">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="57762-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="57762-151">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="57762-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="57762-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="57762-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="57762-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="57762-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="57762-154">メール ヒント</span><span class="sxs-lookup"><span data-stu-id="57762-154">MailTips</span></span>](mailtips.md) <br/> |<span data-ttu-id="57762-155">さまざまな種類のメール ヒントの値を表します。</span><span class="sxs-lookup"><span data-stu-id="57762-155">Represents values for various types of mail tips.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="57762-156">親要素</span><span class="sxs-lookup"><span data-stu-id="57762-156">Parent elements</span></span>

|<span data-ttu-id="57762-157">**要素**</span><span class="sxs-lookup"><span data-stu-id="57762-157">**Element**</span></span>|<span data-ttu-id="57762-158">**説明**</span><span class="sxs-lookup"><span data-stu-id="57762-158">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="57762-159">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span><span class="sxs-lookup"><span data-stu-id="57762-159">ResponseMessages (ArrayOfMailTipsResponseMessageType)</span></span>](responsemessages-arrayofmailtipsresponsemessagetype.md) <br/> |<span data-ttu-id="57762-160">メール ヒントの応答メッセージの一覧を表します。</span><span class="sxs-lookup"><span data-stu-id="57762-160">Represents a list of mail tips response messages.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="57762-161">テキスト値</span><span class="sxs-lookup"><span data-stu-id="57762-161">Text value</span></span>

<span data-ttu-id="57762-162">なし。</span><span class="sxs-lookup"><span data-stu-id="57762-162">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="57762-163">備考</span><span class="sxs-lookup"><span data-stu-id="57762-163">Remarks</span></span>

<span data-ttu-id="57762-164">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="57762-164">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="57762-165">要素情報</span><span class="sxs-lookup"><span data-stu-id="57762-165">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="57762-166">名前空間</span><span class="sxs-lookup"><span data-stu-id="57762-166">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="57762-167">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="57762-167">Schema Name</span></span>  <br/> |<span data-ttu-id="57762-168">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="57762-168">Messages schema</span></span>  <br/> |
|<span data-ttu-id="57762-169">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="57762-169">Validation File</span></span>  <br/> |<span data-ttu-id="57762-170">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="57762-170">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="57762-171">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="57762-171">Can be Empty</span></span>  <br/> |<span data-ttu-id="57762-172">False</span><span class="sxs-lookup"><span data-stu-id="57762-172">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="57762-173">関連項目</span><span class="sxs-lookup"><span data-stu-id="57762-173">See also</span></span>

- [<span data-ttu-id="57762-174">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="57762-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

