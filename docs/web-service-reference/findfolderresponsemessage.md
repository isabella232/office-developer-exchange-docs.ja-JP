---
title: FindFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FindFolderResponseMessage
api_type:
- schema
ms.assetid: 538d64fe-51ae-41d2-bfab-91698678aa1b
description: FindFolderResponseMessage 要素には、状態および 1 つの FindFolder 操作要求の結果が含まれています。
ms.openlocfilehash: 5623e5e538e617e5bd4bbc4444328ac83d7b8065
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760509"
---
# <a name="findfolderresponsemessage"></a><span data-ttu-id="c0d1b-103">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c0d1b-103">FindFolderResponseMessage</span></span>

<span data-ttu-id="c0d1b-104">**FindFolderResponseMessage**要素には、状態および 1 つの結果が含まれています[FindFolder 操作](findfolder-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-104">The **FindFolderResponseMessage** element contains the status and result of a single [FindFolder operation](findfolder-operation.md) request.</span></span> 
  
[<span data-ttu-id="c0d1b-105">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="c0d1b-105">FindFolderResponse</span></span>](findfolderresponse.md)
  
[<span data-ttu-id="c0d1b-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c0d1b-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="c0d1b-107">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c0d1b-107">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md)
  
```xml
<FindFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootFolder/>
</FindFolderResponseMessage>
```

 <span data-ttu-id="c0d1b-108">**FindFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c0d1b-108">**FindFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c0d1b-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="c0d1b-109">Attributes and elements</span></span>

<span data-ttu-id="c0d1b-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c0d1b-111">属性</span><span class="sxs-lookup"><span data-stu-id="c0d1b-111">Attributes</span></span>

|<span data-ttu-id="c0d1b-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="c0d1b-112">**Attribute**</span></span>|<span data-ttu-id="c0d1b-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="c0d1b-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c0d1b-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="c0d1b-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="c0d1b-115">[FindFolder 操作](findfolder-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-115">Describes the status of a [FindFolder operation](findfolder-operation.md) response.</span></span><br/><br/> <span data-ttu-id="c0d1b-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="c0d1b-117">-成功</span><span class="sxs-lookup"><span data-stu-id="c0d1b-117">-  Success</span></span>  <br/><span data-ttu-id="c0d1b-118">-警告</span><span class="sxs-lookup"><span data-stu-id="c0d1b-118">-  Warning</span></span>  <br/><span data-ttu-id="c0d1b-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="c0d1b-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="c0d1b-120">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="c0d1b-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="c0d1b-121">**値**</span><span class="sxs-lookup"><span data-stu-id="c0d1b-121">**Value**</span></span>|<span data-ttu-id="c0d1b-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="c0d1b-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c0d1b-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="c0d1b-123">**Success**</span></span> <br/> |<span data-ttu-id="c0d1b-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="c0d1b-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="c0d1b-125">**Warning**</span></span> <br/> | <span data-ttu-id="c0d1b-126">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-126">Describes a request that was not processed.</span></span> <span data-ttu-id="c0d1b-127">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="c0d1b-128">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="c0d1b-129">-Exchange ストアは、バッチの中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="c0d1b-130">-Active Directory ドメイン サービス (AD DS) がオフラインになった。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="c0d1b-131">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="c0d1b-132">-メッセージ データベース (MDB) がオフラインになった。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="c0d1b-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="c0d1b-134">クォータを超過しました。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="c0d1b-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="c0d1b-135">**Error**</span></span> <br/> | <span data-ttu-id="c0d1b-136">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="c0d1b-137">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-137">The following are examples of sources of errors:</span></span>  <br/><span data-ttu-id="c0d1b-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="c0d1b-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="c0d1b-139">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="c0d1b-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="c0d1b-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="c0d1b-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="c0d1b-141">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="c0d1b-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="c0d1b-142">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="c0d1b-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="c0d1b-143">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="c0d1b-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="c0d1b-144">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c0d1b-145">子要素</span><span class="sxs-lookup"><span data-stu-id="c0d1b-145">Child elements</span></span>

|<span data-ttu-id="c0d1b-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="c0d1b-146">**Element**</span></span>|<span data-ttu-id="c0d1b-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="c0d1b-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0d1b-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="c0d1b-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c0d1b-149">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c0d1b-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c0d1b-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c0d1b-151">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="c0d1b-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c0d1b-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c0d1b-153">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="c0d1b-154">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="c0d1b-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c0d1b-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c0d1b-156">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="c0d1b-157">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="c0d1b-157">RootFolder (FindFolderResponseMessage)</span></span>](rootfolder-findfolderresponsemessage.md) <br/> |<span data-ttu-id="c0d1b-158">[FindFolder 操作](findfolder-operation.md)中に単一のルート フォルダーの検索の結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-158">Contains the results from a search of a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c0d1b-159">親要素</span><span class="sxs-lookup"><span data-stu-id="c0d1b-159">Parent elements</span></span>

|<span data-ttu-id="c0d1b-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="c0d1b-160">**Element**</span></span>|<span data-ttu-id="c0d1b-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="c0d1b-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c0d1b-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c0d1b-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="c0d1b-163">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c0d1b-164">備考</span><span class="sxs-lookup"><span data-stu-id="c0d1b-164">Remarks</span></span>

<span data-ttu-id="c0d1b-165">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c0d1b-166">要素情報</span><span class="sxs-lookup"><span data-stu-id="c0d1b-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c0d1b-167">名前空間</span><span class="sxs-lookup"><span data-stu-id="c0d1b-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c0d1b-168">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c0d1b-168">Schema name</span></span>  <br/> |<span data-ttu-id="c0d1b-169">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="c0d1b-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c0d1b-170">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c0d1b-170">Validation file</span></span>  <br/> |<span data-ttu-id="c0d1b-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="c0d1b-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c0d1b-172">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-172">Can be empty</span></span>  <br/> |<span data-ttu-id="c0d1b-173">False</span><span class="sxs-lookup"><span data-stu-id="c0d1b-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c0d1b-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="c0d1b-174">See also</span></span>

- <span data-ttu-id="c0d1b-175">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="c0d1b-175">[FindFolder operation](findfolder-operation.md)</span></span>
- [<span data-ttu-id="c0d1b-176">フォルダーを検索します。</span><span class="sxs-lookup"><span data-stu-id="c0d1b-176">Finding Folders</span></span>](http://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

