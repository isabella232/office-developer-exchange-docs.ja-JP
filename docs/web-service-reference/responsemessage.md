---
title: ResponseMessage
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ResponseMessage
api_type:
- schema
ms.assetid: bf57265a-d354-4cd7-bbfc-d93e19cbede6
description: ResponseMessage 要素は、要求内の単一のエンティティの応答ステータスに関する説明情報を提供します。
ms.openlocfilehash: 69f1f6f12d10044045b72dd644536e742c479b9e
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833191"
---
# <a name="responsemessage"></a><span data-ttu-id="3aa05-103">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="3aa05-103">ResponseMessage</span></span>

<span data-ttu-id="3aa05-104">**ResponseMessage**要素は、要求内の単一のエンティティの応答ステータスに関する説明情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="3aa05-104">The **ResponseMessage** element provides descriptive information about the response status for a single entity within a request.</span></span> 
  
```xml
<ResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ResponseMessage>
```

 <span data-ttu-id="3aa05-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3aa05-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="3aa05-106">属性および要素</span><span class="sxs-lookup"><span data-stu-id="3aa05-106">Attributes and elements</span></span>

<span data-ttu-id="3aa05-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="3aa05-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="3aa05-108">属性</span><span class="sxs-lookup"><span data-stu-id="3aa05-108">Attributes</span></span>

|<span data-ttu-id="3aa05-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="3aa05-109">**Attribute**</span></span>|<span data-ttu-id="3aa05-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="3aa05-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3aa05-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="3aa05-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="3aa05-112">応答のステータスを表します。</span><span class="sxs-lookup"><span data-stu-id="3aa05-112">Represents the status of the response.</span></span> <br/><br/><span data-ttu-id="3aa05-113">次の値は、この属性の有効です。</span><span class="sxs-lookup"><span data-stu-id="3aa05-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="3aa05-114">-成功</span><span class="sxs-lookup"><span data-stu-id="3aa05-114">-  Success</span></span>  <br/><span data-ttu-id="3aa05-115">-警告</span><span class="sxs-lookup"><span data-stu-id="3aa05-115">-  Warning</span></span>  <br/><span data-ttu-id="3aa05-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="3aa05-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="3aa05-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="3aa05-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="3aa05-118">**値**</span><span class="sxs-lookup"><span data-stu-id="3aa05-118">**Value**</span></span>|<span data-ttu-id="3aa05-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="3aa05-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="3aa05-120">成功</span><span class="sxs-lookup"><span data-stu-id="3aa05-120">Success</span></span>  <br/> |<span data-ttu-id="3aa05-121">満了する要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="3aa05-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="3aa05-122">警告</span><span class="sxs-lookup"><span data-stu-id="3aa05-122">Warning</span></span>  <br/> | <span data-ttu-id="3aa05-123">処理されなかった要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="3aa05-123">Describes a request that was not processed.</span></span> <span data-ttu-id="3aa05-124">警告は、要求内のアイテムを処理し、それ以降の項目を処理できませんでした、エラーが発生した場合に返される場合があります。</span><span class="sxs-lookup"><span data-stu-id="3aa05-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="3aa05-125">以下は、警告の原因が考えられます。</span><span class="sxs-lookup"><span data-stu-id="3aa05-125">The following are some possible causes for warnings:</span></span>  <br/><br/><span data-ttu-id="3aa05-126">-Exchange ストアは、バッチの実行中にオフラインです。</span><span class="sxs-lookup"><span data-stu-id="3aa05-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="3aa05-127">-Active Directory ディレクトリ サービスは、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="3aa05-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="3aa05-128">-メールボックスを移動します。</span><span class="sxs-lookup"><span data-stu-id="3aa05-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="3aa05-129">-メッセージ データベース (MDB) は、オフラインです。</span><span class="sxs-lookup"><span data-stu-id="3aa05-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="3aa05-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="3aa05-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="3aa05-131">クォータを超えています。</span><span class="sxs-lookup"><span data-stu-id="3aa05-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="3aa05-132">エラー</span><span class="sxs-lookup"><span data-stu-id="3aa05-132">Error</span></span>  <br/> | <span data-ttu-id="3aa05-133">満たせない要求をについて説明します。</span><span class="sxs-lookup"><span data-stu-id="3aa05-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="3aa05-134">以下は、エラーの原因が考えられます。</span><span class="sxs-lookup"><span data-stu-id="3aa05-134">The following are some possible causes for errors:</span></span>  <br/><br/><span data-ttu-id="3aa05-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="3aa05-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="3aa05-136">属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="3aa05-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="3aa05-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="3aa05-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="3aa05-138">属性または要素のコンテキストでは無効です</span><span class="sxs-lookup"><span data-stu-id="3aa05-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="3aa05-139">の任意のクライアントから不正アクセスしようと</span><span class="sxs-lookup"><span data-stu-id="3aa05-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="3aa05-140">の有効なクライアント側の呼び出しに応答サーバー側の障害</span><span class="sxs-lookup"><span data-stu-id="3aa05-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="3aa05-141">エラーに関する情報は、 [ResponseCode](responsecode.md)および[メッセージ テキスト](messagetext.md)の要素を参照しています。</span><span class="sxs-lookup"><span data-stu-id="3aa05-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="3aa05-142">子要素</span><span class="sxs-lookup"><span data-stu-id="3aa05-142">Child elements</span></span>

