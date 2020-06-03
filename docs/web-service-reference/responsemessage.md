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
description: ResponseMessage 要素は、要求内の1つのエンティティの応答状態に関する説明情報を提供します。
ms.openlocfilehash: a7f4240b1e988cb69d67118c6db58db0d7babba5
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467159"
---
# <a name="responsemessage"></a><span data-ttu-id="297fa-103">ResponseMessage</span><span class="sxs-lookup"><span data-stu-id="297fa-103">ResponseMessage</span></span>

<span data-ttu-id="297fa-104">**ResponseMessage**要素は、要求内の1つのエンティティの応答状態に関する説明情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="297fa-104">The **ResponseMessage** element provides descriptive information about the response status for a single entity within a request.</span></span> 
  
```xml
<ResponseMessage ResponseClass="">
   <MessageText/>
   <ResponseCode/>
   <DescriptiveLinkKey/>
   <MessageXml/>
</ResponseMessage>
```

 <span data-ttu-id="297fa-105">**ResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="297fa-105">**ResponseMessageType**</span></span>
## <a name="attributes-and-elements"></a><span data-ttu-id="297fa-106">属性と要素</span><span class="sxs-lookup"><span data-stu-id="297fa-106">Attributes and elements</span></span>

<span data-ttu-id="297fa-107">以下のセクションで、属性、子要素、親要素について説明します。</span><span class="sxs-lookup"><span data-stu-id="297fa-107">The following sections describe attributes, child elements, and parent elements.</span></span>
  
### <a name="attributes"></a><span data-ttu-id="297fa-108">属性</span><span class="sxs-lookup"><span data-stu-id="297fa-108">Attributes</span></span>

|<span data-ttu-id="297fa-109">**属性**</span><span class="sxs-lookup"><span data-stu-id="297fa-109">**Attribute**</span></span>|<span data-ttu-id="297fa-110">**説明**</span><span class="sxs-lookup"><span data-stu-id="297fa-110">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="297fa-111">**ResponseClass**</span><span class="sxs-lookup"><span data-stu-id="297fa-111">**ResponseClass**</span></span> <br/> | <span data-ttu-id="297fa-112">応答の状態を表します。</span><span class="sxs-lookup"><span data-stu-id="297fa-112">Represents the status of the response.</span></span> <br/><br/><span data-ttu-id="297fa-113">この属性には、次の値が有効です。</span><span class="sxs-lookup"><span data-stu-id="297fa-113">The following values are valid for this attribute:</span></span>  <br/><br/><span data-ttu-id="297fa-114">-成功</span><span class="sxs-lookup"><span data-stu-id="297fa-114">-  Success</span></span>  <br/><span data-ttu-id="297fa-115">-Warning</span><span class="sxs-lookup"><span data-stu-id="297fa-115">-  Warning</span></span>  <br/><span data-ttu-id="297fa-116">-エラー</span><span class="sxs-lookup"><span data-stu-id="297fa-116">-  Error</span></span>  <br/> |
   
#### <a name="responseclass-attribute-values"></a><span data-ttu-id="297fa-117">ResponseClass 属性の値</span><span class="sxs-lookup"><span data-stu-id="297fa-117">ResponseClass attribute values</span></span>

