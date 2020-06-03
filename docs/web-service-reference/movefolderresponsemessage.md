---
title: MoveFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- MoveFolderResponseMessage
api_type:
- schema
ms.assetid: 54917251-96af-44c2-ae90-d545f0a16e2e
description: MoveFolderResponseMessage 要素には、1つの MoveFolder 操作要求の状態と結果が含まれています。
ms.openlocfilehash: 634fec89445b49d1c8c42541f2fc50d07b5a1acd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467474"
---
# <a name="movefolderresponsemessage"></a><span data-ttu-id="28739-103">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="28739-103">MoveFolderResponseMessage</span></span>

<span data-ttu-id="28739-104">**MoveFolderResponseMessage**要素には、1つの[movefolder 操作](movefolder-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="28739-104">The **MoveFolderResponseMessage** element contains the status and result of a single [MoveFolder operation](movefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="28739-105">MoveFolderResponse</span><span class="sxs-lookup"><span data-stu-id="28739-105">MoveFolderResponse</span></span>](movefolderresponse.md)
- [<span data-ttu-id="28739-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="28739-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="28739-107">MoveFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="28739-107">MoveFolderResponseMessage</span></span>](movefolderresponsemessage.md)
  
```xml
<MoveFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</MoveFolderResponseMessage>
```

 <span data-ttu-id="28739-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="28739-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="28739-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="28739-109">Attributes and elements</span></span>

<span data-ttu-id="28739-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="28739-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="28739-111">属性</span><span class="sxs-lookup"><span data-stu-id="28739-111">Attributes</span></span>

|<span data-ttu-id="28739-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="28739-112">**Attribute**</span></span>|<span data-ttu-id="28739-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="28739-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="28739-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="28739-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="28739-115">[Movefolder 操作](movefolder-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="28739-115">Describes the status of a [MoveFolder operation](movefolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="28739-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="28739-116">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="28739-117">-成功</span><span class="sxs-lookup"><span data-stu-id="28739-117">-  Success</span></span>  <br/><span data-ttu-id="28739-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="28739-118">-  Warning</span></span>  <br/><span data-ttu-id="28739-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="28739-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="28739-120">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="28739-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="28739-121">**値**</span><span class="sxs-lookup"><span data-stu-id="28739-121">**Value**</span></span>|<span data-ttu-id="28739-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="28739-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="28739-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="28739-123">**Success**</span></span> <br/> |<span data-ttu-id="28739-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="28739-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="28739-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="28739-125">**Warning**</span></span> <br/> | <span data-ttu-id="28739-126">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="28739-126">Describes a request that was not processed.</span></span> <span data-ttu-id="28739-127">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="28739-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/> <span data-ttu-id="28739-128">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="28739-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="28739-129">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="28739-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="28739-130">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="28739-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="28739-131">-メールボックスが移動されました。</span><span class="sxs-lookup"><span data-stu-id="28739-131">-  Mailboxes were moved.</span></span>  <br/><span data-ttu-id="28739-132">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="28739-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="28739-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="28739-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="28739-134">-クォータを超過しました。</span><span class="sxs-lookup"><span data-stu-id="28739-134">-  A quota was exceeded.</span></span>  <br/> |
|<span data-ttu-id="28739-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="28739-135">**Error**</span></span> <br/> | <span data-ttu-id="28739-136">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="28739-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="28739-137">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="28739-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="28739-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="28739-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="28739-139">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="28739-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="28739-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="28739-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="28739-141">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="28739-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="28739-142">-クライアントによる承認されていないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="28739-142">-  Any unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="28739-143">-有効なクライアント側の呼び出しに応答して、サーバー側で障害が発生した</span><span class="sxs-lookup"><span data-stu-id="28739-143">-  Any server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="28739-144">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="28739-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="28739-145">子要素</span><span class="sxs-lookup"><span data-stu-id="28739-145">Child elements</span></span>

|<span data-ttu-id="28739-146">**Element**</span><span class="sxs-lookup"><span data-stu-id="28739-146">**Element**</span></span>|<span data-ttu-id="28739-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="28739-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28739-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="28739-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="28739-149">応答の状態のテキストの説明。</span><span class="sxs-lookup"><span data-stu-id="28739-149">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="28739-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="28739-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="28739-151">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="28739-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="28739-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="28739-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="28739-153">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="28739-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="28739-154">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="28739-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="28739-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="28739-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="28739-156">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="28739-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="28739-157">フォルダー</span><span class="sxs-lookup"><span data-stu-id="28739-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="28739-158">移動したフォルダーの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="28739-158">Contains an array of moved folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="28739-159">親要素</span><span class="sxs-lookup"><span data-stu-id="28739-159">Parent elements</span></span>

|<span data-ttu-id="28739-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="28739-160">**Element**</span></span>|<span data-ttu-id="28739-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="28739-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="28739-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="28739-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="28739-163">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="28739-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="28739-164">注釈</span><span class="sxs-lookup"><span data-stu-id="28739-164">Remarks</span></span>

<span data-ttu-id="28739-165">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="28739-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="28739-166">要素の情報</span><span class="sxs-lookup"><span data-stu-id="28739-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="28739-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="28739-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="28739-168">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="28739-168">Schema Name</span></span>  <br/> |<span data-ttu-id="28739-169">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="28739-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="28739-170">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="28739-170">Validation File</span></span>  <br/> |<span data-ttu-id="28739-171">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="28739-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="28739-172">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="28739-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="28739-173">正しくない</span><span class="sxs-lookup"><span data-stu-id="28739-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="28739-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="28739-174">See also</span></span>

- [<span data-ttu-id="28739-175">MoveFolder</span><span class="sxs-lookup"><span data-stu-id="28739-175">MoveFolder</span></span>](movefolder.md)
- [<span data-ttu-id="28739-176">MoveFolder 操作</span><span class="sxs-lookup"><span data-stu-id="28739-176">MoveFolder operation</span></span>](movefolder-operation.md)

