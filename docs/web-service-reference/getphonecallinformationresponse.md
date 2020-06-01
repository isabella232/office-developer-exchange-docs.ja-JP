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
description: GetPhoneCallInformationResponse 要素は、1つの GetPhoneCallInformation 要求に対する応答を定義します。
ms.openlocfilehash: 5bc060504ea734ec2d7e01707ef6bbdb0aa665d3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457887"
---
# <a name="getphonecallinformationresponse"></a><span data-ttu-id="c2819-103">GetPhoneCallInformationResponse</span><span class="sxs-lookup"><span data-stu-id="c2819-103">GetPhoneCallInformationResponse</span></span>

<span data-ttu-id="c2819-104">**GetPhoneCallInformationResponse**要素は、1つの GetPhoneCallInformation 要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="c2819-104">The **GetPhoneCallInformationResponse** element defines a response to a single GetPhoneCallInformation request.</span></span> 
  
```xml
<GetPhoneCallInformationResponse ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>   <PhoneCallInformation/>
</GetPhoneCallInformationResponse>
```

 <span data-ttu-id="c2819-105">**GetPhoneCallInformationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c2819-105">**GetPhoneCallInformationResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c2819-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c2819-106">Attributes and elements</span></span>

<span data-ttu-id="c2819-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c2819-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c2819-108">属性</span><span class="sxs-lookup"><span data-stu-id="c2819-108">Attributes</span></span>

|<span data-ttu-id="c2819-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="c2819-109">**Attribute**</span></span>|<span data-ttu-id="c2819-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2819-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c2819-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="c2819-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="c2819-112">応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="c2819-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="c2819-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="c2819-113">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="c2819-114">-成功</span><span class="sxs-lookup"><span data-stu-id="c2819-114">-  Success</span></span>  <br/><span data-ttu-id="c2819-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="c2819-115">-  Warning</span></span>  <br/><span data-ttu-id="c2819-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="c2819-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="c2819-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="c2819-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="c2819-118">**値**</span><span class="sxs-lookup"><span data-stu-id="c2819-118">**Value**</span></span>|<span data-ttu-id="c2819-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2819-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c2819-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="c2819-120">**Success**</span></span> <br/> |<span data-ttu-id="c2819-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="c2819-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="c2819-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="c2819-122">**Warning**</span></span> <br/> | <span data-ttu-id="c2819-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="c2819-123">Describes a request that was not processed.</span></span> <span data-ttu-id="c2819-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c2819-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="c2819-125">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c2819-125">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="c2819-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="c2819-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="c2819-127">-Active Directory ディレクトリサービスがオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="c2819-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="c2819-128">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="c2819-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="c2819-129">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="c2819-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="c2819-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="c2819-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="c2819-131">-クォータが限界を超えています。</span><span class="sxs-lookup"><span data-stu-id="c2819-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="c2819-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="c2819-132">**Error**</span></span> <br/> | <span data-ttu-id="c2819-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="c2819-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="c2819-134">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c2819-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="c2819-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="c2819-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="c2819-136">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="c2819-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="c2819-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="c2819-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="c2819-138">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="c2819-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="c2819-139">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="c2819-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="c2819-140">-有効なクライアント側の呼び出しに応答した場合のサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="c2819-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="c2819-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c2819-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c2819-142">子要素</span><span class="sxs-lookup"><span data-stu-id="c2819-142">Child elements</span></span>

|<span data-ttu-id="c2819-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="c2819-143">**Element**</span></span>|<span data-ttu-id="c2819-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="c2819-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c2819-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="c2819-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c2819-146">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="c2819-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c2819-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c2819-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c2819-148">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="c2819-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="c2819-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c2819-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c2819-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="c2819-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="c2819-151">この要素には0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c2819-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="c2819-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c2819-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c2819-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="c2819-153">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="c2819-154">PhoneCallInformation</span><span class="sxs-lookup"><span data-stu-id="c2819-154">PhoneCallInformation</span></span>](phonecallinformation.md) <br/> |<span data-ttu-id="c2819-155">通話の状態情報を指定します。</span><span class="sxs-lookup"><span data-stu-id="c2819-155">Specifies the state information for a phone call.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c2819-156">親要素</span><span class="sxs-lookup"><span data-stu-id="c2819-156">Parent elements</span></span>

<span data-ttu-id="c2819-157">なし。</span><span class="sxs-lookup"><span data-stu-id="c2819-157">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="c2819-158">注釈</span><span class="sxs-lookup"><span data-stu-id="c2819-158">Remarks</span></span>

<span data-ttu-id="c2819-159">この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされた Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c2819-159">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c2819-160">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c2819-160">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c2819-161">Namespace</span><span class="sxs-lookup"><span data-stu-id="c2819-161">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c2819-162">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c2819-162">Schema Name</span></span>  <br/> |<span data-ttu-id="c2819-163">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="c2819-163">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c2819-164">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c2819-164">Validation File</span></span>  <br/> |<span data-ttu-id="c2819-165">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c2819-165">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c2819-166">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="c2819-166">Can be Empty</span></span>  <br/> |<span data-ttu-id="c2819-167">正しくない</span><span class="sxs-lookup"><span data-stu-id="c2819-167">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c2819-168">関連項目</span><span class="sxs-lookup"><span data-stu-id="c2819-168">See also</span></span>

- [<span data-ttu-id="c2819-169">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="c2819-169">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

