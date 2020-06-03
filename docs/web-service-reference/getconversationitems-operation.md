---
title: GetConversationItems 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8ae00a99-b37b-4194-829c-fe300db6ab99
description: GetConversationItems 操作についての情報を検索します。
ms.openlocfilehash: ddeb5386e56653a32ca2e6d212518704cd0f0c58
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457782"
---
# <a name="getconversationitems-operation"></a><span data-ttu-id="7b606-103">GetConversationItems 操作</span><span class="sxs-lookup"><span data-stu-id="7b606-103">GetConversationItems operation</span></span>

<span data-ttu-id="7b606-104">**GetConversationItems**操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="7b606-104">Find information about the **GetConversationItems** operation.</span></span> 
  
<span data-ttu-id="7b606-105">**GetConversationItems**操作は、スレッド内のノードに整理されている1つまたは複数のアイテムのセットを取得します。</span><span class="sxs-lookup"><span data-stu-id="7b606-105">The **GetConversationItems** operation gets one or more sets of items that are organized in to nodes in a conversation.</span></span> 
  
<span data-ttu-id="7b606-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7b606-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getconversationitems-operation"></a><span data-ttu-id="7b606-107">GetConversationItems 操作の使用</span><span class="sxs-lookup"><span data-stu-id="7b606-107">Using the GetConversationItems operation</span></span>

<span data-ttu-id="7b606-108">**GetConversationItems**操作を使用して、プライマリメールボックスとアーカイブメールボックスの両方について、スレッド内のアイテムを取得することができます。</span><span class="sxs-lookup"><span data-stu-id="7b606-108">You can use the **GetConversationItems** operation to get items in conversations for both primary and archive mailboxes.</span></span> 
  
### <a name="getconversationitems-operation-soap-headers"></a><span data-ttu-id="7b606-109">GetConversationItems 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7b606-109">GetConversationItems operation SOAP headers</span></span>

<span data-ttu-id="7b606-110">**GetConversationItems**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="7b606-110">The **GetConversationItems** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="7b606-111">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="7b606-111">**Header name**</span></span>|<span data-ttu-id="7b606-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="7b606-112">**Element**</span></span>|<span data-ttu-id="7b606-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="7b606-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7b606-114">**偽装**</span><span class="sxs-lookup"><span data-stu-id="7b606-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="7b606-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="7b606-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="7b606-116">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="7b606-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="7b606-117">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="7b606-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7b606-118">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="7b606-118">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="7b606-119">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="7b606-119">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="7b606-120">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="7b606-120">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="7b606-121">この要素の最小値は**Exchange2013**です。</span><span class="sxs-lookup"><span data-stu-id="7b606-121">The minimum value for this element is **Exchange2013**.</span></span> <span data-ttu-id="7b606-122">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="7b606-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7b606-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="7b606-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="7b606-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7b606-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="7b606-125">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="7b606-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="7b606-126">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="7b606-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getconversationitems-operation-request-example-get-items-in-a-single-conversation"></a><span data-ttu-id="7b606-127">GetConversationItems 操作要求の例: 1 つの会話内のアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="7b606-127">GetConversationItems operation request example: Get items in a single conversation</span></span>

<span data-ttu-id="7b606-128">次の**GetConversationItems**操作要求の例は、単一の会話ですべてのスレッドアイテムを取得する方法を示しています。ただし、[削除済みアイテム] フォルダーと [下書き] フォルダーにあるアイテムは例外です。</span><span class="sxs-lookup"><span data-stu-id="7b606-128">The following example of a **GetConversationItems** operation request shows how to get all conversation items in a single conversation, with the exception of items located in the Deleted Items and Drafts folders.</span></span> <span data-ttu-id="7b606-129">応答で返される各アイテムには、アイテム識別子、件名、およびアイテムがメールボックスで受信された日時が含まれます。</span><span class="sxs-lookup"><span data-stu-id="7b606-129">Each item returned in the response will contain an item identifier, a subject, and the time that the item was received in the mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="7b606-130">この記事のすべてのアイテム識別子と変更キーは、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="7b606-130">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:GetConversationItems>
         <m:ItemShape>
            <t:BaseShape>IdOnly</t:BaseShape>
            <t:AdditionalProperties>
               <t:FieldURI FieldURI="item:Subject" />
               <t:FieldURI FieldURI="item:DateTimeReceived" />
            </t:AdditionalProperties>
         </m:ItemShape>
         <m:FoldersToIgnore>
            <t:DistinguishedFolderId Id="deleteditems" />
            <t:DistinguishedFolderId Id="drafts" />
         </m:FoldersToIgnore>
         <m:SortOrder>TreeOrderDescending</m:SortOrder>
         <m:Conversations>
            <t:Conversation>
               <t:ConversationId Id="AAQkADEzOTExYjJkakJCs=" />
            </t:Conversation>
         </m:Conversations>
      </m:GetConversationItems>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="7b606-131">この**GetConversationItems**要求の例には、次のオプションは含まれていません。</span><span class="sxs-lookup"><span data-stu-id="7b606-131">This example of a **GetConversationItems** request does not include the following options:</span></span> 
  
