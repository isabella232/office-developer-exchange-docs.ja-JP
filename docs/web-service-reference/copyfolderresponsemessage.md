---
title: CopyFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CopyFolderResponseMessage
api_type:
- schema
ms.assetid: c82092a9-50ff-4ae1-b819-ebabbf89262b
description: CopyFolderResponseMessage 要素には、状態および 1 つの CopyFolder 操作要求の結果が含まれています。
ms.openlocfilehash: 2bb2b407e0ae6b854d214c4b9d68ac8ed65b2c7b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759781"
---
# <a name="copyfolderresponsemessage"></a><span data-ttu-id="8500c-103">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8500c-103">CopyFolderResponseMessage</span></span>

<span data-ttu-id="8500c-104">**CopyFolderResponseMessage**要素には、状態および 1 つの結果が含まれています[CopyFolder 操作](copyfolder-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="8500c-104">The **CopyFolderResponseMessage** element contains the status and result of a single [CopyFolder operation](copyfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="8500c-105">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="8500c-105">CopyFolderResponse</span></span>](copyfolderresponse.md) 
- [<span data-ttu-id="8500c-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8500c-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="8500c-107">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="8500c-107">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
  
```xml
<CopyFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CopyFolderResponseMessage>
```

 <span data-ttu-id="8500c-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="8500c-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="8500c-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="8500c-109">Attributes and elements</span></span>

<span data-ttu-id="8500c-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="8500c-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="8500c-111">属性</span><span class="sxs-lookup"><span data-stu-id="8500c-111">Attributes</span></span>

|<span data-ttu-id="8500c-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="8500c-112">**Attribute**</span></span>|<span data-ttu-id="8500c-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="8500c-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8500c-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="8500c-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="8500c-115">[CopyFolder 操作](copyfolder-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="8500c-115">Describes the status of a [CopyFolder operation](copyfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="8500c-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="8500c-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="8500c-117">-成功</span><span class="sxs-lookup"><span data-stu-id="8500c-117">- Success</span></span>  <br/><span data-ttu-id="8500c-118">-警告</span><span class="sxs-lookup"><span data-stu-id="8500c-118">-  Warning</span></span>  <br/><span data-ttu-id="8500c-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="8500c-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="8500c-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="8500c-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="8500c-121">**値**</span><span class="sxs-lookup"><span data-stu-id="8500c-121">**Value**</span></span>|<span data-ttu-id="8500c-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="8500c-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="8500c-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="8500c-123">**Success**</span></span> <br/> |<span data-ttu-id="8500c-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="8500c-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="8500c-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="8500c-125">**Warning**</span></span> <br/> | <span data-ttu-id="8500c-126">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="8500c-126">Describes a request that was not processed.</span></span> <span data-ttu-id="8500c-127">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="8500c-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="8500c-128">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="8500c-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="8500c-129">-Exchange ストアは、バッチの中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="8500c-129">- The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="8500c-130">-Active Directory ドメイン サービス (AD DS) がオフラインになった。</span><span class="sxs-lookup"><span data-stu-id="8500c-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="8500c-131">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="8500c-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="8500c-132">-メッセージ データベース (MDB) がオフラインになった。</span><span class="sxs-lookup"><span data-stu-id="8500c-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="8500c-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="8500c-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="8500c-134">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="8500c-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="8500c-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="8500c-135">**Error**</span></span> <br/> | <span data-ttu-id="8500c-136">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="8500c-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="8500c-137">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="8500c-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="8500c-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="8500c-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="8500c-139">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="8500c-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="8500c-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="8500c-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="8500c-141">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="8500c-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="8500c-142">-承認されていないアクセスをしようとした任意のクライアント</span><span class="sxs-lookup"><span data-stu-id="8500c-142">-  Unauthorized access attempted by any client</span></span>  <br/><span data-ttu-id="8500c-143">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="8500c-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="8500c-144">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="8500c-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="8500c-145">子要素</span><span class="sxs-lookup"><span data-stu-id="8500c-145">Child elements</span></span>

|<span data-ttu-id="8500c-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="8500c-146">**Element**</span></span>|<span data-ttu-id="8500c-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="8500c-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8500c-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="8500c-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="8500c-149">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="8500c-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="8500c-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="8500c-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="8500c-151">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="8500c-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="8500c-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="8500c-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="8500c-153">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="8500c-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="8500c-154">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8500c-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="8500c-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="8500c-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="8500c-156">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="8500c-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="8500c-157">フォルダー</span><span class="sxs-lookup"><span data-stu-id="8500c-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="8500c-158">コピーしたフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="8500c-158">Contains an array of copied folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="8500c-159">親要素</span><span class="sxs-lookup"><span data-stu-id="8500c-159">Parent elements</span></span>

|<span data-ttu-id="8500c-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="8500c-160">**Element**</span></span>|<span data-ttu-id="8500c-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="8500c-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="8500c-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="8500c-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="8500c-163">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="8500c-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="8500c-164">備考</span><span class="sxs-lookup"><span data-stu-id="8500c-164">Remarks</span></span>

<span data-ttu-id="8500c-165">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="8500c-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="8500c-166">要素情報</span><span class="sxs-lookup"><span data-stu-id="8500c-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="8500c-167">名前空間</span><span class="sxs-lookup"><span data-stu-id="8500c-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="8500c-168">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="8500c-168">Schema name</span></span>  <br/> |<span data-ttu-id="8500c-169">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="8500c-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="8500c-170">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="8500c-170">Validation file</span></span>  <br/> |<span data-ttu-id="8500c-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="8500c-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="8500c-172">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="8500c-172">Can be empty</span></span>  <br/> |<span data-ttu-id="8500c-173">False</span><span class="sxs-lookup"><span data-stu-id="8500c-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="8500c-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="8500c-174">See also</span></span>

- [<span data-ttu-id="8500c-175">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="8500c-175">CopyFolder operation</span></span>](copyfolder-operation.md)
- <span data-ttu-id="8500c-176">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="8500c-176">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span> 
- [<span data-ttu-id="8500c-177">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="8500c-177">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

