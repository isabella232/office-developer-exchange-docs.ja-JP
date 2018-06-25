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
description: DeleteItemResponseMessage 要素には、状態および 1 つの DeleteItem 操作要求の結果が含まれています。
ms.openlocfilehash: 1f0cc3d49bfa5fba6da32cf65df6b6718ccfbded
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759997"
---
# <a name="deleteitemresponsemessage"></a><span data-ttu-id="32eba-103">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="32eba-103">DeleteItemResponseMessage</span></span>

<span data-ttu-id="32eba-104">**DeleteItemResponseMessage**要素には、状態および 1 つの結果が含まれている[DeleteItem の操作](deleteitem-operation.md)を要求します。</span><span class="sxs-lookup"><span data-stu-id="32eba-104">The **DeleteItemResponseMessage** element contains the status and result of a single [DeleteItem operation](deleteitem-operation.md) request.</span></span> 
  
- [<span data-ttu-id="32eba-105">DeleteItemResponse</span><span class="sxs-lookup"><span data-stu-id="32eba-105">DeleteItemResponse</span></span>](deleteitemresponse.md) 
- [<span data-ttu-id="32eba-106">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="32eba-106">ResponseMessages</span></span>](responsemessages.md)  
- [<span data-ttu-id="32eba-107">DeleteItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="32eba-107">DeleteItemResponseMessage</span></span>](deleteitemresponsemessage.md)
  
```xml
<DeleteItemResponseMessage>
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</DeleteItemResponseMessage>
```

 <span data-ttu-id="32eba-108">**DeleteItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="32eba-108">**DeleteItemResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="32eba-109">属性および要素</span><span class="sxs-lookup"><span data-stu-id="32eba-109">Attributes and elements</span></span>

<span data-ttu-id="32eba-110">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="32eba-110">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="32eba-111">属性</span><span class="sxs-lookup"><span data-stu-id="32eba-111">Attributes</span></span>

|<span data-ttu-id="32eba-112">**属性**</span><span class="sxs-lookup"><span data-stu-id="32eba-112">**Attribute**</span></span>|<span data-ttu-id="32eba-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="32eba-113">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="32eba-114">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="32eba-114">**ResponseClass**</span></span> <br/> | <span data-ttu-id="32eba-115">[DeleteItem 操作](deleteitem-operation.md)の応答のステータスについて説明します。</span><span class="sxs-lookup"><span data-stu-id="32eba-115">Describes the status of a [DeleteItem operation](deleteitem-operation.md) response.</span></span><br/><br/><span data-ttu-id="32eba-116">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="32eba-116">The following values are valid for this attribute:</span></span><br/><br/><span data-ttu-id="32eba-117">-成功</span><span class="sxs-lookup"><span data-stu-id="32eba-117">- Success</span></span>  <br/><span data-ttu-id="32eba-118">-警告</span><span class="sxs-lookup"><span data-stu-id="32eba-118">-  Warning</span></span>  <br/><span data-ttu-id="32eba-119">-エラー</span><span class="sxs-lookup"><span data-stu-id="32eba-119">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute"></a><span data-ttu-id="32eba-120">ResponseClass 属性</span><span class="sxs-lookup"><span data-stu-id="32eba-120">ResponseClass attribute</span></span>

|<span data-ttu-id="32eba-121">**値**</span><span class="sxs-lookup"><span data-stu-id="32eba-121">**Value**</span></span>|<span data-ttu-id="32eba-122">**説明**</span><span class="sxs-lookup"><span data-stu-id="32eba-122">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="32eba-123">**Success**</span><span class="sxs-lookup"><span data-stu-id="32eba-123">**Success**</span></span> <br/> |<span data-ttu-id="32eba-124">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="32eba-124">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="32eba-125">**Warning**</span><span class="sxs-lookup"><span data-stu-id="32eba-125">**Warning**</span></span> <br/> | <span data-ttu-id="32eba-126">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="32eba-126">Describes a request that was not processed.</span></span> <span data-ttu-id="32eba-127">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="32eba-127">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span><br/><br/><span data-ttu-id="32eba-128">警告の送信元の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="32eba-128">The following are examples of sources of warnings:</span></span><br/><br/><span data-ttu-id="32eba-129">-Exchange ストアは、バッチの中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="32eba-129">-  The Exchange store goes offline during the batch.</span></span>  <br/><span data-ttu-id="32eba-130">-Active Directory ドメイン サービス (AD DS) がオフラインになった。</span><span class="sxs-lookup"><span data-stu-id="32eba-130">-  Active Directory Domain Services (AD DS) goes offline.</span></span>  <br/><span data-ttu-id="32eba-131">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="32eba-131">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="32eba-132">-メッセージ データベース (MDB) がオフラインになった。</span><span class="sxs-lookup"><span data-stu-id="32eba-132">-  The message database (MDB) goes offline.</span></span>  <br/><span data-ttu-id="32eba-133">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="32eba-133">-  A password is expired.</span></span>  <br/><span data-ttu-id="32eba-134">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="32eba-134">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="32eba-135">**Error**</span><span class="sxs-lookup"><span data-stu-id="32eba-135">**Error**</span></span> <br/> | <span data-ttu-id="32eba-136">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="32eba-136">Describes a request that cannot be fulfilled.</span></span><br/><br/><span data-ttu-id="32eba-137">次に、エラーのソースの例を示します。</span><span class="sxs-lookup"><span data-stu-id="32eba-137">The following are examples of sources of errors:</span></span><br/><br/><span data-ttu-id="32eba-138">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="32eba-138">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="32eba-139">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="32eba-139">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="32eba-140">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="32eba-140">-  Unknown tag</span></span>  <br/><span data-ttu-id="32eba-141">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="32eba-141">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="32eba-142">-クライアントが、管理者によって許可されている最大レベルよりも上のエラーのログ出力レベルを設定しようとしています。</span><span class="sxs-lookup"><span data-stu-id="32eba-142">-  A client attempt to set the error logging level above the maximum level that is permitted by the administrator</span></span>  <br/><span data-ttu-id="32eba-143">-クライアントが、管理者によって指定されている既定のレベル以下のエラーの重大度レベルを設定しようとしています。</span><span class="sxs-lookup"><span data-stu-id="32eba-143">-  A client attempt to set the severity failure level below the default level that is specified by the administrator</span></span>  <br/><span data-ttu-id="32eba-144">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="32eba-144">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="32eba-145">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="32eba-145">-  Server-side failure in response to a valid client-side call</span></span><br/><br/>  <span data-ttu-id="32eba-146">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="32eba-146">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="32eba-147">子要素</span><span class="sxs-lookup"><span data-stu-id="32eba-147">Child elements</span></span>

