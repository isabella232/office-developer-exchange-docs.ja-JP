---
title: UpdateUserConfigurationResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UpdateUserConfigurationResponseMessage
api_type:
- schema
ms.assetid: 27728e57-5a9b-4314-ad64-df7869098f62
description: UpdateUserConfigurationResponseMessage 要素には、状態および 1 つの UpdateUserConfiguration 操作要求の結果が含まれています。
ms.openlocfilehash: db26bb4bc821ac9a09c350009ab8132466e759bf
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19839899"
---
# <a name="updateuserconfigurationresponsemessage"></a><span data-ttu-id="d2693-103">UpdateUserConfigurationResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d2693-103">UpdateUserConfigurationResponseMessage</span></span>

<span data-ttu-id="d2693-104">**UpdateUserConfigurationResponseMessage**要素には、状態および 1 つの UpdateUserConfiguration 操作要求の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d2693-104">The **UpdateUserConfigurationResponseMessage** element contains the status and result of a single UpdateUserConfiguration operation request.</span></span> 
  
```xml
<UpdateUserConfigurationResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UpdateUserConfigurationResponseMessage>
```

 <span data-ttu-id="d2693-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d2693-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d2693-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="d2693-106">Attributes and elements</span></span>

<span data-ttu-id="d2693-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d2693-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d2693-108">属性</span><span class="sxs-lookup"><span data-stu-id="d2693-108">Attributes</span></span>

|<span data-ttu-id="d2693-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="d2693-109">**Attribute**</span></span>|<span data-ttu-id="d2693-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2693-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d2693-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="d2693-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d2693-112">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="d2693-112">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="d2693-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="d2693-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="d2693-114">-成功</span><span class="sxs-lookup"><span data-stu-id="d2693-114">-  Success</span></span>  <br/><span data-ttu-id="d2693-115">-警告</span><span class="sxs-lookup"><span data-stu-id="d2693-115">-  Warning</span></span>  <br/><span data-ttu-id="d2693-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="d2693-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d2693-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="d2693-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="d2693-118">**値**</span><span class="sxs-lookup"><span data-stu-id="d2693-118">**Value**</span></span>|<span data-ttu-id="d2693-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2693-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d2693-120">**Success**</span><span class="sxs-lookup"><span data-stu-id="d2693-120">**Success**</span></span> <br/> |<span data-ttu-id="d2693-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="d2693-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d2693-122">**Warning**</span><span class="sxs-lookup"><span data-stu-id="d2693-122">**Warning**</span></span> <br/> | <span data-ttu-id="d2693-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="d2693-123">Describes a request that was not processed.</span></span> <span data-ttu-id="d2693-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="d2693-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="d2693-125">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d2693-125">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="d2693-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="d2693-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="d2693-127">-Active Directory ディレクトリ サービスは、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="d2693-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="d2693-128">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="d2693-128">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="d2693-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="d2693-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="d2693-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="d2693-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="d2693-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="d2693-131">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="d2693-132">**Error**</span><span class="sxs-lookup"><span data-stu-id="d2693-132">**Error**</span></span> <br/> | <span data-ttu-id="d2693-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="d2693-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="d2693-134">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="d2693-134">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="d2693-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="d2693-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="d2693-136">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="d2693-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="d2693-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="d2693-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="d2693-138">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="d2693-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="d2693-139">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="d2693-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="d2693-140">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="d2693-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="d2693-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="d2693-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d2693-142">子要素</span><span class="sxs-lookup"><span data-stu-id="d2693-142">Child elements</span></span>

|<span data-ttu-id="d2693-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="d2693-143">**Element**</span></span>|<span data-ttu-id="d2693-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2693-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2693-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="d2693-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="d2693-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="d2693-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="d2693-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d2693-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="d2693-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="d2693-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="d2693-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d2693-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="d2693-150">現在使用されていない、将来使用するために予約されています。</span><span class="sxs-lookup"><span data-stu-id="d2693-150">Currently unused and reserved for future use.</span></span> <span data-ttu-id="d2693-151">この要素には、0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d2693-151">This element contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="d2693-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="d2693-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="d2693-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="d2693-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d2693-154">親要素</span><span class="sxs-lookup"><span data-stu-id="d2693-154">Parent elements</span></span>

|<span data-ttu-id="d2693-155">**要素**</span><span class="sxs-lookup"><span data-stu-id="d2693-155">**Element**</span></span>|<span data-ttu-id="d2693-156">**説明**</span><span class="sxs-lookup"><span data-stu-id="d2693-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d2693-157">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d2693-157">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d2693-158">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="d2693-158">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d2693-159">備考</span><span class="sxs-lookup"><span data-stu-id="d2693-159">Remarks</span></span>

<span data-ttu-id="d2693-160">この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割と Exchange Server を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="d2693-160">The schema that describes this element is located in the EWS virtual directory of the computer that is running Exchange Server with the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d2693-161">要素情報</span><span class="sxs-lookup"><span data-stu-id="d2693-161">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d2693-162">名前空間</span><span class="sxs-lookup"><span data-stu-id="d2693-162">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d2693-163">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d2693-163">Schema Name</span></span>  <br/> |<span data-ttu-id="d2693-164">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="d2693-164">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d2693-165">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d2693-165">Validation File</span></span>  <br/> |<span data-ttu-id="d2693-166">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="d2693-166">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d2693-167">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d2693-167">Can be Empty</span></span>  <br/> |<span data-ttu-id="d2693-168">False</span><span class="sxs-lookup"><span data-stu-id="d2693-168">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d2693-169">関連項目</span><span class="sxs-lookup"><span data-stu-id="d2693-169">See also</span></span>

- [<span data-ttu-id="d2693-170">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="d2693-170">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