- <span data-ttu-id="7b606-132">応答で返されるアイテムの最大数を設定する[Maxitemstoreturn](maxitemstoreturn.md)要素。</span><span class="sxs-lookup"><span data-stu-id="7b606-132">The [MaxItemsToReturn](maxitemstoreturn.md) element, which sets the maximum number of items to return in the response.</span></span> 
    
- <span data-ttu-id="7b606-133">[MailboxScope](mailboxscope.md)要素。 **GetConversationItems**操作がプライマリメールボックス、アーカイブメールボックス、または両方のメールボックスで実行されるかどうかを示すことによって、メールボックスのスコープを設定します。</span><span class="sxs-lookup"><span data-stu-id="7b606-133">The [MailboxScope](mailboxscope.md) element, which sets the mailbox scope by indicating whether the **GetConversationItems** operation is to be performed on the primary mailbox, the archive mailbox, or both mailboxes.</span></span> 
    
- <span data-ttu-id="7b606-134">[Syncstate (base64Binary)](syncstate-base64binary.md)要素。同期状態は、会話で新規または更新された会話アイテムのみを取得するように設定されています。</span><span class="sxs-lookup"><span data-stu-id="7b606-134">The [SyncState (base64Binary)](syncstate-base64binary.md) element, which sets the synchronization state to only get conversation items that are new or updated in the conversation.</span></span> <span data-ttu-id="7b606-135">この要素は、会話ごとに設定されます。</span><span class="sxs-lookup"><span data-stu-id="7b606-135">This element is set for each conversation.</span></span> 
    
<span data-ttu-id="7b606-136">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7b606-136">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7b606-137">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="7b606-137">GetConversationItems</span></span>](getconversationitems.md)
    
- [<span data-ttu-id="7b606-138">ItemShape</span><span class="sxs-lookup"><span data-stu-id="7b606-138">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="7b606-139">BaseShape</span><span class="sxs-lookup"><span data-stu-id="7b606-139">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="7b606-140">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="7b606-140">AdditionalProperties</span></span>](additionalproperties.md)
    
- [<span data-ttu-id="7b606-141">FieldURI</span><span class="sxs-lookup"><span data-stu-id="7b606-141">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="7b606-142">FoldersToIgnore</span><span class="sxs-lookup"><span data-stu-id="7b606-142">FoldersToIgnore</span></span>](folderstoignore.md)
    
- [<span data-ttu-id="7b606-143">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="7b606-143">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="7b606-144">ソート順序 (ConversationNodeSortOrder)</span><span class="sxs-lookup"><span data-stu-id="7b606-144">SortOrder (ConversationNodeSortOrder)</span></span>](sortorder-conversationnodesortorder.md)
    
- [<span data-ttu-id="7b606-145">会話</span><span class="sxs-lookup"><span data-stu-id="7b606-145">Conversations</span></span>](conversations-ex15websvcsotherref.md)
    
- [<span data-ttu-id="7b606-146">会話 (ConversationRequestType)</span><span class="sxs-lookup"><span data-stu-id="7b606-146">Conversation (ConversationRequestType)</span></span>](conversation-conversationrequesttype.md)
    
- [<span data-ttu-id="7b606-147">ConversationId</span><span class="sxs-lookup"><span data-stu-id="7b606-147">ConversationId</span></span>](conversationid.md)
    
## <a name="successful-getconversationitems-operation-response"></a><span data-ttu-id="7b606-148">成功した GetConversationItems 操作の応答</span><span class="sxs-lookup"><span data-stu-id="7b606-148">Successful GetConversationItems operation response</span></span>

