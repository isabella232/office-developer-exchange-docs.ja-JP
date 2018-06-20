---
title: GetConversationItems の操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 8ae00a99-b37b-4194-829c-fe300db6ab99
description: GetConversationItems の操作に関する情報を検索します。
ms.openlocfilehash: 9d9fb9cc04bcbb5846162c77c852defa51dff98b
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760672"
---
# <a name="getconversationitems-operation"></a><span data-ttu-id="001a3-103">GetConversationItems の操作</span><span class="sxs-lookup"><span data-stu-id="001a3-103">GetConversationItems operation</span></span>

<span data-ttu-id="001a3-104">**GetConversationItems**の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="001a3-104">Find information about the **GetConversationItems** operation.</span></span> 
  
<span data-ttu-id="001a3-105">**GetConversationItems**操作では、会話内のノードで構成されたアイテムの 1 つまたは複数のセットを取得します。</span><span class="sxs-lookup"><span data-stu-id="001a3-105">The **GetConversationItems** operation gets one or more sets of items that are organized in to nodes in a conversation.</span></span> 
  
<span data-ttu-id="001a3-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="001a3-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getconversationitems-operation"></a><span data-ttu-id="001a3-107">GetConversationItems 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="001a3-107">Using the GetConversationItems operation</span></span>

<span data-ttu-id="001a3-108">**GetConversationItems**操作を使用すると、原色の両方の会話とアーカイブ メールボックス内のアイテムを取得します。</span><span class="sxs-lookup"><span data-stu-id="001a3-108">You can use the **GetConversationItems** operation to get items in conversations for both primary and archive mailboxes.</span></span> 
  
### <a name="getconversationitems-operation-soap-headers"></a><span data-ttu-id="001a3-109">GetConversationItems 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="001a3-109">GetConversationItems operation SOAP headers</span></span>

<span data-ttu-id="001a3-110">**GetConversationItems**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="001a3-110">The **GetConversationItems** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="001a3-111">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="001a3-111">**Header name**</span></span>|<span data-ttu-id="001a3-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="001a3-112">**Element**</span></span>|<span data-ttu-id="001a3-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="001a3-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="001a3-114">**偽装**</span><span class="sxs-lookup"><span data-stu-id="001a3-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="001a3-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="001a3-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="001a3-116">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="001a3-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="001a3-117">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="001a3-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="001a3-118">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="001a3-118">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="001a3-119">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="001a3-119">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="001a3-120">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="001a3-120">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="001a3-121">この要素の最小値は、 **Exchange2013**です。</span><span class="sxs-lookup"><span data-stu-id="001a3-121">The minimum value for this element is **Exchange2013**.</span></span> <span data-ttu-id="001a3-122">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="001a3-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="001a3-123">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="001a3-123">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="001a3-124">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="001a3-124">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="001a3-125">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="001a3-125">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="001a3-126">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="001a3-126">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getconversationitems-operation-request-example-get-items-in-a-single-conversation"></a><span data-ttu-id="001a3-127">GetConversationItems 操作の要求の例: 1 つの会話でアイテムを取得</span><span class="sxs-lookup"><span data-stu-id="001a3-127">GetConversationItems operation request example: Get items in a single conversation</span></span>

<span data-ttu-id="001a3-128">**GetConversationItems**操作要求の次の例では、削除済みアイテムおよび [下書き] フォルダー内にある項目を除いて、1 つのテーマでの会話のすべての項目を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="001a3-128">The following example of a **GetConversationItems** operation request shows how to get all conversation items in a single conversation, with the exception of items located in the Deleted Items and Drafts folders.</span></span> <span data-ttu-id="001a3-129">応答で返される各項目は、項目 id、件名、およびアイテムをメールボックスで受信した時間に含まれます。</span><span class="sxs-lookup"><span data-stu-id="001a3-129">Each item returned in the response will contain an item identifier, a subject, and the time that the item was received in the mailbox.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="001a3-130">すべての項目の識別子と変更キーをこの資料では、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="001a3-130">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
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

<span data-ttu-id="001a3-131">**GetConversationItems**要求の次の使用例では、次のオプションは含まれません。</span><span class="sxs-lookup"><span data-stu-id="001a3-131">This example of a **GetConversationItems** request does not include the following options:</span></span> 
  
