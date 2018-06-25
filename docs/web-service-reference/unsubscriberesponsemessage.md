---
title: UnsubscribeResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- UnsubscribeResponseMessage
api_type:
- schema
ms.assetid: 92c53b13-0ca1-4b44-b925-b23682e9417c
description: UnsubscribeResponseMessage 要素には、状態および 1 つの購読の取り消し操作要求の結果が含まれています。
ms.openlocfilehash: 09475b8c858ddcd0e404819b6b9a281cbf7cfcbb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839826"
---
# <a name="unsubscriberesponsemessage"></a><span data-ttu-id="39bb3-103">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="39bb3-103">UnsubscribeResponseMessage</span></span>

<span data-ttu-id="39bb3-104">**UnsubscribeResponseMessage**要素には、状態および 1 つの結果が含まれている[購読の取り消し操作](unsubscribe-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="39bb3-104">The **UnsubscribeResponseMessage** element contains the status and result of a single [Unsubscribe operation](unsubscribe-operation.md) request.</span></span> 
  
- [<span data-ttu-id="39bb3-105">UnsubscribeResponse</span><span class="sxs-lookup"><span data-stu-id="39bb3-105">UnsubscribeResponse</span></span>](unsubscriberesponse.md)
- [<span data-ttu-id="39bb3-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="39bb3-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="39bb3-107">UnsubscribeResponseMessage</span><span class="sxs-lookup"><span data-stu-id="39bb3-107">UnsubscribeResponseMessage</span></span>](unsubscriberesponsemessage.md)
  
```xml
<UnsubscribeResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</UnsubscribeResponseMessage>
```

 <span data-ttu-id="39bb3-108">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="39bb3-108">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="39bb3-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="39bb3-109">Attributes and elements</span></span>

<span data-ttu-id="39bb3-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="39bb3-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="39bb3-111">属性</span><span class="sxs-lookup"><span data-stu-id="39bb3-111">Attributes</span></span>

|<span data-ttu-id="39bb3-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="39bb3-112">**Attribute**</span></span>|<span data-ttu-id="39bb3-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="39bb3-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="39bb3-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="39bb3-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="39bb3-115">[購読の取り消し操作](unsubscribe-operation.md)応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="39bb3-115">Describes the status of an [Unsubscribe operation](unsubscribe-operation.md) response.</span></span> <br/><br/><span data-ttu-id="39bb3-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="39bb3-116">The following values are valid for this attribute:</span></span> <br/> <br/><span data-ttu-id="39bb3-117">-成功</span><span class="sxs-lookup"><span data-stu-id="39bb3-117">-  Success</span></span>  <br/><span data-ttu-id="39bb3-118">-警告</span><span class="sxs-lookup"><span data-stu-id="39bb3-118">-  Warning</span></span>  <br/><span data-ttu-id="39bb3-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="39bb3-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="39bb3-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="39bb3-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="39bb3-121">**値**</span><span class="sxs-lookup"><span data-stu-id="39bb3-121">**Value**</span></span>|<span data-ttu-id="39bb3-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="39bb3-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="39bb3-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="39bb3-123">**Success**</span></span> <br/> |<span data-ttu-id="39bb3-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="39bb3-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="39bb3-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="39bb3-125">**Warning**</span></span> <br/> | <span data-ttu-id="39bb3-126">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="39bb3-126">Describes a request that was not processed.</span></span> <span data-ttu-id="39bb3-127">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="39bb3-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="39bb3-128">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="39bb3-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="39bb3-129">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="39bb3-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="39bb3-130">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="39bb3-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="39bb3-131">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="39bb3-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="39bb3-132">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="39bb3-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="39bb3-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="39bb3-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="39bb3-134">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="39bb3-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="39bb3-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="39bb3-135">**Error**</span></span> <br/> | <span data-ttu-id="39bb3-136">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="39bb3-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="39bb3-137">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="39bb3-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="39bb3-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="39bb3-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="39bb3-139">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="39bb3-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="39bb3-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="39bb3-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="39bb3-141">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="39bb3-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="39bb3-142">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="39bb3-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="39bb3-143">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="39bb3-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="39bb3-144">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="39bb3-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="39bb3-145">子要素</span><span class="sxs-lookup"><span data-stu-id="39bb3-145">Child elements</span></span>

|<span data-ttu-id="39bb3-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="39bb3-146">**Element**</span></span>|<span data-ttu-id="39bb3-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="39bb3-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39bb3-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="39bb3-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="39bb3-149">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="39bb3-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="39bb3-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="39bb3-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="39bb3-151">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="39bb3-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="39bb3-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="39bb3-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="39bb3-153">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="39bb3-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="39bb3-154">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="39bb3-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="39bb3-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="39bb3-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="39bb3-156">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="39bb3-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="39bb3-157">親要素</span><span class="sxs-lookup"><span data-stu-id="39bb3-157">Parent elements</span></span>

|<span data-ttu-id="39bb3-158">**要素**</span><span class="sxs-lookup"><span data-stu-id="39bb3-158">**Element**</span></span>|<span data-ttu-id="39bb3-159">**説明**</span><span class="sxs-lookup"><span data-stu-id="39bb3-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="39bb3-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="39bb3-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="39bb3-161">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="39bb3-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="39bb3-162">備考</span><span class="sxs-lookup"><span data-stu-id="39bb3-162">Remarks</span></span>

<span data-ttu-id="39bb3-163">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="39bb3-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="39bb3-164">要素情報</span><span class="sxs-lookup"><span data-stu-id="39bb3-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="39bb3-165">名前空間</span><span class="sxs-lookup"><span data-stu-id="39bb3-165">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="39bb3-166">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="39bb3-166">Schema Name</span></span>  <br/> |<span data-ttu-id="39bb3-167">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="39bb3-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="39bb3-168">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="39bb3-168">Validation File</span></span>  <br/> |<span data-ttu-id="39bb3-169">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="39bb3-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="39bb3-170">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="39bb3-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="39bb3-171">False</span><span class="sxs-lookup"><span data-stu-id="39bb3-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="39bb3-172">関連項目</span><span class="sxs-lookup"><span data-stu-id="39bb3-172">See also</span></span>

- [<span data-ttu-id="39bb3-173">Unsubscribe 操作</span><span class="sxs-lookup"><span data-stu-id="39bb3-173">Unsubscribe operation</span></span>](unsubscribe-operation.md)
- [<span data-ttu-id="39bb3-174">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="39bb3-174">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

