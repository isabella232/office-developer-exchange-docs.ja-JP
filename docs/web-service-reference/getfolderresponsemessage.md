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
description: GetFolderResponseMessage 要素には、1つの GetFolder 操作要求の状態と結果が含まれています。
ms.openlocfilehash: ddf23790e804c3f0562f65ebaa3cb591433eab69
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456459"
---
# <a name="getfolderresponsemessage"></a><span data-ttu-id="ea2ec-103">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ea2ec-103">GetFolderResponseMessage</span></span>

<span data-ttu-id="ea2ec-104">**GetFolderResponseMessage**要素には、1つの[getfolder 操作](getfolder-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-104">The **GetFolderResponseMessage** element contains the status and result of a single [GetFolder operation](getfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="ea2ec-105">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ea2ec-105">GetFolderResponse</span></span>](getfolderresponse.md) 
- [<span data-ttu-id="ea2ec-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ea2ec-106">ResponseMessages</span></span>](responsemessages.md)
- [<span data-ttu-id="ea2ec-107">GetFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="ea2ec-107">GetFolderResponseMessage</span></span>](getfolderresponsemessage.md)
  
```xml
<GetFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</GetFolderResponseMessage>
```

 <span data-ttu-id="ea2ec-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="ea2ec-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="ea2ec-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="ea2ec-109">Attributes and elements</span></span>

<span data-ttu-id="ea2ec-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="ea2ec-111">属性</span><span class="sxs-lookup"><span data-stu-id="ea2ec-111">Attributes</span></span>

|<span data-ttu-id="ea2ec-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="ea2ec-112">**Attribute**</span></span>|<span data-ttu-id="ea2ec-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="ea2ec-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ea2ec-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="ea2ec-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="ea2ec-115">[Getfolder 操作](getfolder-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-115">Describes the status of a [GetFolder operation](getfolder-operation.md) response.</span></span> <br/><br/><span data-ttu-id="ea2ec-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-116">The following values are valid for this attribute:</span></span><br/>  <br/><span data-ttu-id="ea2ec-117">-成功</span><span class="sxs-lookup"><span data-stu-id="ea2ec-117">-  Success</span></span>  <br/><span data-ttu-id="ea2ec-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="ea2ec-118">-  Warning</span></span>  <br/><span data-ttu-id="ea2ec-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="ea2ec-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="ea2ec-120">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="ea2ec-120">ResponseClass Attribute</span></span>

|<span data-ttu-id="ea2ec-121">**値**</span><span class="sxs-lookup"><span data-stu-id="ea2ec-121">**Value**</span></span>|<span data-ttu-id="ea2ec-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="ea2ec-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="ea2ec-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="ea2ec-123">**Success**</span></span> <br/> |<span data-ttu-id="ea2ec-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="ea2ec-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="ea2ec-125">**Warning**</span></span> <br/> | <span data-ttu-id="ea2ec-126">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-126">Describes a request that was not processed.</span></span> <span data-ttu-id="ea2ec-127">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="ea2ec-128">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-128">The following are examples of sources of warnings:</span></span>  <br/><br/><span data-ttu-id="ea2ec-129">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-129">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="ea2ec-130">-Active Directory ドメインサービス (AD DS) がオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-130">-  Active Directory Domain Services (AD DS) is offline.</span></span>  <br/><span data-ttu-id="ea2ec-131">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="ea2ec-132">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-132">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="ea2ec-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="ea2ec-134">-クォータが上限を超えています。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="ea2ec-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="ea2ec-135">**Error**</span></span> <br/> | <span data-ttu-id="ea2ec-136">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-136">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="ea2ec-137">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="ea2ec-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="ea2ec-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="ea2ec-139">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="ea2ec-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="ea2ec-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="ea2ec-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="ea2ec-141">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="ea2ec-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="ea2ec-142">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="ea2ec-142">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="ea2ec-143">-有効なクライアント側の呼び出しに応答した場合のサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="ea2ec-143">-  Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="ea2ec-144">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="ea2ec-145">子要素</span><span class="sxs-lookup"><span data-stu-id="ea2ec-145">Child elements</span></span>

|<span data-ttu-id="ea2ec-146">**Element**</span><span class="sxs-lookup"><span data-stu-id="ea2ec-146">**Element**</span></span>|<span data-ttu-id="ea2ec-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="ea2ec-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea2ec-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="ea2ec-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="ea2ec-149">応答の状態の説明をテキストで提供します。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-149">Provides text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="ea2ec-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="ea2ec-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="ea2ec-151">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="ea2ec-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="ea2ec-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="ea2ec-153">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="ea2ec-154">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="ea2ec-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="ea2ec-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="ea2ec-156">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="ea2ec-157">フォルダー</span><span class="sxs-lookup"><span data-stu-id="ea2ec-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="ea2ec-158">Folder 操作で使用されるフォルダーの配列が含まれています。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-158">Contains an array of folders that are used in folder operations.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="ea2ec-159">親要素</span><span class="sxs-lookup"><span data-stu-id="ea2ec-159">Parent elements</span></span>

|<span data-ttu-id="ea2ec-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="ea2ec-160">**Element**</span></span>|<span data-ttu-id="ea2ec-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="ea2ec-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="ea2ec-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="ea2ec-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="ea2ec-163">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="ea2ec-164">注釈</span><span class="sxs-lookup"><span data-stu-id="ea2ec-164">Remarks</span></span>

<span data-ttu-id="ea2ec-165">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="ea2ec-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="ea2ec-166">要素の情報</span><span class="sxs-lookup"><span data-stu-id="ea2ec-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="ea2ec-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="ea2ec-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="ea2ec-168">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="ea2ec-168">Schema Name</span></span>  <br/> |<span data-ttu-id="ea2ec-169">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="ea2ec-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="ea2ec-170">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="ea2ec-170">Validation File</span></span>  <br/> |<span data-ttu-id="ea2ec-171">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="ea2ec-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="ea2ec-172">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="ea2ec-172">Can be Empty</span></span>  <br/> |<span data-ttu-id="ea2ec-173">正しくない</span><span class="sxs-lookup"><span data-stu-id="ea2ec-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="ea2ec-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="ea2ec-174">See also</span></span>

- [<span data-ttu-id="ea2ec-175">GetFolder</span><span class="sxs-lookup"><span data-stu-id="ea2ec-175">GetFolder</span></span>](getfolder.md)
- [<span data-ttu-id="ea2ec-176">GetFolderResponse</span><span class="sxs-lookup"><span data-stu-id="ea2ec-176">GetFolderResponse</span></span>](getfolderresponse.md) 
- [<span data-ttu-id="ea2ec-177">GetFolder 操作</span><span class="sxs-lookup"><span data-stu-id="ea2ec-177">GetFolder operation</span></span>](getfolder-operation.md)