- <span data-ttu-id="001a3-132">[MaxItemsToReturn](maxitemstoreturn.md)要素の応答を取得するアイテムの最大数を設定します。</span><span class="sxs-lookup"><span data-stu-id="001a3-132">The [MaxItemsToReturn](maxitemstoreturn.md) element, which sets the maximum number of items to return in the response.</span></span> 
    
- <span data-ttu-id="001a3-133">[MailboxScope](mailboxscope.md)要素、 **GetConversationItems**操作は、プライマリ メールボックス、アーカイブ先のメールボックス、または両方のメールボックスに対して実行するかどうかを示すことによってメールボックスのスコープを設定します。</span><span class="sxs-lookup"><span data-stu-id="001a3-133">The [MailboxScope](mailboxscope.md) element, which sets the mailbox scope by indicating whether the **GetConversationItems** operation is to be performed on the primary mailbox, the archive mailbox, or both mailboxes.</span></span> 
    
- <span data-ttu-id="001a3-134">[同期状態 (base64Binary)](syncstate-base64binary.md)要素、だけは、スレッドの会話の項目を取得するのには同期の状態を設定します。</span><span class="sxs-lookup"><span data-stu-id="001a3-134">The [SyncState (base64Binary)](syncstate-base64binary.md) element, which sets the synchronization state to only get conversation items that are new or updated in the conversation.</span></span> <span data-ttu-id="001a3-135">この要素は、会話ごとに設定されています。</span><span class="sxs-lookup"><span data-stu-id="001a3-135">This element is set for each conversation.</span></span> 
    
<span data-ttu-id="001a3-136">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="001a3-136">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="001a3-137">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="001a3-137">GetConversationItems</span></span>](getconversationitems.md)
    
- [<span data-ttu-id="001a3-138">ItemShape</span><span class="sxs-lookup"><span data-stu-id="001a3-138">ItemShape</span></span>](itemshape.md)
    
- [<span data-ttu-id="001a3-139">BaseShape</span><span class="sxs-lookup"><span data-stu-id="001a3-139">BaseShape</span></span>](baseshape.md)
    
- [<span data-ttu-id="001a3-140">AdditionalProperties</span><span class="sxs-lookup"><span data-stu-id="001a3-140">AdditionalProperties</span></span>](additionalproperties.md)
    
- [<span data-ttu-id="001a3-141">FieldURI</span><span class="sxs-lookup"><span data-stu-id="001a3-141">FieldURI</span></span>](fielduri.md)
    
- [<span data-ttu-id="001a3-142">FoldersToIgnore</span><span class="sxs-lookup"><span data-stu-id="001a3-142">FoldersToIgnore</span></span>](folderstoignore.md)
    
- [<span data-ttu-id="001a3-143">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="001a3-143">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
- [<span data-ttu-id="001a3-144">並べ替え順序 (ConversationNodeSortOrder)</span><span class="sxs-lookup"><span data-stu-id="001a3-144">SortOrder (ConversationNodeSortOrder)</span></span>](sortorder-conversationnodesortorder.md)
    
- [<span data-ttu-id="001a3-145">スレッド</span><span class="sxs-lookup"><span data-stu-id="001a3-145">Conversations</span></span>](conversations-ex15websvcsotherref.md)
    
- [<span data-ttu-id="001a3-146">会話 (ConversationRequestType)</span><span class="sxs-lookup"><span data-stu-id="001a3-146">Conversation (ConversationRequestType)</span></span>](conversation-conversationrequesttype.md)
    
- [<span data-ttu-id="001a3-147">ConversationId</span><span class="sxs-lookup"><span data-stu-id="001a3-147">ConversationId</span></span>](conversationid.md)
    
## <a name="successful-getconversationitems-operation-response"></a><span data-ttu-id="001a3-148">GetConversationItems 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="001a3-148">Successful GetConversationItems operation response</span></span>

<span data-ttu-id="001a3-149">次の例では、1 つの会話でアイテムを取得する**GetConversationItems**操作要求に正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="001a3-149">The following example shows a successful response to a **GetConversationItems** operation request to get items in a single conversation.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15"
                           MinorVersion="0"
                           MajorBuildNumber="545"
                           MinorBuildNumber="11"
                           Version="Exchange2013"
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:GetConversationItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                                      xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="001a3-150">**GetConversationItems**の後続の操作要求の同期状態を保存することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="001a3-150">We recommend that you save the SyncState for subsequent **GetConversationItems** operation requests.</span></span> 
  
<span data-ttu-id="001a3-151">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="001a3-151">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="001a3-152">GetConversationItemsResponse</span><span class="sxs-lookup"><span data-stu-id="001a3-152">GetConversationItemsResponse</span></span>](getconversationitemsresponse.md)
    