|<span data-ttu-id="3aa05-143">**要素**</span><span class="sxs-lookup"><span data-stu-id="3aa05-143">**Element**</span></span>|<span data-ttu-id="3aa05-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="3aa05-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3aa05-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="3aa05-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="3aa05-146">応答のステータスの説明を提供します。</span><span class="sxs-lookup"><span data-stu-id="3aa05-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="3aa05-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3aa05-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="3aa05-148">要求で発生した特定のエラーを識別するエラー コードを提供します。</span><span class="sxs-lookup"><span data-stu-id="3aa05-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="3aa05-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="3aa05-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="3aa05-150">現在使用されていない将来の使用に予約されているとします。</span><span class="sxs-lookup"><span data-stu-id="3aa05-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="3aa05-151">0 の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3aa05-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="3aa05-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="3aa05-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="3aa05-153">追加のエラー応答情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="3aa05-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="3aa05-154">親要素</span><span class="sxs-lookup"><span data-stu-id="3aa05-154">Parent elements</span></span>

|<span data-ttu-id="3aa05-155">**要素**</span><span class="sxs-lookup"><span data-stu-id="3aa05-155">**Element**</span></span>|<span data-ttu-id="3aa05-156">**説明**</span><span class="sxs-lookup"><span data-stu-id="3aa05-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="3aa05-157">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="3aa05-157">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="3aa05-158">1 つのメールボックスのユーザーの空き時間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3aa05-158">Contains the free/busy information for a single mailbox user.</span></span> <br/> <br/> <span data-ttu-id="3aa05-159">この要素への XPath 2.0 の式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="3aa05-159">The following is the XPath 2.0 expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray[i]/FreeBusyResponse` <br/> |
|[<span data-ttu-id="3aa05-160">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="3aa05-160">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="3aa05-161">会議の提案の要求の応答の情報と提案のデータが含まれています。</span><span class="sxs-lookup"><span data-stu-id="3aa05-161">Contains response information and suggestion data for requested meeting suggestions.</span></span>  <br/><br/> <span data-ttu-id="3aa05-162">この要素への XPath 2.0 の式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="3aa05-162">The following is the XPath 2.0 expression to this element:</span></span><br/>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
|[<span data-ttu-id="3aa05-163">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="3aa05-163">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="3aa05-164">応答結果とユーザーの不在時の設定が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3aa05-164">Contains the response results and the OOF settings for a user.</span></span>  <br/><br/> <span data-ttu-id="3aa05-165">この要素への XPath 2.0 の式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="3aa05-165">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/GetUserOofSettingsResponse` <br/> |
|[<span data-ttu-id="3aa05-166">SetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="3aa05-166">SetUserOofSettingsResponse</span></span>](setuseroofsettingsresponse.md) <br/> |<span data-ttu-id="3aa05-167">実行しようとした[SetUserOofSettingsRequest](setuseroofsettingsrequest.md)メッセージの結果が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3aa05-167">Contains the result of an attempted [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) message.</span></span> <br/> <br/> <span data-ttu-id="3aa05-168">この要素への XPath 2.0 の式は、次のようにします。</span><span class="sxs-lookup"><span data-stu-id="3aa05-168">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/SetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="3aa05-169">備考</span><span class="sxs-lookup"><span data-stu-id="3aa05-169">Remarks</span></span>

