---
title: DeleteItemResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- DeleteItemResponseMessage
api_type:
- schema
ms.assetid: c3d34c4d-8d83-4612-aa9e-66f9cc7314df
description: DeleteItemResponseMessage 要素には、1つの DeleteItem 操作要求の状態と結果が含まれています。
ms.openlocfilehash: 78e3efc6a9e9e6629d7efe7f2dc294e0a731005a
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526929"
---
# <a name="deleteitemresponsemessage"></a><span data-ttu-id="198c4-103">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="198c4-103">DeleteItemResponseMessage</span></span>

<span data-ttu-id="198c4-104">**DeleteItemResponseMessage**要素には、1つの[DeleteItem 操作](deleteitem-operation.md)要求の状態と結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="198c4-104">The **DeleteItemResponseMessage** element contains the status and result of a single [DeleteItem operation](deleteitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="198c4-105">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="198c4-105">DeleteItemResponse</span></span>](deleteitemresponse.md) 
- [<span data-ttu-id="198c4-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="198c4-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="198c4-107">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="198c4-107">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
  
```xml
<DeleteItemResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteItemResponseMessage>
```

 <span data-ttu-id="198c4-108">**DeleteItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="198c4-108">**DeleteItemResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="198c4-109">属性と要素</span><span class="sxs-lookup"><span data-stu-id="198c4-109">Attributes and elements</span></span>

<span data-ttu-id="198c4-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="198c4-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="198c4-111">属性</span><span class="sxs-lookup"><span data-stu-id="198c4-111">Attributes</span></span>

|<span data-ttu-id="198c4-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="198c4-112">**Attribute**</span></span>|<span data-ttu-id="198c4-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="198c4-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="198c4-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="198c4-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="198c4-115">[DeleteItem 操作](deleteitem-operation.md)の応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="198c4-115">Describes the status of a [DeleteItem operation](deleteitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="198c4-116">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="198c4-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="198c4-117">-成功</span><span class="sxs-lookup"><span data-stu-id="198c4-117">- Success</span></span>  <br/><span data-ttu-id="198c4-118">-Warning</span><span class="sxs-lookup"><span data-stu-id="198c4-118">-  Warning</span></span>  <br/><span data-ttu-id="198c4-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="198c4-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="198c4-120">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="198c4-120">ResponseClass attribute</span></span>

|<span data-ttu-id="198c4-121">**値**</span><span class="sxs-lookup"><span data-stu-id="198c4-121">**Value**</span></span>|<span data-ttu-id="198c4-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="198c4-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="198c4-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="198c4-123">**Success**</span></span> <br/> |<span data-ttu-id="198c4-124">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="198c4-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="198c4-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="198c4-125">**Warning**</span></span> <br/> | <span data-ttu-id="198c4-126">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="198c4-126">Describes a request that was not processed.</span></span> <span data-ttu-id="198c4-127">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="198c4-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="198c4-128">警告のソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="198c4-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="198c4-129">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="198c4-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="198c4-130">-Active Directory ドメインサービス (AD DS) はオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="198c4-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="198c4-131">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="198c4-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="198c4-132">-メッセージデータベース (MDB) はオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="198c4-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="198c4-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="198c4-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="198c4-134">-クォータが上限を超えています。</span><span class="sxs-lookup"><span data-stu-id="198c4-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="198c4-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="198c4-135">**Error**</span></span> <br/> | <span data-ttu-id="198c4-136">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="198c4-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="198c4-137">エラーのソースの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="198c4-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="198c4-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="198c4-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="198c4-139">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="198c4-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="198c4-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="198c4-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="198c4-141">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="198c4-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="198c4-142">-クライアントは、管理者によって許可されている最大レベル以上のエラーログ出力レベルを設定しようとしました</span><span class="sxs-lookup"><span data-stu-id="198c4-142">-  A client attempt to set the error logging level above the maximum level that is permitted by the administrator</span></span>  <br/><span data-ttu-id="198c4-143">-クライアントは、管理者によって指定された既定のレベルの下に重大度エラーレベルを設定しようとしています。</span><span class="sxs-lookup"><span data-stu-id="198c4-143">-  A client attempt to set the severity failure level below the default level that is specified by the administrator</span></span>  <br/><span data-ttu-id="198c4-144">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="198c4-144">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="198c4-145">-有効なクライアント側の呼び出しに応答した場合のサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="198c4-145">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="198c4-146">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="198c4-146">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="198c4-147">子要素</span><span class="sxs-lookup"><span data-stu-id="198c4-147">Child elements</span></span>

|<span data-ttu-id="198c4-148">**Element**</span><span class="sxs-lookup"><span data-stu-id="198c4-148">**Element**</span></span>|<span data-ttu-id="198c4-149">**説明**</span><span class="sxs-lookup"><span data-stu-id="198c4-149">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="198c4-150">MessageText</span><span class="sxs-lookup"><span data-stu-id="198c4-150">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="198c4-151">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="198c4-151">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="198c4-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="198c4-152">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="198c4-153">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="198c4-153">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="198c4-154">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="198c4-154">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="198c4-155">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="198c4-155">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="198c4-156">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="198c4-156">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="198c4-157">MessageXml</span><span class="sxs-lookup"><span data-stu-id="198c4-157">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="198c4-158">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="198c4-158">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="198c4-159">親要素</span><span class="sxs-lookup"><span data-stu-id="198c4-159">Parent elements</span></span>

|<span data-ttu-id="198c4-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="198c4-160">**Element**</span></span>|<span data-ttu-id="198c4-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="198c4-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="198c4-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="198c4-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="198c4-163">Exchange Web サービス要求に対する応答メッセージを含みます。</span><span class="sxs-lookup"><span data-stu-id="198c4-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="198c4-164">注釈</span><span class="sxs-lookup"><span data-stu-id="198c4-164">Remarks</span></span>

<span data-ttu-id="198c4-165">この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="198c4-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="198c4-166">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="198c4-166">Version differences</span></span>

<span data-ttu-id="198c4-167">Build 15.00.0986.00 以降のバージョンの Exchange では、 **DeleteItemResponseMessage**要素の型は**Deleteitemresponsemessagetype**です。</span><span class="sxs-lookup"><span data-stu-id="198c4-167">In versions of Exchange starting with build 15.00.0986.00, the **DeleteItemResponseMessage** element is of type **DeleteItemResponseMessageType**.</span></span> <span data-ttu-id="198c4-168">以前のバージョンでは、要素の種類は**Responsemessagetype**です。</span><span class="sxs-lookup"><span data-stu-id="198c4-168">In previous versions, the element is of type **ResponseMessageType**.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="198c4-169">要素の情報</span><span class="sxs-lookup"><span data-stu-id="198c4-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="198c4-170">Namespace</span><span class="sxs-lookup"><span data-stu-id="198c4-170">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="198c4-171">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="198c4-171">Schema Name</span></span>  <br/> |<span data-ttu-id="198c4-172">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="198c4-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="198c4-173">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="198c4-173">Validation File</span></span>  <br/> |<span data-ttu-id="198c4-174">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="198c4-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="198c4-175">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="198c4-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="198c4-176">正しくない</span><span class="sxs-lookup"><span data-stu-id="198c4-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="198c4-177">関連項目</span><span class="sxs-lookup"><span data-stu-id="198c4-177">See also</span></span>

- [<span data-ttu-id="198c4-178">DeleteItem 操作</span><span class="sxs-lookup"><span data-stu-id="198c4-178">DeleteItem operation</span></span>](deleteitem-operation.md)
- [<span data-ttu-id="198c4-179">Exchange 用 EWS リファレンス</span><span class="sxs-lookup"><span data-stu-id="198c4-179">EWS reference for Exchange</span></span>](ews-reference-for-exchange.md)
- [<span data-ttu-id="198c4-180">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="198c4-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="198c4-181">アイテムの削除 (Exchange Web サービス)</span><span class="sxs-lookup"><span data-stu-id="198c4-181">Deleting Items (Exchange Web Services)</span></span>](https://msdn.microsoft.com/library/9bfc39e6-d944-4eb6-8aee-cbaf1e37c67d%28Office.15%29.aspx)

