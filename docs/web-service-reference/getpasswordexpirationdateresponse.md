---
title: GetPasswordExpirationDateResponse
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 3d3fff1f-ef13-46d5-bd7f-ef535eb80c72
description: GetPasswordExpirationDateResponse 要素は、GetPasswordExpirationDate 操作操作要求への応答を定義します。
ms.openlocfilehash: c925b2b37879ba0f8f25b2dd73737ed2f3202555
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530205"
---
# <a name="getpasswordexpirationdateresponse"></a><span data-ttu-id="d54f7-103">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="d54f7-103">GetPasswordExpirationDateResponse</span></span>

<span data-ttu-id="d54f7-104">**GetPasswordExpirationDateResponse**要素は、 [GetPasswordExpirationDate 操作](getpasswordexpirationdate-operation.md)操作要求への応答を定義します。</span><span class="sxs-lookup"><span data-stu-id="d54f7-104">The **GetPasswordExpirationDateResponse** element defines the response to a [GetPasswordExpirationDate operation](getpasswordexpirationdate-operation.md) operation request.</span></span> 
  
- [<span data-ttu-id="d54f7-105">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d54f7-105">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="d54f7-106">GetPasswordExpirationDateResponse</span><span class="sxs-lookup"><span data-stu-id="d54f7-106">GetPasswordExpirationDateResponse</span></span>](getpasswordexpirationdateresponse.md)
  
```XML
<GetPasswordExpirationDateResponse>
    <PasswordExpirationDate />
</GetPasswordExpirationDateResponse>
```

 <span data-ttu-id="d54f7-107">**GetPasswordExpirationDateResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="d54f7-107">**GetPasswordExpirationDateResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="d54f7-108">属性と要素</span><span class="sxs-lookup"><span data-stu-id="d54f7-108">Attributes and elements</span></span>

<span data-ttu-id="d54f7-109">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="d54f7-109">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="d54f7-110">属性</span><span class="sxs-lookup"><span data-stu-id="d54f7-110">Attributes</span></span>

|<span data-ttu-id="d54f7-111">**属性**</span><span class="sxs-lookup"><span data-stu-id="d54f7-111">**Attribute**</span></span>|<span data-ttu-id="d54f7-112">**説明**</span><span class="sxs-lookup"><span data-stu-id="d54f7-112">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d54f7-113">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="d54f7-113">**ResponseClass**</span></span> <br/> | <span data-ttu-id="d54f7-114">応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="d54f7-114">Describes the status of the response.</span></span> <br/><br/><span data-ttu-id="d54f7-115">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="d54f7-115">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="d54f7-116">-成功</span><span class="sxs-lookup"><span data-stu-id="d54f7-116">-  Success</span></span>  <br/><span data-ttu-id="d54f7-117">-Warning</span><span class="sxs-lookup"><span data-stu-id="d54f7-117">-  Warning</span></span>  <br/><span data-ttu-id="d54f7-118">-エラー</span><span class="sxs-lookup"><span data-stu-id="d54f7-118">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="d54f7-119">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="d54f7-119">ResponseClass attribute values</span></span>

|<span data-ttu-id="d54f7-120">**値**</span><span class="sxs-lookup"><span data-stu-id="d54f7-120">**Value**</span></span>|<span data-ttu-id="d54f7-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="d54f7-121">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="d54f7-122">**Success**</span><span class="sxs-lookup"><span data-stu-id="d54f7-122">**Success**</span></span> <br/> |<span data-ttu-id="d54f7-123">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="d54f7-123">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="d54f7-124">**Warning**</span><span class="sxs-lookup"><span data-stu-id="d54f7-124">**Warning**</span></span> <br/> | <span data-ttu-id="d54f7-125">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="d54f7-125">Describes a request that was not processed.</span></span> <span data-ttu-id="d54f7-126">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d54f7-126">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="d54f7-127">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d54f7-127">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="d54f7-128">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="d54f7-128">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="d54f7-129">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="d54f7-129">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="d54f7-130">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="d54f7-130">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="d54f7-131">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="d54f7-131">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="d54f7-132">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="d54f7-132">-  A password is expired.</span></span>  <br/><span data-ttu-id="d54f7-133">-クォータが限界を超えています。</span><span class="sxs-lookup"><span data-stu-id="d54f7-133">-  A quota has been exceeded.</span></span>  <br/> |
|<span data-ttu-id="d54f7-134">**Error**</span><span class="sxs-lookup"><span data-stu-id="d54f7-134">**Error**</span></span> <br/> | <span data-ttu-id="d54f7-135">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="d54f7-135">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="d54f7-136">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d54f7-136">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="d54f7-137">-属性または要素が無効です。</span><span class="sxs-lookup"><span data-stu-id="d54f7-137">-  Invalid attributes or elements.</span></span>  <br/><span data-ttu-id="d54f7-138">-範囲外の属性または要素。</span><span class="sxs-lookup"><span data-stu-id="d54f7-138">-  Attributes or elements that are out of range.</span></span>  <br/><span data-ttu-id="d54f7-139">-不明なタグ。</span><span class="sxs-lookup"><span data-stu-id="d54f7-139">-  An unknown tag.</span></span>  <br/><span data-ttu-id="d54f7-140">-コンテキスト内で有効ではない属性または要素。</span><span class="sxs-lookup"><span data-stu-id="d54f7-140">-  An attribute or element that is not valid in the context.</span></span>  <br/><span data-ttu-id="d54f7-141">-クライアントによる権限のないアクセス試行。</span><span class="sxs-lookup"><span data-stu-id="d54f7-141">-  An unauthorized access attempt by any client.</span></span>  <br/><span data-ttu-id="d54f7-142">-有効なクライアント側の呼び出しに応答して、サーバー側で障害が発生した。</span><span class="sxs-lookup"><span data-stu-id="d54f7-142">-  A server-side failure in response to a valid client-side call.</span></span>  <br/><br/>  <span data-ttu-id="d54f7-143">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d54f7-143">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="d54f7-144">子要素</span><span class="sxs-lookup"><span data-stu-id="d54f7-144">Child elements</span></span>

|<span data-ttu-id="d54f7-145">**要素名**</span><span class="sxs-lookup"><span data-stu-id="d54f7-145">**Element name**</span></span>|<span data-ttu-id="d54f7-146">**説明**</span><span class="sxs-lookup"><span data-stu-id="d54f7-146">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d54f7-147">PasswordExpirationDate</span><span class="sxs-lookup"><span data-stu-id="d54f7-147">PasswordExpirationDate</span></span>](passwordexpirationdate.md) <br/> |<span data-ttu-id="d54f7-148">要求で指定された電子メールアカウントのパスワードの有効期限日を示します。</span><span class="sxs-lookup"><span data-stu-id="d54f7-148">Provides the password expiration date for the email account specified in the request.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="d54f7-149">親要素</span><span class="sxs-lookup"><span data-stu-id="d54f7-149">Parent elements</span></span>

|<span data-ttu-id="d54f7-150">**要素名**</span><span class="sxs-lookup"><span data-stu-id="d54f7-150">**Element name**</span></span>|<span data-ttu-id="d54f7-151">**説明**</span><span class="sxs-lookup"><span data-stu-id="d54f7-151">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="d54f7-152">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d54f7-152">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="d54f7-153">Exchange Web サービス (EWS) 要求に対する応答メッセージが保存されています。</span><span class="sxs-lookup"><span data-stu-id="d54f7-153">Contains the response messages for an Exchange Web Services (EWS) request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="d54f7-154">注釈</span><span class="sxs-lookup"><span data-stu-id="d54f7-154">Remarks</span></span>

<span data-ttu-id="d54f7-155">この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。</span><span class="sxs-lookup"><span data-stu-id="d54f7-155">The schema that describes this element is located in the IIS virtual directory that hosts Exchange Web Services.</span></span>
  
<span data-ttu-id="d54f7-156">この要素は Exchange Server 2010 Service Pack 2 (SP2) で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d54f7-156">This element was introduced in Exchange Server 2010 Service Pack 2 (SP2).</span></span>
  
## <a name="element-information"></a><span data-ttu-id="d54f7-157">要素の情報</span><span class="sxs-lookup"><span data-stu-id="d54f7-157">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="d54f7-158">Namespace</span><span class="sxs-lookup"><span data-stu-id="d54f7-158">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="d54f7-159">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="d54f7-159">Schema Name</span></span>  <br/> |<span data-ttu-id="d54f7-160">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="d54f7-160">Messages schema</span></span>  <br/> |
|<span data-ttu-id="d54f7-161">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="d54f7-161">Validation File</span></span>  <br/> |<span data-ttu-id="d54f7-162">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="d54f7-162">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="d54f7-163">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="d54f7-163">Can be Empty</span></span>  <br/> |<span data-ttu-id="d54f7-164">正しくない</span><span class="sxs-lookup"><span data-stu-id="d54f7-164">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="d54f7-165">関連項目</span><span class="sxs-lookup"><span data-stu-id="d54f7-165">See also</span></span>

- [<span data-ttu-id="d54f7-166">GetPasswordExpirationDate 操作</span><span class="sxs-lookup"><span data-stu-id="d54f7-166">GetPasswordExpirationDate operation</span></span>](getpasswordexpirationdate-operation.md)
- [<span data-ttu-id="d54f7-167">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="d54f7-167">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