<span data-ttu-id="3aa05-170">**ResponseMessageType**型は、Exchange Web サービスの応答をすべてに共通です。</span><span class="sxs-lookup"><span data-stu-id="3aa05-170">The **ResponseMessageType** type is common to all Exchange Web Services responses.</span></span> <span data-ttu-id="3aa05-171">**ResponseMessageType**型は、次の複合型によって拡張されました。</span><span class="sxs-lookup"><span data-stu-id="3aa05-171">The **ResponseMessageType** type is extended by the following complex types:</span></span> 
  
- <span data-ttu-id="3aa05-172">**ApplyConversationActionResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3aa05-172">**ApplyConversationActionResponseMessageType**</span></span>
    
- <span data-ttu-id="3aa05-173">**AttachmentInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3aa05-173">**AttachmentInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="3aa05-174">**DeleteAttachmentResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3aa05-174">**DeleteAttachmentResponseMessageType**</span></span>
    
- <span data-ttu-id="3aa05-175">**DeleteItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3aa05-175">**DeleteItemResponseMessageType**</span></span>
    
- <span data-ttu-id="3aa05-176">**ExpandDLResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3aa05-176">**ExpandDLResponseMessageType**</span></span>
    
- <span data-ttu-id="3aa05-177">**FindFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3aa05-177">**FindFolderResponseMessageType**</span></span>
    
- <span data-ttu-id="3aa05-178">**FindItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3aa05-178">**FindItemResponseMessageType**</span></span>
    
- <span data-ttu-id="3aa05-179">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3aa05-179">**FolderInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="3aa05-180">**GetEventsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3aa05-180">**GetEventsResponseMessageType**</span></span>
    
- <span data-ttu-id="3aa05-181">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3aa05-181">**ItemInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="3aa05-182">**ResolveNamesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3aa05-182">**ResolveNamesResponseMessageType**</span></span>
    
- <span data-ttu-id="3aa05-183">**SubscribeResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3aa05-183">**SubscribeResponseMessageType**</span></span>
    
- <span data-ttu-id="3aa05-184">**SendNotificationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3aa05-184">**SendNotificationResponseMessageType**</span></span>
    
- <span data-ttu-id="3aa05-185">**SyncFolderHierarchyResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3aa05-185">**SyncFolderHierarchyResponseMessageType**</span></span>
    
- <span data-ttu-id="3aa05-186">**SyncFolderItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="3aa05-186">**SyncFolderItemsResponseMessageType**</span></span>
    
<span data-ttu-id="3aa05-187">この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。</span><span class="sxs-lookup"><span data-stu-id="3aa05-187">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="3aa05-188">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="3aa05-188">Version differences</span></span>

<span data-ttu-id="3aa05-189">**ApplyConversationActionResponseMessage**および**DeleteItemResponseMessageType**の種類は、Exchange のビルド 15.00.0986.00 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3aa05-189">The **ApplyConversationActionResponseMessage** and **DeleteItemResponseMessageType** types were introduced in Exchange build 15.00.0986.00.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="3aa05-190">要素情報</span><span class="sxs-lookup"><span data-stu-id="3aa05-190">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="3aa05-191">名前空間</span><span class="sxs-lookup"><span data-stu-id="3aa05-191">Namespace</span></span>  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="3aa05-192">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="3aa05-192">Schema Name</span></span>  <br/> |<span data-ttu-id="3aa05-193">メッセージ スキーマ</span><span class="sxs-lookup"><span data-stu-id="3aa05-193">Messages schema</span></span>  <br/> |
|<span data-ttu-id="3aa05-194">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="3aa05-194">Validation File</span></span>  <br/> |<span data-ttu-id="3aa05-195">Messages.xsd</span><span class="sxs-lookup"><span data-stu-id="3aa05-195">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="3aa05-196">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="3aa05-196">Can be Empty</span></span>  <br/> |<span data-ttu-id="3aa05-197">False</span><span class="sxs-lookup"><span data-stu-id="3aa05-197">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="3aa05-198">関連項目</span><span class="sxs-lookup"><span data-stu-id="3aa05-198">See also</span></span>

- [<span data-ttu-id="3aa05-199">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="3aa05-199">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="3aa05-200">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="3aa05-200">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="3aa05-201">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="3aa05-201">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="3aa05-202">ユーザーの状態を取得します。</span><span class="sxs-lookup"><span data-stu-id="3aa05-202">Getting User Availability</span></span>](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