|<span data-ttu-id="297fa-118">**値**</span><span class="sxs-lookup"><span data-stu-id="297fa-118">**Value**</span></span>|<span data-ttu-id="297fa-119">**説明**</span><span class="sxs-lookup"><span data-stu-id="297fa-119">**Description**</span></span>|
|:-----|:-----|
|<span data-ttu-id="297fa-120">成功</span><span class="sxs-lookup"><span data-stu-id="297fa-120">Success</span></span>  <br/> |<span data-ttu-id="297fa-121">満たされる要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="297fa-121">Describes a request that is fulfilled.</span></span>  <br/> |
|<span data-ttu-id="297fa-122">警告</span><span class="sxs-lookup"><span data-stu-id="297fa-122">Warning</span></span>  <br/> | <span data-ttu-id="297fa-123">処理されなかった要求を示します。</span><span class="sxs-lookup"><span data-stu-id="297fa-123">Describes a request that was not processed.</span></span> <span data-ttu-id="297fa-124">要求内のアイテムが処理され、その後のアイテムを処理できなかったときにエラーが発生した場合は、警告が返されることがあります。</span><span class="sxs-lookup"><span data-stu-id="297fa-124">A warning may be returned if an error occurred while an item in the request was processing and subsequent items could not be processed.</span></span> <br/><br/><span data-ttu-id="297fa-125">以下に、次のような警告の原因を示します。</span><span class="sxs-lookup"><span data-stu-id="297fa-125">The following are some possible causes for warnings:</span></span>  <br/><br/><span data-ttu-id="297fa-126">-バッチ処理中に Exchange ストアがオフラインになります。</span><span class="sxs-lookup"><span data-stu-id="297fa-126">-  The Exchange store is offline during the batch.</span></span>  <br/><span data-ttu-id="297fa-127">-Active Directory ディレクトリサービスがオフラインになっています。</span><span class="sxs-lookup"><span data-stu-id="297fa-127">-  The Active Directory directory service is offline.</span></span>  <br/><span data-ttu-id="297fa-128">-メールボックスは移動されます。</span><span class="sxs-lookup"><span data-stu-id="297fa-128">-  Mailboxes are moved.</span></span>  <br/><span data-ttu-id="297fa-129">-メッセージデータベース (MDB) はオフラインです。</span><span class="sxs-lookup"><span data-stu-id="297fa-129">-  The message database (MDB) is offline.</span></span>  <br/><span data-ttu-id="297fa-130">-パスワードの有効期限が切れています。</span><span class="sxs-lookup"><span data-stu-id="297fa-130">-  A password is expired.</span></span>  <br/><span data-ttu-id="297fa-131">-クォータが上限を超えています。</span><span class="sxs-lookup"><span data-stu-id="297fa-131">-  A quota is exceeded.</span></span>  <br/> |
|<span data-ttu-id="297fa-132">Error</span><span class="sxs-lookup"><span data-stu-id="297fa-132">Error</span></span>  <br/> | <span data-ttu-id="297fa-133">満たされない要求を記述します。</span><span class="sxs-lookup"><span data-stu-id="297fa-133">Describes a request that cannot be fulfilled.</span></span> <br/><br/><span data-ttu-id="297fa-134">エラーの原因として、次のようなものが考えられます。</span><span class="sxs-lookup"><span data-stu-id="297fa-134">The following are some possible causes for errors:</span></span>  <br/><br/><span data-ttu-id="297fa-135">-無効な属性または要素</span><span class="sxs-lookup"><span data-stu-id="297fa-135">-  Invalid attributes or elements</span></span>  <br/><span data-ttu-id="297fa-136">-属性または要素が範囲外です</span><span class="sxs-lookup"><span data-stu-id="297fa-136">-  Attributes or elements out of range</span></span>  <br/><span data-ttu-id="297fa-137">-不明なタグ</span><span class="sxs-lookup"><span data-stu-id="297fa-137">-  Unknown tag</span></span>  <br/><span data-ttu-id="297fa-138">-属性または要素がコンテキスト内で有効ではありません</span><span class="sxs-lookup"><span data-stu-id="297fa-138">-  Attribute or element not valid in the context</span></span>  <br/><span data-ttu-id="297fa-139">-クライアントによる権限のないアクセス試行</span><span class="sxs-lookup"><span data-stu-id="297fa-139">-  Unauthorized access attempt by any client</span></span>  <br/><span data-ttu-id="297fa-140">-有効なクライアント側の呼び出しに応答した場合のサーバー側エラー</span><span class="sxs-lookup"><span data-stu-id="297fa-140">-  Server-side failure in response to a valid client-side call</span></span>  <br/> <br/> <span data-ttu-id="297fa-141">エラーに関する情報については、応答[secの](responsecode.md)要素と[messagetext](messagetext.md)要素を参照してください。</span><span class="sxs-lookup"><span data-stu-id="297fa-141">Information about the error can be found in the [ResponseCode](responsecode.md) and [MessageText](messagetext.md) elements.</span></span>  <br/> |
   