<span data-ttu-id="7b606-149">次の例は、1回の会話でアイテムを取得するための**GetConversationItems**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="7b606-149">The following example shows a successful response to a **GetConversationItems** operation request to get items in a single conversation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0"
                           MajorBuildNumber="545"
                           MinorBuildNumber="11"
                           Version="Exchange2013"
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetConversationItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                                      xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:GetConversationItemsResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Conversation>
                  <t:ConversationId Id="AAQkADEzOTExYjJkakJCs=" />
                  <t:SyncState>AQIAAABNVkUwAgIAAABhHqHUAwIAAABNVkUxBAIAAABhHqHfBAIAAABhHqHV</t:SyncState>
                  <t:ConversationNodes>
                     <t:ConversationNode>
                        <t:InternetMessageId>6a4838fa804045e09d40c1a39b9ea916@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTQrAABhHqHfAAA=" ChangeKey="CQAAABYAAACYAABhPpaq" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T18:42:27Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>2695d2b837954d68846b0c30491f5af1@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTExYjJkLTYxZDAt" ChangeKey="CQAAABQrAABhPpaP" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:38:26Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>15a56698d503438fbdaa18186d5b81b7@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>d3113e59c89c4288ae13100d033f8dbc@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkADEzOTFNVkUxAAA=" ChangeKey="CQAAABY4QrAABhPvYK" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:37:00Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>d3113e59c89c4288ae13100d033f8dbc@contoso.com</t:InternetMessageId>
                        <t:ParentInternetMessageId>189b712056c2430dbce334b40496ad00@contoso.com</t:ParentInternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkm4QrAABhHqHUAAA=" ChangeKey="CQAAABQrAABhPpaN" />
                              <t:Subject>RE: Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:37:05Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                     <t:ConversationNode>
                        <t:InternetMessageId>189b712056c2430dbce334b40496ad00@contoso.com</t:InternetMessageId>
                        <t:Items>
                           <t:Message>
                              <t:ItemId Id="AAMkArAABNVkUwAAA=" ChangeKey="CQAAABm4QrAABhPvYJ" />
                              <t:Subject>Daily issue scrub</t:Subject>
                              <t:DateTimeReceived>2012-10-30T17:36:00Z</t:DateTimeReceived>
                           </t:Message>
                        </t:Items>
                     </t:ConversationNode>
                  </t:ConversationNodes>
               </m:Conversation>
            </m:GetConversationItemsResponseMessage>
         </m:ResponseMessages>
      </m:GetConversationItemsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="7b606-150">後続の**GetConversationItems**操作要求の syncstate を保存することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="7b606-150">We recommend that you save the SyncState for subsequent **GetConversationItems** operation requests.</span></span> 
  
<span data-ttu-id="7b606-151">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7b606-151">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7b606-152">GetConversationItemsResponse</span><span class="sxs-lookup"><span data-stu-id="7b606-152">GetConversationItemsResponse</span></span>](getconversationitemsresponse.md)
    
- [<span data-ttu-id="7b606-153">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="7b606-153">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="7b606-154">GetConversationItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7b606-154">GetConversationItemsResponseMessage</span></span>](getconversationitemsresponsemessage.md)
    
- [<span data-ttu-id="7b606-155">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7b606-155">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7b606-156">会話 (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="7b606-156">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md)
    
- [<span data-ttu-id="7b606-157">ConversationId</span><span class="sxs-lookup"><span data-stu-id="7b606-157">ConversationId</span></span>](conversationid.md)
    
- [<span data-ttu-id="7b606-158">SyncState (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="7b606-158">SyncState (base64Binary)</span></span>](syncstate-base64binary.md)
    
- [<span data-ttu-id="7b606-159">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="7b606-159">ConversationNodes</span></span>](conversationnodes.md)
    
- [<span data-ttu-id="7b606-160">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="7b606-160">ConversationNode</span></span>](conversationnode.md)
    
- [<span data-ttu-id="7b606-161">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="7b606-161">InternetMessageId</span></span>](internetmessageid.md)
    
- [<span data-ttu-id="7b606-162">アイテム (非 Emptyarrayofallitemstype)</span><span class="sxs-lookup"><span data-stu-id="7b606-162">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="7b606-163">Message</span><span class="sxs-lookup"><span data-stu-id="7b606-163">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="7b606-164">ItemId</span><span class="sxs-lookup"><span data-stu-id="7b606-164">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="7b606-165">件名</span><span class="sxs-lookup"><span data-stu-id="7b606-165">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="7b606-166">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="7b606-166">DateTimeReceived</span></span>](datetimereceived.md)
    
## <a name="getconversationitems-operation-error-response"></a><span data-ttu-id="7b606-167">GetConversationItems 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="7b606-167">GetConversationItems operation error response</span></span>

<span data-ttu-id="7b606-168">次の例は、 **GetConversationItems**操作要求に対するエラー応答を示しています。これは、メールボックスに存在しなくなった、または無視されたすべてのスレッドアイテムが存在する会話内のアイテムを取得するためです。</span><span class="sxs-lookup"><span data-stu-id="7b606-168">The following example shows an error response to a **GetConversationItems** operation request to get items in a conversation that either no longer exists in the mailbox, or for which all the conversation items are located in folders that are ignored.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="556" MinorBuildNumber="8" Version="Exchange2013" xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" xmlns="https://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetConversationItemsResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:GetConversationItemsResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:GetConversationItemsResponseMessage>
      </m:ResponseMessages>
    </m:GetConversationItemsResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="7b606-169">関連項目</span><span class="sxs-lookup"><span data-stu-id="7b606-169">See also</span></span>

- [<span data-ttu-id="7b606-170">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="7b606-170">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="7b606-171">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="7b606-171">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
    
- [<span data-ttu-id="7b606-172">FindConversation 操作</span><span class="sxs-lookup"><span data-stu-id="7b606-172">FindConversation operation</span></span>](findconversation-operation.md)
    