- [<span data-ttu-id="001a3-153">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="001a3-153">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="001a3-154">GetConversationItemsResponseMessage</span><span class="sxs-lookup"><span data-stu-id="001a3-154">GetConversationItemsResponseMessage</span></span>](getconversationitemsresponsemessage.md)
    
- [<span data-ttu-id="001a3-155">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="001a3-155">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="001a3-156">会話 (ConversationResponseType)</span><span class="sxs-lookup"><span data-stu-id="001a3-156">Conversation (ConversationResponseType)</span></span>](conversation-conversationresponsetype.md)
    
- [<span data-ttu-id="001a3-157">ConversationId</span><span class="sxs-lookup"><span data-stu-id="001a3-157">ConversationId</span></span>](conversationid.md)
    
- [<span data-ttu-id="001a3-158">同期状態 (base64Binary)</span><span class="sxs-lookup"><span data-stu-id="001a3-158">SyncState (base64Binary)</span></span>](syncstate-base64binary.md)
    
- [<span data-ttu-id="001a3-159">ConversationNodes</span><span class="sxs-lookup"><span data-stu-id="001a3-159">ConversationNodes</span></span>](conversationnodes.md)
    
- [<span data-ttu-id="001a3-160">ConversationNode</span><span class="sxs-lookup"><span data-stu-id="001a3-160">ConversationNode</span></span>](conversationnode.md)
    
- [<span data-ttu-id="001a3-161">InternetMessageId</span><span class="sxs-lookup"><span data-stu-id="001a3-161">InternetMessageId</span></span>](internetmessageid.md)
    
- [<span data-ttu-id="001a3-162">アイテム (NonEmptyArrayOfAllItemsType)</span><span class="sxs-lookup"><span data-stu-id="001a3-162">Items (NonEmptyArrayOfAllItemsType)</span></span>](items-nonemptyarrayofallitemstype.md)
    
- [<span data-ttu-id="001a3-163">Message</span><span class="sxs-lookup"><span data-stu-id="001a3-163">Message</span></span>](message-ex15websvcsotherref.md)
    
- [<span data-ttu-id="001a3-164">ItemId</span><span class="sxs-lookup"><span data-stu-id="001a3-164">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="001a3-165">Subject</span><span class="sxs-lookup"><span data-stu-id="001a3-165">Subject</span></span>](subject.md)
    
- [<span data-ttu-id="001a3-166">DateTimeReceived</span><span class="sxs-lookup"><span data-stu-id="001a3-166">DateTimeReceived</span></span>](datetimereceived.md)
    
## <a name="getconversationitems-operation-error-response"></a><span data-ttu-id="001a3-167">GetConversationItems 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="001a3-167">GetConversationItems operation error response</span></span>

<span data-ttu-id="001a3-168">次の使用例は、メールボックス、または、会話のすべての項目内にあるフォルダーは無視されるは、存在しないのいずれかの会話で項目を取得する**GetConversationItems**の操作要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="001a3-168">The following example shows an error response to a **GetConversationItems** operation request to get items in a conversation that either no longer exists in the mailbox, or for which all the conversation items are located in folders that are ignored.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="556" MinorBuildNumber="8" Version="Exchange2013" xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" xmlns="http://schemas.microsoft.com/exchange/services/2006/types" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:GetConversationItemsResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="see-also"></a><span data-ttu-id="001a3-169">関連項目</span><span class="sxs-lookup"><span data-stu-id="001a3-169">See also</span></span>

- [<span data-ttu-id="001a3-170">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="001a3-170">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="001a3-171">ApplyConversationAction 操作</span><span class="sxs-lookup"><span data-stu-id="001a3-171">ApplyConversationAction operation</span></span>](applyconversationaction-operation.md)
    
- <span data-ttu-id="001a3-172">
  [FindConversation 操作](findconversation-operation.md)</span><span class="sxs-lookup"><span data-stu-id="001a3-172">[FindConversation operation](findconversation-operation.md)</span></span>
    

