---
title: GetFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetFolderResponseMessage
api_type:
- schema
ms.assetid: 51359863-d110-4c12-b89f-aba5e3e40c1d
description: GetFolderResponseMessage 要素には、状態および 1 つの GetFolder 操作要求の結果が含まれています。
ms.openlocfilehash: a6b67907dba311a3ce482ff8f524378fb4be9694
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760740"
---
# <a name="getfolderresponsemessage"></a><span data-ttu-id="5ee53-103">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5ee53-103">GetFolderResponseMessage</span></span>

<span data-ttu-id="5ee53-104">**GetFolderResponseMessage**要素には、状態および 1 つの結果が含まれている[GetFolder の操作](getfolder-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="5ee53-104">The **GetFolderResponseMessage** element contains the status and result of a single [GetFolder operation](getfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="5ee53-105">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="5ee53-105">GetFolderResponse</span></span>](getfolderresponse.md) 
- [<span data-ttu-id="5ee53-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5ee53-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="5ee53-107">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5ee53-107">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
  
```xml
<GetFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</GetFolderResponseMessage>
```

 <span data-ttu-id="5ee53-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="5ee53-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5ee53-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="5ee53-109">Attributes and elements</span></span>

<span data-ttu-id="5ee53-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5ee53-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5ee53-111">属性</span><span class="sxs-lookup"><span data-stu-id="5ee53-111">Attributes</span></span>

|<span data-ttu-id="5ee53-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="5ee53-112">**Attribute**</span></span>|<span data-ttu-id="5ee53-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="5ee53-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5ee53-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="5ee53-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="5ee53-115">[GetFolder の操作](getfolder-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="5ee53-115">Describes the status of a [GetFolder operation](getfolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="5ee53-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="5ee53-116">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="5ee53-117">-成功</span><span class="sxs-lookup"><span data-stu-id="5ee53-117">-  Success</span></span>  <br/><span data-ttu-id="5ee53-118">-警告</span><span class="sxs-lookup"><span data-stu-id="5ee53-118">-  Warning</span></span>  <br/><span data-ttu-id="5ee53-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="5ee53-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="5ee53-120">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="5ee53-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="5ee53-121">**値**</span><span class="sxs-lookup"><span data-stu-id="5ee53-121">**Value**</span></span>|<span data-ttu-id="5ee53-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="5ee53-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5ee53-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="5ee53-123">**Success**</span></span> <br/> |<span data-ttu-id="5ee53-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="5ee53-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="5ee53-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="5ee53-125">**Warning**</span></span> <br/> | <span data-ttu-id="5ee53-126">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="5ee53-126">Describes a request that was not processed.</span></span> <span data-ttu-id="5ee53-127">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="5ee53-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="5ee53-128">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5ee53-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="5ee53-129">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="5ee53-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="5ee53-130">-Active Directory ドメイン サービス (AD DS) では、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="5ee53-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="5ee53-131">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="5ee53-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="5ee53-132">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="5ee53-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="5ee53-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="5ee53-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="5ee53-134">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="5ee53-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="5ee53-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="5ee53-135">**Error**</span></span> <br/> | <span data-ttu-id="5ee53-136">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="5ee53-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="5ee53-137">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="5ee53-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="5ee53-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="5ee53-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="5ee53-139">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="5ee53-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="5ee53-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="5ee53-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="5ee53-141">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="5ee53-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="5ee53-142">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="5ee53-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="5ee53-143">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="5ee53-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="5ee53-144">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="5ee53-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5ee53-145">子要素</span><span class="sxs-lookup"><span data-stu-id="5ee53-145">Child elements</span></span>

|<span data-ttu-id="5ee53-146">**要素**</span><span class="sxs-lookup"><span data-stu-id="5ee53-146">**Element**</span></span>|<span data-ttu-id="5ee53-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="5ee53-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ee53-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="5ee53-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="5ee53-149">応答のステータスの説明テキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="5ee53-149">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="5ee53-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5ee53-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="5ee53-151">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="5ee53-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="5ee53-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5ee53-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="5ee53-153">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="5ee53-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="5ee53-154">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5ee53-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="5ee53-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="5ee53-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="5ee53-156">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="5ee53-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="5ee53-157">フォルダー</span><span class="sxs-lookup"><span data-stu-id="5ee53-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="5ee53-158">フォルダーの操作で使用されているフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5ee53-158">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5ee53-159">親要素</span><span class="sxs-lookup"><span data-stu-id="5ee53-159">Parent elements</span></span>

|<span data-ttu-id="5ee53-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="5ee53-160">**Element**</span></span>|<span data-ttu-id="5ee53-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="5ee53-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5ee53-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5ee53-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="5ee53-163">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="5ee53-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5ee53-164">備考</span><span class="sxs-lookup"><span data-stu-id="5ee53-164">Remarks</span></span>

<span data-ttu-id="5ee53-165">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="5ee53-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5ee53-166">要素情報</span><span class="sxs-lookup"><span data-stu-id="5ee53-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5ee53-167">名前空間</span><span class="sxs-lookup"><span data-stu-id="5ee53-167">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5ee53-168">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5ee53-168">Schema Name</span></span>  <br/> |<span data-ttu-id="5ee53-169">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="5ee53-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5ee53-170">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5ee53-170">Validation File</span></span>  <br/> |<span data-ttu-id="5ee53-171">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="5ee53-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5ee53-172">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5ee53-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="5ee53-173">False</span><span class="sxs-lookup"><span data-stu-id="5ee53-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5ee53-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="5ee53-174">See also</span></span>

- [<span data-ttu-id="5ee53-175">GetFolder</span><span class="sxs-lookup"><span data-stu-id="5ee53-175">GetFolder</span></span>](getfolder.md)
- [<span data-ttu-id="5ee53-176">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="5ee53-176">GetFolderResponse</span></span>](getfolderresponse.md) 
- <span data-ttu-id="5ee53-177">
  [GetFolder 操作](getfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="5ee53-177">[GetFolder operation](getfolder-operation.md)</span></span>