### <a name="child-elements"></a><span data-ttu-id="297fa-142">子要素</span><span class="sxs-lookup"><span data-stu-id="297fa-142">Child elements</span></span>

|<span data-ttu-id="297fa-143">**Element**</span><span class="sxs-lookup"><span data-stu-id="297fa-143">**Element**</span></span>|<span data-ttu-id="297fa-144">**説明**</span><span class="sxs-lookup"><span data-stu-id="297fa-144">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="297fa-145">MessageText</span><span class="sxs-lookup"><span data-stu-id="297fa-145">MessageText</span></span>](messagetext.md) <br/> |<span data-ttu-id="297fa-146">応答の状態を説明するテキストを提供します。</span><span class="sxs-lookup"><span data-stu-id="297fa-146">Provides a text description of the status of the response.</span></span>  <br/> |
|[<span data-ttu-id="297fa-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="297fa-147">ResponseCode</span></span>](responsecode.md) <br/> |<span data-ttu-id="297fa-148">要求で発生した特定のエラーを識別するエラーコードを提供します。</span><span class="sxs-lookup"><span data-stu-id="297fa-148">Provides an error code that identifies the specific error that the request encountered.</span></span>  <br/> |
|[<span data-ttu-id="297fa-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="297fa-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md) <br/> |<span data-ttu-id="297fa-150">現在未使用で、今後の使用のために予約されています。</span><span class="sxs-lookup"><span data-stu-id="297fa-150">Currently unused and is reserved for future use.</span></span> <span data-ttu-id="297fa-151">このプロパティには0の値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="297fa-151">It contains a value of 0.</span></span>  <br/> |
|[<span data-ttu-id="297fa-152">MessageXml</span><span class="sxs-lookup"><span data-stu-id="297fa-152">MessageXml</span></span>](messagexml.md) <br/> |<span data-ttu-id="297fa-153">エラー応答に関する追加情報を提供します。</span><span class="sxs-lookup"><span data-stu-id="297fa-153">Provides additional error response information.</span></span>  <br/> |
   
### <a name="parent-elements"></a><span data-ttu-id="297fa-154">親要素</span><span class="sxs-lookup"><span data-stu-id="297fa-154">Parent elements</span></span>

|<span data-ttu-id="297fa-155">**要素**</span><span class="sxs-lookup"><span data-stu-id="297fa-155">**Element**</span></span>|<span data-ttu-id="297fa-156">**説明**</span><span class="sxs-lookup"><span data-stu-id="297fa-156">**Description**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="297fa-157">FreeBusyResponse</span><span class="sxs-lookup"><span data-stu-id="297fa-157">FreeBusyResponse</span></span>](freebusyresponse.md) <br/> |<span data-ttu-id="297fa-158">1つのメールボックスユーザーの空き時間情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="297fa-158">Contains the free/busy information for a single mailbox user.</span></span> <br/> <br/> <span data-ttu-id="297fa-159">この要素の XPath 2.0 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="297fa-159">The following is the XPath 2.0 expression to this element:</span></span> <br/> <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray[i]/FreeBusyResponse` <br/> |
|[<span data-ttu-id="297fa-160">SuggestionsResponse</span><span class="sxs-lookup"><span data-stu-id="297fa-160">SuggestionsResponse</span></span>](suggestionsresponse.md) <br/> |<span data-ttu-id="297fa-161">要求された会議の提案の応答情報と提案データを格納します。</span><span class="sxs-lookup"><span data-stu-id="297fa-161">Contains response information and suggestion data for requested meeting suggestions.</span></span>  <br/><br/> <span data-ttu-id="297fa-162">この要素の XPath 2.0 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="297fa-162">The following is the XPath 2.0 expression to this element:</span></span><br/>  <br/>  `/GetUserAvailabilityResponse/SuggestionsResponse` <br/> |
|[<span data-ttu-id="297fa-163">GetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="297fa-163">GetUserOofSettingsResponse</span></span>](getuseroofsettingsresponse.md) <br/> |<span data-ttu-id="297fa-164">応答結果とユーザーの OOF 設定が含まれます。</span><span class="sxs-lookup"><span data-stu-id="297fa-164">Contains the response results and the OOF settings for a user.</span></span>  <br/><br/> <span data-ttu-id="297fa-165">この要素の XPath 2.0 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="297fa-165">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/GetUserOofSettingsResponse` <br/> |
|[<span data-ttu-id="297fa-166">SetUserOofSettingsResponse</span><span class="sxs-lookup"><span data-stu-id="297fa-166">SetUserOofSettingsResponse</span></span>](setuseroofsettingsresponse.md) <br/> |<span data-ttu-id="297fa-167">試行された[Setuseroofsettingsrequest](setuseroofsettingsrequest.md)メッセージの結果を格納します。</span><span class="sxs-lookup"><span data-stu-id="297fa-167">Contains the result of an attempted [SetUserOofSettingsRequest](setuseroofsettingsrequest.md) message.</span></span> <br/> <br/> <span data-ttu-id="297fa-168">この要素の XPath 2.0 式を次に示します。</span><span class="sxs-lookup"><span data-stu-id="297fa-168">The following is the XPath 2.0 expression to this element:</span></span>  <br/><br/>  `/SetUserOofSettingsResponse` <br/> |
   
