---
title: CreateUserConfigurationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CreateUserConfigurationResponseMessage
api_type:
- schema
ms.assetid: 9c11427c-74c9-4c6a-a0e7-7d5556670c1e
description: CreateUserConfigurationResponseMessage 要素には、状態および 1 つの CreateUserConfiguration 要求の結果が含まれています。
ms.openlocfilehash: 718d62d9f5b920eaf9481054b095958a9f44cbf8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759876"
---
# <a name="createuserconfigurationresponsemessage"></a><span data-ttu-id="1e04e-103">CreateUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="1e04e-103">CreateUserConfigurationResponseMessage</span></span>

<span data-ttu-id="1e04e-104">**CreateUserConfigurationResponseMessage**要素には、状態および 1 つの**CreateUserConfiguration**要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1e04e-104">The **CreateUserConfigurationResponseMessage** element contains the status and result of a single **CreateUserConfiguration** request.</span></span> 
  
```xml
<CreateUserConfigurationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</CreateUserConfigurationResponseMessage>
```

<span data-ttu-id="1e04e-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="1e04e-105">**ResponseMessageType**</span></span>

## <a name="attributes-and-elements"></a><span data-ttu-id="1e04e-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="1e04e-106">Attributes and elements</span></span>

<span data-ttu-id="1e04e-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="1e04e-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="1e04e-108">属性</span><span class="sxs-lookup"><span data-stu-id="1e04e-108">Attributes</span></span>

|<span data-ttu-id="1e04e-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="1e04e-109">**Attribute**</span></span>|<span data-ttu-id="1e04e-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="1e04e-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1e04e-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="1e04e-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="1e04e-112">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1e04e-112">Describes the status of the response.</span></span><br/><br/><span data-ttu-id="1e04e-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="1e04e-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="1e04e-114">-成功</span><span class="sxs-lookup"><span data-stu-id="1e04e-114">-  Success</span></span>  <br/><span data-ttu-id="1e04e-115">-警告</span><span class="sxs-lookup"><span data-stu-id="1e04e-115">-  Warning</span></span>  <br/><span data-ttu-id="1e04e-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="1e04e-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="1e04e-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="1e04e-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="1e04e-118">**値**</span><span class="sxs-lookup"><span data-stu-id="1e04e-118">**Value**</span></span>|<span data-ttu-id="1e04e-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="1e04e-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="1e04e-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="1e04e-120">**Success**</span></span> <br/> |<span data-ttu-id="1e04e-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1e04e-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="1e04e-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="1e04e-122">**Warning**</span></span> <br/> | <span data-ttu-id="1e04e-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1e04e-123">Describes a request that was not processed.</span></span> <span data-ttu-id="1e04e-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="1e04e-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="1e04e-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1e04e-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="1e04e-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="1e04e-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="1e04e-127">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="1e04e-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="1e04e-128">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="1e04e-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="1e04e-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="1e04e-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="1e04e-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="1e04e-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="1e04e-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="1e04e-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="1e04e-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="1e04e-132">**Error**</span></span> <br/> | <span data-ttu-id="1e04e-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="1e04e-133">Describes a request that cannot be fulfilled.</span></span><br/><br/> <span data-ttu-id="1e04e-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="1e04e-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="1e04e-135">-無効な属性または要素。</span><span class="sxs-lookup"><span data-stu-id="1e04e-135">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="1e04e-136">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="1e04e-136">-  Attributes or elements that are out of range.</span></span>  <br/><span data-ttu-id="1e04e-137">-不明なタグです。</span><span class="sxs-lookup"><span data-stu-id="1e04e-137">-  An unknown tag.</span></span>  <br/><span data-ttu-id="1e04e-138">-属性または要素はコンテキスト内で有効ではありません。</span><span class="sxs-lookup"><span data-stu-id="1e04e-138">-  The attribute or element is not valid in the context.</span></span>  <br/><span data-ttu-id="1e04e-139">-任意のクライアントで不正なアクセス試行。</span><span class="sxs-lookup"><span data-stu-id="1e04e-139">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="1e04e-140">-クライアント側の有効な呼び出しへの応答でサーバー側エラーです。</span><span class="sxs-lookup"><span data-stu-id="1e04e-140">-  A server-side failure in response to a valid client-side call.</span></span><br/><br/>  <span data-ttu-id="1e04e-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="1e04e-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="1e04e-142">子要素</span><span class="sxs-lookup"><span data-stu-id="1e04e-142">Child elements</span></span>

|<span data-ttu-id="1e04e-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="1e04e-143">**Element**</span></span>|<span data-ttu-id="1e04e-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="1e04e-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e04e-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="1e04e-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="1e04e-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="1e04e-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="1e04e-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1e04e-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="1e04e-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="1e04e-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="1e04e-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="1e04e-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="1e04e-150">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="1e04e-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="1e04e-151">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1e04e-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="1e04e-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="1e04e-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="1e04e-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="1e04e-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="1e04e-154">親要素</span><span class="sxs-lookup"><span data-stu-id="1e04e-154">Parent elements</span></span>

|<span data-ttu-id="1e04e-155">**要素**</span><span class="sxs-lookup"><span data-stu-id="1e04e-155">**Element**</span></span>|<span data-ttu-id="1e04e-156">**説明**</span><span class="sxs-lookup"><span data-stu-id="1e04e-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="1e04e-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="1e04e-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="1e04e-158">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="1e04e-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="1e04e-159">テキスト値</span><span class="sxs-lookup"><span data-stu-id="1e04e-159">Text value</span></span>

<span data-ttu-id="1e04e-160">なし。</span><span class="sxs-lookup"><span data-stu-id="1e04e-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="1e04e-161">備考</span><span class="sxs-lookup"><span data-stu-id="1e04e-161">Remarks</span></span>

<span data-ttu-id="1e04e-162">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="1e04e-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="1e04e-163">要素情報</span><span class="sxs-lookup"><span data-stu-id="1e04e-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="1e04e-164">名前空間</span><span class="sxs-lookup"><span data-stu-id="1e04e-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="1e04e-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="1e04e-165">Schema Name</span></span>  <br/> |<span data-ttu-id="1e04e-166">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="1e04e-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="1e04e-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="1e04e-167">Validation File</span></span>  <br/> |<span data-ttu-id="1e04e-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="1e04e-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="1e04e-169">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="1e04e-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="1e04e-170">False</span><span class="sxs-lookup"><span data-stu-id="1e04e-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="1e04e-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="1e04e-171">See also</span></span>

- [<span data-ttu-id="1e04e-172">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="1e04e-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

