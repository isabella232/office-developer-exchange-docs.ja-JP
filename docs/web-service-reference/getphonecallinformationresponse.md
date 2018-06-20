---
title: GetPhoneCallInformationResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetPhoneCallInformationResponse
api_type:
- schema
ms.assetid: 17f79875-46ec-4289-b974-b3c35af429cd
description: GetPhoneCallInformationResponse 要素は、1 つの GetPhoneCallInformation 要求への応答を定義します。
ms.openlocfilehash: 5a03d63198cd00997b8975b18a5ae0eb5fca1af2
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760837"
---
# <a name="getphonecallinformationresponse"></a><span data-ttu-id="e4f2f-103">GetPhoneCallInformationResponse</span><span class="sxs-lookup"><span data-stu-id="e4f2f-103">GetPhoneCallInformationResponse</span></span>

<span data-ttu-id="e4f2f-104">**GetPhoneCallInformationResponse**要素は、1 つの GetPhoneCallInformation 要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-104">The **GetPhoneCallInformationResponse** element defines a response to a single GetPhoneCallInformation request.</span></span> 
  
```xml
<GetPhoneCallInformationResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <PhoneCallInformation/>
</GetPhoneCallInformationResponse>
```

 <span data-ttu-id="e4f2f-105">**GetPhoneCallInformationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-105">**GetPhoneCallInformationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="e4f2f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="e4f2f-106">Attributes and elements</span></span>

<span data-ttu-id="e4f2f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="e4f2f-108">属性</span><span class="sxs-lookup"><span data-stu-id="e4f2f-108">Attributes</span></span>

|<span data-ttu-id="e4f2f-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-109">**Attribute**</span></span>|<span data-ttu-id="e4f2f-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e4f2f-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="e4f2f-112">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="e4f2f-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="e4f2f-114">-成功</span><span class="sxs-lookup"><span data-stu-id="e4f2f-114">-  Success</span></span>  <br/><span data-ttu-id="e4f2f-115">-警告</span><span class="sxs-lookup"><span data-stu-id="e4f2f-115">-  Warning</span></span>  <br/><span data-ttu-id="e4f2f-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="e4f2f-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="e4f2f-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="e4f2f-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="e4f2f-118">**値**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-118">**Value**</span></span>|<span data-ttu-id="e4f2f-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="e4f2f-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-120">**Success**</span></span> <br/> |<span data-ttu-id="e4f2f-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="e4f2f-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-122">**Warning**</span></span> <br/> | <span data-ttu-id="e4f2f-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-123">Describes a request that was not processed.</span></span> <span data-ttu-id="e4f2f-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="e4f2f-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="e4f2f-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="e4f2f-127">-Active Directory ディレクトリ サービスは、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="e4f2f-128">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="e4f2f-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="e4f2f-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="e4f2f-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="e4f2f-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-132">**Error**</span></span> <br/> | <span data-ttu-id="e4f2f-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="e4f2f-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="e4f2f-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="e4f2f-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="e4f2f-136">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="e4f2f-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="e4f2f-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="e4f2f-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="e4f2f-138">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="e4f2f-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="e4f2f-139">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="e4f2f-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="e4f2f-140">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="e4f2f-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="e4f2f-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="e4f2f-142">子要素</span><span class="sxs-lookup"><span data-stu-id="e4f2f-142">Child elements</span></span>

|<span data-ttu-id="e4f2f-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-143">**Element**</span></span>|<span data-ttu-id="e4f2f-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="e4f2f-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="e4f2f-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="e4f2f-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="e4f2f-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="e4f2f-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e4f2f-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="e4f2f-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="e4f2f-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e4f2f-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="e4f2f-150">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="e4f2f-151">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="e4f2f-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="e4f2f-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="e4f2f-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="e4f2f-154">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="e4f2f-154">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="e4f2f-155">電話の状態情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-155">Specifies the state information for a phone call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="e4f2f-156">親要素</span><span class="sxs-lookup"><span data-stu-id="e4f2f-156">Parent elements</span></span>

<span data-ttu-id="e4f2f-157">なし。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-157">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="e4f2f-158">備考</span><span class="sxs-lookup"><span data-stu-id="e4f2f-158">Remarks</span></span>

<span data-ttu-id="e4f2f-159">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="e4f2f-159">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="e4f2f-160">要素情報</span><span class="sxs-lookup"><span data-stu-id="e4f2f-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="e4f2f-161">名前空間</span><span class="sxs-lookup"><span data-stu-id="e4f2f-161">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="e4f2f-162">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="e4f2f-162">Schema Name</span></span>  <br/> |<span data-ttu-id="e4f2f-163">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="e4f2f-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="e4f2f-164">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="e4f2f-164">Validation File</span></span>  <br/> |<span data-ttu-id="e4f2f-165">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="e4f2f-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="e4f2f-166">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="e4f2f-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="e4f2f-167">False</span><span class="sxs-lookup"><span data-stu-id="e4f2f-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="e4f2f-168">関連項目</span><span class="sxs-lookup"><span data-stu-id="e4f2f-168">See also</span></span>

- [<span data-ttu-id="e4f2f-169">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="e4f2f-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