## <a name="remarks"></a><span data-ttu-id="297fa-169">注釈</span><span class="sxs-lookup"><span data-stu-id="297fa-169">Remarks</span></span>

<span data-ttu-id="297fa-170">**Responsemessagetype**の種類は、すべての Exchange Web サービスの応答に共通です。</span><span class="sxs-lookup"><span data-stu-id="297fa-170">The **ResponseMessageType** type is common to all Exchange Web Services responses.</span></span> <span data-ttu-id="297fa-171">**Responsemessagetype**型は、次の複合型によって拡張されます。</span><span class="sxs-lookup"><span data-stu-id="297fa-171">The **ResponseMessageType** type is extended by the following complex types:</span></span> 
  
- <span data-ttu-id="297fa-172">**ApplyConversationActionResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="297fa-172">**ApplyConversationActionResponseMessageType**</span></span>
    
- <span data-ttu-id="297fa-173">**AttachmentInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="297fa-173">**AttachmentInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="297fa-174">**DeleteAttachmentResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="297fa-174">**DeleteAttachmentResponseMessageType**</span></span>
    
- <span data-ttu-id="297fa-175">**DeleteItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="297fa-175">**DeleteItemResponseMessageType**</span></span>
    
- <span data-ttu-id="297fa-176">**ExpandDLResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="297fa-176">**ExpandDLResponseMessageType**</span></span>
    
- <span data-ttu-id="297fa-177">**FindFolderResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="297fa-177">**FindFolderResponseMessageType**</span></span>
    
- <span data-ttu-id="297fa-178">**FindItemResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="297fa-178">**FindItemResponseMessageType**</span></span>
    
- <span data-ttu-id="297fa-179">**FolderInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="297fa-179">**FolderInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="297fa-180">**Getイベント Responsemessagetype**</span><span class="sxs-lookup"><span data-stu-id="297fa-180">**GetEventsResponseMessageType**</span></span>
    
- <span data-ttu-id="297fa-181">**ItemInfoResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="297fa-181">**ItemInfoResponseMessageType**</span></span>
    
- <span data-ttu-id="297fa-182">**ResolveNamesResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="297fa-182">**ResolveNamesResponseMessageType**</span></span>
    
