---
title: GetPasswordExpirationDateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d3fff1f-ef13-46d5-bd7f-ef535eb80c72
description: GetPasswordExpirationDateResponse 要素は、GetPasswordExpirationDate 操作の操作要求に対する応答を定義します。
ms.openlocfilehash: 3754a53da53c12479f11c2e32cd15a08cba665fb
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760830"
---
# <a name="getpasswordexpirationdateresponse"></a><span data-ttu-id="0902f-103">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="0902f-103">GetPasswordExpirationDateResponse</span></span>

<span data-ttu-id="0902f-104">**GetPasswordExpirationDateResponse**要素は、 [GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md)の操作要求に対する応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="0902f-104">The **GetPasswordExpirationDateResponse** element defines the response to a [GetPasswordExpirationDate operation](getpasswordexpirationdate-operation.md) operation request.</span></span> 
  
- [<span data-ttu-id="0902f-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0902f-105">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="0902f-106">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="0902f-106">GetPasswordExpirationDateResponse</span></span>](getpasswordexpirationdateresponse.md)
  
```XML
<GetPasswordExpirationDateResponse>
    <PasswordExpirationDate />
</GetPasswordExpirationDateResponse>
```

 <span data-ttu-id="0902f-107">**GetPasswordExpirationDateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="0902f-107">**GetPasswordExpirationDateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="0902f-108">属性および要素</span><span class="sxs-lookup"><span data-stu-id="0902f-108">Attributes and elements</span></span>

<span data-ttu-id="0902f-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="0902f-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="0902f-110">属性</span><span class="sxs-lookup"><span data-stu-id="0902f-110">Attributes</span></span>

|<span data-ttu-id="0902f-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="0902f-111">**Attribute**</span></span>|<span data-ttu-id="0902f-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="0902f-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0902f-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="0902f-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="0902f-114">応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="0902f-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="0902f-115">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="0902f-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="0902f-116">-成功</span><span class="sxs-lookup"><span data-stu-id="0902f-116">-  Success</span></span>  <br/><span data-ttu-id="0902f-117">-警告</span><span class="sxs-lookup"><span data-stu-id="0902f-117">-  Warning</span></span>  <br/><span data-ttu-id="0902f-118">-エラー</span><span class="sxs-lookup"><span data-stu-id="0902f-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="0902f-119">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="0902f-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="0902f-120">**値**</span><span class="sxs-lookup"><span data-stu-id="0902f-120">**Value**</span></span>|<span data-ttu-id="0902f-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="0902f-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="0902f-122">**Success**</span><span class="sxs-lookup"><span data-stu-id="0902f-122">**Success**</span></span> <br/> |<span data-ttu-id="0902f-123">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="0902f-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="0902f-124">**Warning**</span><span class="sxs-lookup"><span data-stu-id="0902f-124">**Warning**</span></span> <br/> | <span data-ttu-id="0902f-125">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="0902f-125">Describes a request that was not processed.</span></span> <span data-ttu-id="0902f-126">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="0902f-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="0902f-127">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="0902f-127">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="0902f-128">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="0902f-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="0902f-129">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="0902f-129">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="0902f-130">-メールボックスは移動されました。</span><span class="sxs-lookup"><span data-stu-id="0902f-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="0902f-131">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="0902f-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="0902f-132">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="0902f-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="0902f-133">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="0902f-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="0902f-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="0902f-134">**Error**</span></span> <br/> | <span data-ttu-id="0902f-135">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="0902f-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="0902f-136">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="0902f-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="0902f-137">-無効な属性または要素。</span><span class="sxs-lookup"><span data-stu-id="0902f-137">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="0902f-138">属性または要素の範囲を超えています。</span><span class="sxs-lookup"><span data-stu-id="0902f-138">-  Attributes or elements that are out of range.</span></span>  <br/><span data-ttu-id="0902f-139">-不明なタグです。</span><span class="sxs-lookup"><span data-stu-id="0902f-139">-  An unknown tag.</span></span>  <br/><span data-ttu-id="0902f-140">属性または要素のコンテキストでは有効ではないです。</span><span class="sxs-lookup"><span data-stu-id="0902f-140">-  An attribute or element that is not valid in the context.</span></span>  <br/><span data-ttu-id="0902f-141">-任意のクライアントで不正なアクセス試行。</span><span class="sxs-lookup"><span data-stu-id="0902f-141">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="0902f-142">-クライアント側の有効な呼び出しへの応答でサーバー側エラーです。</span><span class="sxs-lookup"><span data-stu-id="0902f-142">-  A server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="0902f-143">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="0902f-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="0902f-144">子要素</span><span class="sxs-lookup"><span data-stu-id="0902f-144">Child elements</span></span>

|<span data-ttu-id="0902f-145">**要素名**</span><span class="sxs-lookup"><span data-stu-id="0902f-145">**Element name**</span></span>|<span data-ttu-id="0902f-146">**説明**</span><span class="sxs-lookup"><span data-stu-id="0902f-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0902f-147">PasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="0902f-147">PasswordExpirationDate</span></span>](passwordexpirationdate.md) <br/> |<span data-ttu-id="0902f-148">要求で指定されている電子メール アカウントのパスワードの有効期限の日付を提供します。</span><span class="sxs-lookup"><span data-stu-id="0902f-148">Provides the password expiration date for the email account specified in the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="0902f-149">親要素</span><span class="sxs-lookup"><span data-stu-id="0902f-149">Parent elements</span></span>

|<span data-ttu-id="0902f-150">**要素名**</span><span class="sxs-lookup"><span data-stu-id="0902f-150">**Element name**</span></span>|<span data-ttu-id="0902f-151">**説明**</span><span class="sxs-lookup"><span data-stu-id="0902f-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="0902f-152">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="0902f-152">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="0902f-153">Exchange Web サービス (EWS) 要求の応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="0902f-153">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="0902f-154">備考</span><span class="sxs-lookup"><span data-stu-id="0902f-154">Remarks</span></span>

<span data-ttu-id="0902f-155">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="0902f-155">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="0902f-156">この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0902f-156">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="0902f-157">要素情報</span><span class="sxs-lookup"><span data-stu-id="0902f-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="0902f-158">名前空間</span><span class="sxs-lookup"><span data-stu-id="0902f-158">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="0902f-159">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="0902f-159">Schema Name</span></span>  <br/> |<span data-ttu-id="0902f-160">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="0902f-160">Messages schema</span></span>  <br/> |
|<span data-ttu-id="0902f-161">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="0902f-161">Validation File</span></span>  <br/> |<span data-ttu-id="0902f-162">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="0902f-162">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="0902f-163">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="0902f-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="0902f-164">False</span><span class="sxs-lookup"><span data-stu-id="0902f-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="0902f-165">関連項目</span><span class="sxs-lookup"><span data-stu-id="0902f-165">See also</span></span>

- [<span data-ttu-id="0902f-166">GetPasswordExpirationDate 操作</span><span class="sxs-lookup"><span data-stu-id="0902f-166">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)
- [<span data-ttu-id="0902f-167">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="0902f-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

