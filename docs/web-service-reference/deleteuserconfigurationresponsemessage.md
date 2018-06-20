---
title: DeleteUserConfigurationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteUserConfigurationResponseMessage
api_type:
- schema
ms.assetid: 543b1743-7e1c-4acb-93bd-34532e7fe79b
description: DeleteUserConfigurationResponseMessage 要素には、状態および 1 つの DeleteUserConfiguration 要求の結果が含まれています。
ms.openlocfilehash: 3e07917688ad1f25f7ca3fa06d6db51cf9905503
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760000"
---
# <a name="deleteuserconfigurationresponsemessage"></a><span data-ttu-id="6cf0f-103">DeleteUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="6cf0f-103">DeleteUserConfigurationResponseMessage</span></span>

<span data-ttu-id="6cf0f-104">**DeleteUserConfigurationResponseMessage**要素には、状態および 1 つの**DeleteUserConfiguration**要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-104">The **DeleteUserConfigurationResponseMessage** element contains the status and result of a single **DeleteUserConfiguration** request.</span></span> 
  
```xml
<DeleteUserConfigurationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteUserConfigurationResponseMessage>
```

 <span data-ttu-id="6cf0f-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="6cf0f-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="6cf0f-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="6cf0f-106">Attributes and elements</span></span>

<span data-ttu-id="6cf0f-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="6cf0f-108">属性</span><span class="sxs-lookup"><span data-stu-id="6cf0f-108">Attributes</span></span>

|<span data-ttu-id="6cf0f-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="6cf0f-109">**Attribute**</span></span>|<span data-ttu-id="6cf0f-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="6cf0f-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6cf0f-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="6cf0f-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="6cf0f-112">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-112">Describes the status of the response.</span></span><br/><br/><span data-ttu-id="6cf0f-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-113">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="6cf0f-114">-成功</span><span class="sxs-lookup"><span data-stu-id="6cf0f-114">-  Success</span></span>  <br/><span data-ttu-id="6cf0f-115">-警告</span><span class="sxs-lookup"><span data-stu-id="6cf0f-115">-  Warning</span></span>  <br/><span data-ttu-id="6cf0f-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="6cf0f-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="6cf0f-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="6cf0f-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="6cf0f-118">**値**</span><span class="sxs-lookup"><span data-stu-id="6cf0f-118">**Value**</span></span>|<span data-ttu-id="6cf0f-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="6cf0f-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="6cf0f-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="6cf0f-120">**Success**</span></span> <br/> |<span data-ttu-id="6cf0f-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="6cf0f-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="6cf0f-122">**Warning**</span></span> <br/> | <span data-ttu-id="6cf0f-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-123">Describes a request that was not processed.</span></span> <span data-ttu-id="6cf0f-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="6cf0f-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-125">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="6cf0f-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="6cf0f-127">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-127">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="6cf0f-128">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="6cf0f-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="6cf0f-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="6cf0f-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="6cf0f-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="6cf0f-132">**Error**</span></span> <br/> | <span data-ttu-id="6cf0f-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-133">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="6cf0f-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-134">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="6cf0f-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="6cf0f-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="6cf0f-136">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-136">-  Attributes or elements that are out of range</span></span>  <br/><span data-ttu-id="6cf0f-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="6cf0f-137">-  An unknown tag</span></span>  <br/><span data-ttu-id="6cf0f-138">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-138">-  An attribute or element that is not valid in the context</span></span>  <br/><span data-ttu-id="6cf0f-139">-任意のクライアントから不正なアクセス試行</span><span class="sxs-lookup"><span data-stu-id="6cf0f-139">-  An unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="6cf0f-140">-クライアント側の有効な呼び出しへの応答でサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="6cf0f-140">-  A server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="6cf0f-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="6cf0f-142">子要素</span><span class="sxs-lookup"><span data-stu-id="6cf0f-142">Child elements</span></span>

|<span data-ttu-id="6cf0f-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="6cf0f-143">**Element**</span></span>|<span data-ttu-id="6cf0f-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="6cf0f-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cf0f-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="6cf0f-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="6cf0f-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="6cf0f-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="6cf0f-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="6cf0f-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="6cf0f-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="6cf0f-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="6cf0f-150">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="6cf0f-151">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="6cf0f-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="6cf0f-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="6cf0f-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="6cf0f-154">親要素</span><span class="sxs-lookup"><span data-stu-id="6cf0f-154">Parent elements</span></span>

|<span data-ttu-id="6cf0f-155">**要素**</span><span class="sxs-lookup"><span data-stu-id="6cf0f-155">**Element**</span></span>|<span data-ttu-id="6cf0f-156">**説明**</span><span class="sxs-lookup"><span data-stu-id="6cf0f-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="6cf0f-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="6cf0f-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="6cf0f-158">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="text-value"></a><span data-ttu-id="6cf0f-159">テキスト値</span><span class="sxs-lookup"><span data-stu-id="6cf0f-159">Text value</span></span>

<span data-ttu-id="6cf0f-160">なし。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-160">None.</span></span>
  
## <a name="remarks"></a><span data-ttu-id="6cf0f-161">備考</span><span class="sxs-lookup"><span data-stu-id="6cf0f-161">Remarks</span></span>

<span data-ttu-id="6cf0f-162">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="6cf0f-162">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="6cf0f-163">要素情報</span><span class="sxs-lookup"><span data-stu-id="6cf0f-163">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="6cf0f-164">名前空間</span><span class="sxs-lookup"><span data-stu-id="6cf0f-164">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="6cf0f-165">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="6cf0f-165">Schema Name</span></span>  <br/> |<span data-ttu-id="6cf0f-166">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="6cf0f-166">Messages schema</span></span>  <br/> |
|<span data-ttu-id="6cf0f-167">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="6cf0f-167">Validation File</span></span>  <br/> |<span data-ttu-id="6cf0f-168">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="6cf0f-168">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="6cf0f-169">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="6cf0f-169">Can be Empty</span></span>  <br/> |<span data-ttu-id="6cf0f-170">False</span><span class="sxs-lookup"><span data-stu-id="6cf0f-170">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="6cf0f-171">関連項目</span><span class="sxs-lookup"><span data-stu-id="6cf0f-171">See also</span></span>

- [<span data-ttu-id="6cf0f-172">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="6cf0f-172">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