- <span data-ttu-id="297fa-183">**オンラインでのお電話**</span><span class="sxs-lookup"><span data-stu-id="297fa-183">**SubscribeResponseMessageType**</span></span>
    
- <span data-ttu-id="297fa-184">**SendNotificationResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="297fa-184">**SendNotificationResponseMessageType**</span></span>
    
- <span data-ttu-id="297fa-185">**SyncFolderHierarchyResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="297fa-185">**SyncFolderHierarchyResponseMessageType**</span></span>
    
- <span data-ttu-id="297fa-186">**SyncFolderItemsResponseMessageType**</span><span class="sxs-lookup"><span data-stu-id="297fa-186">**SyncFolderItemsResponseMessageType**</span></span>
    
<span data-ttu-id="297fa-187">この要素を記述するスキーマは、Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。</span><span class="sxs-lookup"><span data-stu-id="297fa-187">The schema that describes this element is located in the EWS virtual directory of the computer that is running Microsoft Exchange Server 2007 that has the Client Access server role installed.</span></span>
  
### <a name="version-differences"></a><span data-ttu-id="297fa-188">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="297fa-188">Version differences</span></span>

<span data-ttu-id="297fa-189">**ApplyConversationActionResponseMessage**および**Deleteitemresponsemessagetype**の種類は、Exchange build 15.00.0986.00 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="297fa-189">The **ApplyConversationActionResponseMessage** and **DeleteItemResponseMessageType** types were introduced in Exchange build 15.00.0986.00.</span></span> 
  
## <a name="element-information"></a><span data-ttu-id="297fa-190">要素の情報</span><span class="sxs-lookup"><span data-stu-id="297fa-190">Element information</span></span>

|||
|:-----|:-----|
|<span data-ttu-id="297fa-191">Namespace</span><span class="sxs-lookup"><span data-stu-id="297fa-191">Namespace</span></span>  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|<span data-ttu-id="297fa-192">スキーマ名</span><span class="sxs-lookup"><span data-stu-id="297fa-192">Schema Name</span></span>  <br/> |<span data-ttu-id="297fa-193">メッセージスキーマ</span><span class="sxs-lookup"><span data-stu-id="297fa-193">Messages schema</span></span>  <br/> |
|<span data-ttu-id="297fa-194">検証ファイル</span><span class="sxs-lookup"><span data-stu-id="297fa-194">Validation File</span></span>  <br/> |<span data-ttu-id="297fa-195">メッセージ .xsd</span><span class="sxs-lookup"><span data-stu-id="297fa-195">Messages.xsd</span></span>  <br/> |
|<span data-ttu-id="297fa-196">空に設定可能</span><span class="sxs-lookup"><span data-stu-id="297fa-196">Can be Empty</span></span>  <br/> |<span data-ttu-id="297fa-197">正しくない</span><span class="sxs-lookup"><span data-stu-id="297fa-197">False</span></span>  <br/> |
   
## <a name="see-also"></a><span data-ttu-id="297fa-198">関連項目</span><span class="sxs-lookup"><span data-stu-id="297fa-198">See also</span></span>

- [<span data-ttu-id="297fa-199">GetUserAvailability 操作</span><span class="sxs-lookup"><span data-stu-id="297fa-199">GetUserAvailability operation</span></span>](getuseravailability-operation.md)
- [<span data-ttu-id="297fa-200">SetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="297fa-200">SetUserOofSettings operation</span></span>](setuseroofsettings-operation.md)
- [<span data-ttu-id="297fa-201">GetUserOofSettings 操作</span><span class="sxs-lookup"><span data-stu-id="297fa-201">GetUserOofSettings operation</span></span>](getuseroofsettings-operation.md)
- [<span data-ttu-id="297fa-202">ユーザーの空き時間情報の取得</span><span class="sxs-lookup"><span data-stu-id="297fa-202">Getting User Availability</span></span>](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