|<span data-ttu-id="32eba-148">**要素**</span><span class="sxs-lookup"><span data-stu-id="32eba-148">**Element**</span></span>|<span data-ttu-id="32eba-149">**説明**</span><span class="sxs-lookup"><span data-stu-id="32eba-149">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32eba-150">MessageText</span><span class="sxs-lookup"><span data-stu-id="32eba-150">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="32eba-151">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="32eba-151">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="32eba-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="32eba-152">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="32eba-153">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="32eba-153">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="32eba-154">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="32eba-154">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="32eba-155">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="32eba-155">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="32eba-156">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="32eba-156">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="32eba-157">MessageXml</span><span class="sxs-lookup"><span data-stu-id="32eba-157">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="32eba-158">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="32eba-158">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="32eba-159">親要素</span><span class="sxs-lookup"><span data-stu-id="32eba-159">Parent elements</span></span>

|<span data-ttu-id="32eba-160">**要素**</span><span class="sxs-lookup"><span data-stu-id="32eba-160">**Element**</span></span>|<span data-ttu-id="32eba-161">**説明**</span><span class="sxs-lookup"><span data-stu-id="32eba-161">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="32eba-162">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="32eba-162">ResponseMessages</span></span>](responsemessages.md) <br/> |<span data-ttu-id="32eba-163">Exchange Web サービス要求に対する応答メッセージが含まれています。</span><span class="sxs-lookup"><span data-stu-id="32eba-163">Contains the response messages for an Exchange Web Services request.</span></span>  <br/> |
   
## <a name="remarks"></a><span data-ttu-id="32eba-164">備考</span><span class="sxs-lookup"><span data-stu-id="32eba-164">Remarks</span></span>

<span data-ttu-id="32eba-165">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="32eba-165">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2010 that has the Client Access server role installed.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="32eba-166">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="32eba-166">Version differences</span></span>

<span data-ttu-id="32eba-167">Exchange のビルド 15.00.0986.00 以降のバージョンでは、 **DeleteItemResponseMessage**要素は型**DeleteItemResponseMessageType**のです。</span><span class="sxs-lookup"><span data-stu-id="32eba-167">In versions of Exchange starting with build 15.00.0986.00, the **DeleteItemResponseMessage** element is of type **DeleteItemResponseMessageType**.</span></span> <span data-ttu-id="32eba-168">以前のバージョンでは、型**ResponseMessageType**の要素です。</span><span class="sxs-lookup"><span data-stu-id="32eba-168">In previous versions, the element is of type **ResponseMessageType**.</span></span>
  
## <a name="element-information"></a><span data-ttu-id="32eba-169">要素情報</span><span class="sxs-lookup"><span data-stu-id="32eba-169">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="32eba-170">名前空間</span><span class="sxs-lookup"><span data-stu-id="32eba-170">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="32eba-171">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="32eba-171">Schema Name</span></span>  <br/> |<span data-ttu-id="32eba-172">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="32eba-172">Messages schema</span></span>  <br/> |
|<span data-ttu-id="32eba-173">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="32eba-173">Validation File</span></span>  <br/> |<span data-ttu-id="32eba-174">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="32eba-174">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="32eba-175">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="32eba-175">Can be Empty</span></span>  <br/> |<span data-ttu-id="32eba-176">False</span><span class="sxs-lookup"><span data-stu-id="32eba-176">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="32eba-177">関連項目</span><span class="sxs-lookup"><span data-stu-id="32eba-177">See also</span></span>

- [<span data-ttu-id="32eba-178">DeleteItem の操作</span><span class="sxs-lookup"><span data-stu-id="32eba-178">DeleteItem operation</span></span>](deleteitem-operation.md)
- <span data-ttu-id="32eba-179">
  [Exchange 用 EWS リファレンス](ews-reference-for-exchange.md)</span><span class="sxs-lookup"><span data-stu-id="32eba-179">[EWS reference for Exchange](ews-reference-for-exchange.md)</span></span>
- [<span data-ttu-id="32eba-180">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="32eba-180">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)
- [<span data-ttu-id="32eba-181">(Exchange Web サービス) の項目の削除</span><span class="sxs-lookup"><span data-stu-id="32eba-181">Deleting Items (Exchange Web Services)</span></span>](http://msdn.microsoft.com/library/9bfc39e6-d944-4eb6-8aee-cbaf1e37c67d%28Office.15%29.aspx)

