---
title: DeleteFolderResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteFolderResponseMessage
api_type:
- schema
ms.assetid: de4c63ff-80b2-40c2-bc06-ef0c23beacd4
description: DeleteFolderResponseMessage 要素には、1つの DeleteFolder 操作要求の状態と結果が含まれています。
ms.openlocfilehash: 6c593e0d6e8820452bb27a6baa569980e329ef10
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44455738"
---
# <a name="deletefolderresponsemessage"></a><span data-ttu-id="5c7a2-103">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5c7a2-103">DeleteFolderResponseMessage</span></span>

<span data-ttu-id="5c7a2-104">**DeleteFolderResponseMessage**要素には、1つの[deletefolder 操作](deletefolder-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-104">The **DeleteFolderResponseMessage** element contains the status and result of a single [DeleteFolder operation](deletefolder-operation.md) request.</span></span> 
  
- [<span data-ttu-id="5c7a2-105">DeleteFolderResponse</span><span class="sxs-lookup"><span data-stu-id="5c7a2-105">DeleteFolderResponse</span></span>](deletefolderresponse.md)  
- [<span data-ttu-id="5c7a2-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5c7a2-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="5c7a2-107">DeleteFolderResponseMessage</span><span class="sxs-lookup"><span data-stu-id="5c7a2-107">DeleteFolderResponseMessage</span></span>](deletefolderresponsemessage.md)
  
```xml
<DeleteFolderResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteFolderResponseMessage>
```

 <span data-ttu-id="5c7a2-108">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="5c7a2-108">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="5c7a2-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="5c7a2-109">Attributes and elements</span></span>

<span data-ttu-id="5c7a2-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="5c7a2-111">属性</span><span class="sxs-lookup"><span data-stu-id="5c7a2-111">Attributes</span></span>

|<span data-ttu-id="5c7a2-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="5c7a2-112">**Attribute**</span></span>|<span data-ttu-id="5c7a2-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="5c7a2-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5c7a2-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="5c7a2-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="5c7a2-115">[Deletefolder 操作](deletefolder-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-115">Describes the status of a [DeleteFolder operation](deletefolder-operation.md) response.</span></span><br/><br/><span data-ttu-id="5c7a2-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="5c7a2-117">-成功</span><span class="sxs-lookup"><span data-stu-id="5c7a2-117">-  Success</span></span>  <br/><span data-ttu-id="5c7a2-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="5c7a2-118">-  Warning</span></span>  <br/><span data-ttu-id="5c7a2-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="5c7a2-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="5c7a2-120">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="5c7a2-120">ResponseClass attribute values</span></span>

|<span data-ttu-id="5c7a2-121">**値**</span><span class="sxs-lookup"><span data-stu-id="5c7a2-121">**Value**</span></span>|<span data-ttu-id="5c7a2-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="5c7a2-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="5c7a2-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="5c7a2-123">**Success**</span></span> <br/> |<span data-ttu-id="5c7a2-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="5c7a2-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="5c7a2-125">**Warning**</span></span> <br/> | <span data-ttu-id="5c7a2-126">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-126">Describes a request that was not processed.</span></span> <span data-ttu-id="5c7a2-127">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="5c7a2-128">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="5c7a2-129">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-129">- The Exchange store goes offline during the batch.</span></span><br/><span data-ttu-id="5c7a2-130">-Active Directory ドメインサービス (AD DS) はオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-130">- Active Directory Domain Services (AD DS) goes offline.</span></span><br/><span data-ttu-id="5c7a2-131">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-131">- Mailboxes are moved.</span></span><br/><span data-ttu-id="5c7a2-132">-メッセージデータベース (MDB) はオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-132">- The message database (MDB) goes offline.</span></span><br/><span data-ttu-id="5c7a2-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-133">- A password is expired.</span></span><br/><span data-ttu-id="5c7a2-134">-クォータが上限を超えています。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-134">- A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="5c7a2-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="5c7a2-135">**Error**</span></span> <br/> | <span data-ttu-id="5c7a2-136">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="5c7a2-137">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="5c7a2-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="5c7a2-138">- Invalid attributes or elements</span></span><br/><span data-ttu-id="5c7a2-139">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="5c7a2-139">- Attributes or elements out of range</span></span><br/><span data-ttu-id="5c7a2-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="5c7a2-140">- Unknown tag</span></span><br/><span data-ttu-id="5c7a2-141">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="5c7a2-141">- Attribute or element not valid in the context</span></span><br/><span data-ttu-id="5c7a2-142">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="5c7a2-142">- Unauthorized access attempt by any client</span></span><br/><span data-ttu-id="5c7a2-143">-有効なクライアント側の呼び出しに応答した場合のサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="5c7a2-143">- Server-side failure in response to a valid client-side call</span></span>  <br/><br/>  <span data-ttu-id="5c7a2-144">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-144">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="5c7a2-145">子要素</span><span class="sxs-lookup"><span data-stu-id="5c7a2-145">Child elements</span></span>

|<span data-ttu-id="5c7a2-146">**Element**</span><span class="sxs-lookup"><span data-stu-id="5c7a2-146">**Element**</span></span>|<span data-ttu-id="5c7a2-147">**説明**</span><span class="sxs-lookup"><span data-stu-id="5c7a2-147">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c7a2-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="5c7a2-148">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="5c7a2-149">応答の状態のテキストの説明。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-149">A text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="5c7a2-150">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="5c7a2-150">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="5c7a2-151">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-151">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="5c7a2-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="5c7a2-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="5c7a2-153">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-153">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="5c7a2-154">値0が含まれています。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-154">It contains the value of 0.</span></span>  <br/> |
|[<span data-ttu-id="5c7a2-155">MessageXml</span><span class="sxs-lookup"><span data-stu-id="5c7a2-155">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="5c7a2-156">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-156">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="5c7a2-157">親要素</span><span class="sxs-lookup"><span data-stu-id="5c7a2-157">Parent elements</span></span>

|<span data-ttu-id="5c7a2-158">**要素**</span><span class="sxs-lookup"><span data-stu-id="5c7a2-158">**Element**</span></span>|<span data-ttu-id="5c7a2-159">**説明**</span><span class="sxs-lookup"><span data-stu-id="5c7a2-159">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="5c7a2-160">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="5c7a2-160">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="5c7a2-161">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-161">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="5c7a2-162">注釈</span><span class="sxs-lookup"><span data-stu-id="5c7a2-162">Remarks</span></span>

<span data-ttu-id="5c7a2-163">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="5c7a2-163">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="5c7a2-164">要素の情報</span><span class="sxs-lookup"><span data-stu-id="5c7a2-164">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="5c7a2-165">Namespace</span><span class="sxs-lookup"><span data-stu-id="5c7a2-165">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="5c7a2-166">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="5c7a2-166">Schema Name</span></span>  <br/> |<span data-ttu-id="5c7a2-167">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="5c7a2-167">Messages schema</span></span>  <br/> |
|<span data-ttu-id="5c7a2-168">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="5c7a2-168">Validation File</span></span>  <br/> |<span data-ttu-id="5c7a2-169">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="5c7a2-169">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="5c7a2-170">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="5c7a2-170">Can be Empty</span></span>  <br/> |<span data-ttu-id="5c7a2-171">正しくない</span><span class="sxs-lookup"><span data-stu-id="5c7a2-171">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5c7a2-172">関連項目</span><span class="sxs-lookup"><span data-stu-id="5c7a2-172">See also</span></span>

- [<span data-ttu-id="5c7a2-173">DeleteFolder 操作</span><span class="sxs-lookup"><span data-stu-id="5c7a2-173">DeleteFolder operation</span></span>](deletefolder-operation.md)
- [<span data-ttu-id="5c7a2-174">Exchange 用 EWS リファレンス</span><span class="sxs-lookup"><span data-stu-id="5c7a2-174">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="5c7a2-175">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="5c7a2-175">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="5c7a2-176">フォルダーの削除</span><span class="sxs-lookup"><span data-stu-id="5c7a2-176">Deleting Folders</span></span>](https://msdn.microsoft.com/library/1958add5-5071-4239-adb2-40f7a7d74aee%28Office.15%29.aspx)

