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
description: FindFolderResponseMessage 要素には、単一の FindFolder 操作要求の状態と結果が含まれています。
ms.openlocfilehash: 318a09e371043252d43a5197211e9623f34229fd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462564"
---
# <a name="findfolderresponsemessage"></a><span data-ttu-id="c49cf-103">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c49cf-103">FindFolderResponseMessage</span></span>

<span data-ttu-id="c49cf-104">**FindFolderResponseMessage**要素には、単一の[findfolder 操作](findfolder-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c49cf-104">The **FindFolderResponseMessage** element contains the status and result of a single [FindFolder operation](findfolder-operation.md) request.</span></span> 
  
[<span data-ttu-id="c49cf-105">FindFolderResponse</span><span class="sxs-lookup"><span data-stu-id="c49cf-105">FindFolderResponse</span></span>](findfolderresponse.md)
  
[<span data-ttu-id="c49cf-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c49cf-106">ResponseMessages</span></span>](responsemessages.md)
  
[<span data-ttu-id="c49cf-107">FindFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c49cf-107">FindFolderResponseMessage</span></span>](findfolderresponsemessage.md)
  
```xml
<FindFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <RootFolder/>
</FindFolderResponseMessage>
```

 <span data-ttu-id="c49cf-108">**FindFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="c49cf-108">**FindFolderResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="c49cf-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="c49cf-109">Attributes and elements</span></span>

<span data-ttu-id="c49cf-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="c49cf-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="c49cf-111">属性</span><span class="sxs-lookup"><span data-stu-id="c49cf-111">Attributes</span></span>

|<span data-ttu-id="c49cf-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="c49cf-112">**Attribute**</span></span>|<span data-ttu-id="c49cf-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="c49cf-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c49cf-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="c49cf-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="c49cf-115">[Findfolder 操作](findfolder-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="c49cf-115">Describes the status of a [FindFolder operation](findfolder-operation.md) response.</span></span><br/><br/> <span data-ttu-id="c49cf-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="c49cf-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="c49cf-117">-成功</span><span class="sxs-lookup"><span data-stu-id="c49cf-117">-  Success</span></span>  <br/><span data-ttu-id="c49cf-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="c49cf-118">-  Warning</span></span>  <br/><span data-ttu-id="c49cf-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="c49cf-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="c49cf-120">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="c49cf-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="c49cf-121">**値**</span><span class="sxs-lookup"><span data-stu-id="c49cf-121">**Value**</span></span>|<span data-ttu-id="c49cf-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="c49cf-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="c49cf-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="c49cf-123">**Success**</span></span> <br/> |<span data-ttu-id="c49cf-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="c49cf-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="c49cf-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="c49cf-125">**Warning**</span></span> <br/> | <span data-ttu-id="c49cf-126">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="c49cf-126">Describes a request that was not processed.</span></span> <span data-ttu-id="c49cf-127">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="c49cf-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="c49cf-128">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c49cf-128">The following are examples of sources of warnings:</span></span> <br/> <br/><span data-ttu-id="c49cf-129">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="c49cf-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="c49cf-130">-Active Directory ドメインサービス (AD DS) はオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="c49cf-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="c49cf-131">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="c49cf-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="c49cf-132">-メッセージデータベース (MDB) はオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="c49cf-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="c49cf-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="c49cf-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="c49cf-134">-クォータを超過しました。</span><span class="sxs-lookup"><span data-stu-id="c49cf-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="c49cf-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="c49cf-135">**Error**</span></span> <br/> | <span data-ttu-id="c49cf-136">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="c49cf-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="c49cf-137">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c49cf-137">The following are examples of sources of errors:</span></span>  <br/><span data-ttu-id="c49cf-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="c49cf-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="c49cf-139">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="c49cf-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="c49cf-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="c49cf-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="c49cf-141">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="c49cf-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="c49cf-142">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="c49cf-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="c49cf-143">-有効なクライアント側の呼び出しに応答した場合のサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="c49cf-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="c49cf-144">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c49cf-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="c49cf-145">子要素</span><span class="sxs-lookup"><span data-stu-id="c49cf-145">Child elements</span></span>

|<span data-ttu-id="c49cf-146">**Element**</span><span class="sxs-lookup"><span data-stu-id="c49cf-146">**Element**</span></span>|<span data-ttu-id="c49cf-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="c49cf-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c49cf-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="c49cf-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="c49cf-149">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="c49cf-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="c49cf-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c49cf-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="c49cf-151">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="c49cf-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="c49cf-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c49cf-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="c49cf-153">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="c49cf-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="c49cf-154">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c49cf-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="c49cf-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="c49cf-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="c49cf-156">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="c49cf-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="c49cf-157">RootFolder (FindFolderResponseMessage)</span><span class="sxs-lookup"><span data-stu-id="c49cf-157">RootFolder (FindFolderResponseMessage)</span></span>](rootfolder-findfolderresponsemessage.md) <br/> |<span data-ttu-id="c49cf-158">[Findfolder 操作](findfolder-operation.md)中の1つのルートフォルダーの検索結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c49cf-158">Contains the results from a search of a single root folder during a [FindFolder operation](findfolder-operation.md).</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="c49cf-159">親要素</span><span class="sxs-lookup"><span data-stu-id="c49cf-159">Parent elements</span></span>

|<span data-ttu-id="c49cf-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="c49cf-160">**Element**</span></span>|<span data-ttu-id="c49cf-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="c49cf-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="c49cf-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c49cf-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="c49cf-163">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="c49cf-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="c49cf-164">注釈</span><span class="sxs-lookup"><span data-stu-id="c49cf-164">Remarks</span></span>

<span data-ttu-id="c49cf-165">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="c49cf-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="c49cf-166">要素の情報</span><span class="sxs-lookup"><span data-stu-id="c49cf-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="c49cf-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="c49cf-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="c49cf-168">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="c49cf-168">Schema name</span></span>  <br/> |<span data-ttu-id="c49cf-169">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="c49cf-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="c49cf-170">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="c49cf-170">Validation file</span></span>  <br/> |<span data-ttu-id="c49cf-171">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="c49cf-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="c49cf-172">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="c49cf-172">Can be empty</span></span>  <br/> |<span data-ttu-id="c49cf-173">正しくない</span><span class="sxs-lookup"><span data-stu-id="c49cf-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="c49cf-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="c49cf-174">See also</span></span>

- <span data-ttu-id="c49cf-175">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="c49cf-175">[FindFolder operation](findfolder-operation.md)</span></span>
- [<span data-ttu-id="c49cf-176">フォルダーの検索</span><span class="sxs-lookup"><span data-stu-id="c49cf-176">Finding Folders</span></span>](https://msdn.microsoft.com/library/9124d868-017a-43f0-b915-5c0082cacec9%28Office.15%29.aspx)

