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
description: CopyFolderResponseMessage 要素には、1つの CopyFolder 操作要求の状態と結果が含まれています。
ms.openlocfilehash: 796ec57116e4b4943ca370e45cf0abefe7782c08
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458510"
---
# <a name="copyfolderresponsemessage"></a><span data-ttu-id="445db-103">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="445db-103">CopyFolderResponseMessage</span></span>

<span data-ttu-id="445db-104">**CopyFolderResponseMessage**要素には、1つの[copyfolder 操作](copyfolder-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="445db-104">The **CopyFolderResponseMessage** element contains the status and result of a single [CopyFolder operation](copyfolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="445db-105">CopyFolderResponse</span><span class="sxs-lookup"><span data-stu-id="445db-105">CopyFolderResponse</span></span>](copyfolderresponse.md) 
- [<span data-ttu-id="445db-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="445db-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="445db-107">CopyFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="445db-107">CopyFolderResponseMessage</span></span>](copyfolderresponsemessage.md)
  
```xml
<CopyFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
   <Folders/>
</CopyFolderResponseMessage>
```

 <span data-ttu-id="445db-108">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="445db-108">**FolderInfoResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="445db-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="445db-109">Attributes and elements</span></span>

<span data-ttu-id="445db-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="445db-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="445db-111">属性</span><span class="sxs-lookup"><span data-stu-id="445db-111">Attributes</span></span>

|<span data-ttu-id="445db-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="445db-112">**Attribute**</span></span>|<span data-ttu-id="445db-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="445db-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="445db-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="445db-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="445db-115">[Copyfolder 操作](copyfolder-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="445db-115">Describes the status of a [CopyFolder operation](copyfolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="445db-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="445db-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="445db-117">-成功</span><span class="sxs-lookup"><span data-stu-id="445db-117">- Success</span></span>  <br/><span data-ttu-id="445db-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="445db-118">-  Warning</span></span>  <br/><span data-ttu-id="445db-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="445db-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="445db-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="445db-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="445db-121">**値**</span><span class="sxs-lookup"><span data-stu-id="445db-121">**Value**</span></span>|<span data-ttu-id="445db-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="445db-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="445db-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="445db-123">**Success**</span></span> <br/> |<span data-ttu-id="445db-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="445db-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="445db-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="445db-125">**Warning**</span></span> <br/> | <span data-ttu-id="445db-126">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="445db-126">Describes a request that was not processed.</span></span> <span data-ttu-id="445db-127">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="445db-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="445db-128">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="445db-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="445db-129">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="445db-129">- The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="445db-130">-Active Directory ドメインサービス (AD DS) はオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="445db-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="445db-131">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="445db-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="445db-132">-メッセージデータベース (MDB) はオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="445db-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="445db-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="445db-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="445db-134">-クォータが上限を超えています。</span><span class="sxs-lookup"><span data-stu-id="445db-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="445db-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="445db-135">**Error**</span></span> <br/> | <span data-ttu-id="445db-136">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="445db-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="445db-137">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="445db-137">The following are examples of sources of errors:</span></span>  <br/><br/><span data-ttu-id="445db-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="445db-138">- Invalid attributes or elements</span></span>  <br/><span data-ttu-id="445db-139">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="445db-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="445db-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="445db-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="445db-141">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="445db-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="445db-142">-クライアントによる権限のないアクセスの試行</span><span class="sxs-lookup"><span data-stu-id="445db-142">-  Unauthorized access attempted by any client</span></span>  <br/><span data-ttu-id="445db-143">-有効なクライアント側の呼び出しに応答した場合のサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="445db-143">-  Server-side failure in response to a valid client-side call</span></span><br/><br/><span data-ttu-id="445db-144">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="445db-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="445db-145">子要素</span><span class="sxs-lookup"><span data-stu-id="445db-145">Child elements</span></span>

|<span data-ttu-id="445db-146">**Element**</span><span class="sxs-lookup"><span data-stu-id="445db-146">**Element**</span></span>|<span data-ttu-id="445db-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="445db-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="445db-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="445db-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="445db-149">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="445db-149">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="445db-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="445db-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="445db-151">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="445db-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="445db-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="445db-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="445db-153">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="445db-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="445db-154">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="445db-154">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="445db-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="445db-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="445db-156">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="445db-156">Provides additional error response information.</span></span>  <br/> |
|[<span data-ttu-id="445db-157">フォルダー</span><span class="sxs-lookup"><span data-stu-id="445db-157">Folders</span></span>](folders-ex15websvcsotherref.md) <br/> |<span data-ttu-id="445db-158">コピーされたフォルダーの配列を格納します。</span><span class="sxs-lookup"><span data-stu-id="445db-158">Contains an array of copied folders.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="445db-159">親要素</span><span class="sxs-lookup"><span data-stu-id="445db-159">Parent elements</span></span>

|<span data-ttu-id="445db-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="445db-160">**Element**</span></span>|<span data-ttu-id="445db-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="445db-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="445db-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="445db-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="445db-163">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="445db-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="445db-164">注釈</span><span class="sxs-lookup"><span data-stu-id="445db-164">Remarks</span></span>

<span data-ttu-id="445db-165">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="445db-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="445db-166">要素の情報</span><span class="sxs-lookup"><span data-stu-id="445db-166">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="445db-167">Namespace</span><span class="sxs-lookup"><span data-stu-id="445db-167">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="445db-168">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="445db-168">Schema name</span></span>  <br/> |<span data-ttu-id="445db-169">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="445db-169">Messages schema</span></span>  <br/> |
|<span data-ttu-id="445db-170">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="445db-170">Validation file</span></span>  <br/> |<span data-ttu-id="445db-171">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="445db-171">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="445db-172">空にすることができます。</span><span class="sxs-lookup"><span data-stu-id="445db-172">Can be empty</span></span>  <br/> |<span data-ttu-id="445db-173">正しくない</span><span class="sxs-lookup"><span data-stu-id="445db-173">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="445db-174">関連項目</span><span class="sxs-lookup"><span data-stu-id="445db-174">See also</span></span>

- [<span data-ttu-id="445db-175">CopyFolder 操作</span><span class="sxs-lookup"><span data-stu-id="445db-175">CopyFolder operation</span></span>](copyfolder-operation.md)
- [<span data-ttu-id="445db-176">Exchange 用 EWS リファレンス</span><span class="sxs-lookup"><span data-stu-id="445db-176">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md) 
- [<span data-ttu-id="445db-177">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="445db-177">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

