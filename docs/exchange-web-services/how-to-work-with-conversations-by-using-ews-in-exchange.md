---
title: Exchange において EWS を使用して会話を処理する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 7750528c-acb2-43e5-a1e1-ee201c0e1730
description: Exchange で EWS マネージ API または EWS を使用して、会話の検索、会話へのアクションの適用、会話でのアイテムの取得の方法について説明します。
ms.openlocfilehash: 2dc66195f8d37836c32fc33737728c61fc5444ae
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456789"
---
# <a name="work-with-conversations-by-using-ews-in-exchange"></a><span data-ttu-id="bb82c-103">Exchange において EWS を使用して会話を処理する</span><span class="sxs-lookup"><span data-stu-id="bb82c-103">Work with conversations by using EWS in Exchange</span></span>

<span data-ttu-id="bb82c-104">Exchange で EWS マネージ API または EWS を使用して、会話の検索、会話へのアクションの適用、会話でのアイテムの取得の方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="bb82c-104">Learn about how to find conversations, apply actions to conversations, and get items in conversations by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="bb82c-105">Exchange のコンテキストでは、会話は関連のある一連の電子メール メッセージをグループ化して管理する方法です。</span><span class="sxs-lookup"><span data-stu-id="bb82c-105">In the context of Exchange, conversations are a way to group and manage a related set of email messages.</span></span> <span data-ttu-id="bb82c-106">会話は、関連するメッセージを表示する方法も提供できます。</span><span class="sxs-lookup"><span data-stu-id="bb82c-106">They can also provide a way to view related messages.</span></span> <span data-ttu-id="bb82c-107">Exchange はスレッドの最初の電子メール メッセージの **Message-ID** の値に基づいて会話を定義します。</span><span class="sxs-lookup"><span data-stu-id="bb82c-107">Exchange defines conversations based on the **Message-ID** value of the first email message in a thread.</span></span> <span data-ttu-id="bb82c-108">すべての返信および関連するメッセージは、その **References** ヘッダーおよび **In-Reply-To** ヘッダーの中で元のメッセージの **Message-ID** を参照します。</span><span class="sxs-lookup"><span data-stu-id="bb82c-108">All replies and related messages reference the original message's **Message-ID** header in their **References** and **In-Reply-To** headers.</span></span> 
  
<span data-ttu-id="bb82c-109">さらに、SOAP エンベロープ内で、メールボックスで受信するメッセージごとに、Exchange は固有のプロパティと要素を設定します。</span><span class="sxs-lookup"><span data-stu-id="bb82c-109">Additionally, inside the SOAP envelope, for each message received in a mailbox, Exchange sets specific properties and elements.</span></span>
  
<span data-ttu-id="bb82c-110">**表 1. すべての電子メール メッセージに設定される会話のプロパティおよび要素**</span><span class="sxs-lookup"><span data-stu-id="bb82c-110">**Table 1. Conversation properties and elements set on all email messages**</span></span>

|<span data-ttu-id="bb82c-111">**EWS マネージ API のプロパティ**</span><span class="sxs-lookup"><span data-stu-id="bb82c-111">**EWS Managed API property**</span></span>|<span data-ttu-id="bb82c-112">**EWS の要素**</span><span class="sxs-lookup"><span data-stu-id="bb82c-112">**EWS element**</span></span>|<span data-ttu-id="bb82c-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="bb82c-113">**Description**</span></span>|
|:-----|:-----|:-----|
|[<span data-ttu-id="bb82c-114">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="bb82c-114">ConversationTopic</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.conversationtopic%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="bb82c-115">ConversationTopic</span><span class="sxs-lookup"><span data-stu-id="bb82c-115">ConversationTopic</span></span>](https://msdn.microsoft.com/library/46cacf42-4039-4c8a-9b20-c42cdd9f2760%28Office.15%29.aspx) <br/> |<span data-ttu-id="bb82c-116">元のメッセージに設定された件名の値の正規化されたフォームが含まれています。</span><span class="sxs-lookup"><span data-stu-id="bb82c-116">Contains a normalized form of the subject value that was set on the original message.</span></span> <span data-ttu-id="bb82c-117">これは、**Thread-Topic** メッセージ ヘッダーと同じです。</span><span class="sxs-lookup"><span data-stu-id="bb82c-117">This is the same as the **Thread-Topic** message header.</span></span> <span data-ttu-id="bb82c-118">この値は読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bb82c-118">This value is read-only.</span></span>  <br/> |
|[<span data-ttu-id="bb82c-119">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="bb82c-119">ConversationIndex</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.conversationindex%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="bb82c-120">ConversationIndex</span><span class="sxs-lookup"><span data-stu-id="bb82c-120">ConversationIndex</span></span>](https://msdn.microsoft.com/library/fdf47e22-8d93-4ae4-883b-0c9f07f48724%28Office.15%29.aspx) <br/> |<span data-ttu-id="bb82c-121">会話内のアイテムの位置を表します。</span><span class="sxs-lookup"><span data-stu-id="bb82c-121">Represents the position of the item in the conversation.</span></span> <span data-ttu-id="bb82c-122">これは、**Thread-Index** メッセージ ヘッダーと同じです。</span><span class="sxs-lookup"><span data-stu-id="bb82c-122">This is the same as the **Thread-Index** message header.</span></span> <span data-ttu-id="bb82c-123">この値は読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="bb82c-123">This value is read-only.</span></span>  <br/> |
   
<span data-ttu-id="bb82c-124">Exchange は同じ **ConversationTopic** 値を最初のメッセージの返信に適用してから、元のメッセージに対する相対的なメッセージの位置を表す **ConversationIndex** の値を更新します。</span><span class="sxs-lookup"><span data-stu-id="bb82c-124">Exchange applies the same **ConversationTopic** value to replies to the first message and then updates the **ConversationIndex** value to represent the message's position relative to the original message.</span></span> <span data-ttu-id="bb82c-125">電子メール スレッドの件名が変更になった場合、Exchange は新しい **ConversationTopic** 値および新しい **ConversationIndex** 値を新しい会話に適用します。</span><span class="sxs-lookup"><span data-stu-id="bb82c-125">If the subject of the email thread changes, Exchange applies a new **ConversationTopic** value and new **ConversationIndex** values to the new conversation.</span></span> 
  
<span data-ttu-id="bb82c-126">**表 2. 会話を処理するための EWS マネージ API メソッドと EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="bb82c-126">**Table 2. EWS Managed API methods and EWS operations for working with conversations**</span></span>

|<span data-ttu-id="bb82c-127">**目的**</span><span class="sxs-lookup"><span data-stu-id="bb82c-127">**In order to…**</span></span>|<span data-ttu-id="bb82c-128">**使用する EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="bb82c-128">**Use this EWS Managed API method or methods**</span></span>|<span data-ttu-id="bb82c-129">**使用する EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="bb82c-129">**Use this EWS operation**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="bb82c-130">会話を検索する</span><span class="sxs-lookup"><span data-stu-id="bb82c-130">Find conversations</span></span>  <br/> |[<span data-ttu-id="bb82c-131">ExchangeService.FindConversation</span><span class="sxs-lookup"><span data-stu-id="bb82c-131">ExchangeService.FindConversation</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="bb82c-132">FindConversation</span><span class="sxs-lookup"><span data-stu-id="bb82c-132">FindConversation</span></span>](https://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="bb82c-133">会話の操作を適用する</span><span class="sxs-lookup"><span data-stu-id="bb82c-133">Apply conversation actions</span></span>  <br/> |[<span data-ttu-id="bb82c-134">Conversation.EnableAlwaysCategorizeItems</span><span class="sxs-lookup"><span data-stu-id="bb82c-134">Conversation.EnableAlwaysCategorizeItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.conversation.enablealwayscategorizeitems%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="bb82c-135">Conversation.EnableAlwaysDeleteItems</span><span class="sxs-lookup"><span data-stu-id="bb82c-135">Conversation.EnableAlwaysDeleteItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.conversation.enablealwaysdeleteitems%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="bb82c-136">Conversation.EnableAlwaysMoveItems</span><span class="sxs-lookup"><span data-stu-id="bb82c-136">Conversation.EnableAlwaysMoveItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.conversation.enablealwaysmoveitems%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="bb82c-137">ExchangeService.CopyItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="bb82c-137">ExchangeService.CopyItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.copyitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="bb82c-138">ExchangeService.DeleteItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="bb82c-138">ExchangeService.DeleteItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.deleteitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="bb82c-139">ExchangeService.DisableAlwaysCategorizeItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="bb82c-139">ExchangeService.DisableAlwaysCategorizeItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.disablealwayscategorizeitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="bb82c-140">ExchangeService.DisableAlwaysDeleteItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="bb82c-140">ExchangeService.DisableAlwaysDeleteItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.disablealwaysdeleteitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="bb82c-141">ExchangeService.DisableAlwaysMoveItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="bb82c-141">ExchangeService.DisableAlwaysMoveItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.disablealwaysmoveitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="bb82c-142">ExchangeService.EnableAlwaysCategorizeItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="bb82c-142">ExchangeService.EnableAlwaysCategorizeItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.enablealwayscategorizeitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="bb82c-143">ExchangeService.EnableAlwaysDeleteItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="bb82c-143">ExchangeService.EnableAlwaysDeleteItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.enablealwaysdeleteitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="bb82c-144">ExchangeService.EnableAlwaysMoveItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="bb82c-144">ExchangeService.EnableAlwaysMoveItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.enablealwaysmoveitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="bb82c-145">ExchangeService.MoveItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="bb82c-145">ExchangeService.MoveItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.moveitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="bb82c-146">ExchangeService.SetFlagStatusForItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="bb82c-146">ExchangeService.SetFlagStatusForItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.setflagstatusforitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="bb82c-147">ExchangeService.SetReadStateForItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="bb82c-147">ExchangeService.SetReadStateForItemsInConversations</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.setreadstateforitemsinconversations%28v=exchg.80%29.aspx) <br/> [<span data-ttu-id="bb82c-148">ExchangeService.SetRetentionPolicyForItemsInConversations</span><span class="sxs-lookup"><span data-stu-id="bb82c-148">ExchangeService.SetRetentionPolicyForItemsInConversations</span></span>](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.setretentionpolicyforitemsinconversations%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="bb82c-149">ApplyConversationAction</span><span class="sxs-lookup"><span data-stu-id="bb82c-149">ApplyConversationAction</span></span>](https://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="bb82c-150">1 つ以上の会話のアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="bb82c-150">Get items in one or more conversations</span></span>  <br/> |[<span data-ttu-id="bb82c-151">ExchangeService.GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="bb82c-151">ExchangeService.GetConversationItems</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="bb82c-152">GetConversationItems</span><span class="sxs-lookup"><span data-stu-id="bb82c-152">GetConversationItems</span></span>](https://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) <br/> |

<span data-ttu-id="bb82c-153"><a name="bk_findewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="bb82c-153"><a name="bk_findewsma"> </a></span></span>

## <a name="find-a-conversation-by-using-the-ews-managed-api"></a><span data-ttu-id="bb82c-154">EWS マネージ API を使用して会話を検索する</span><span class="sxs-lookup"><span data-stu-id="bb82c-154">Find a conversation by using the EWS Managed API</span></span>

<span data-ttu-id="bb82c-155">次の例に示すように、[ExchangeService.FindConversation](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) EWS マネージ API メソッドを使用して、会話を検索することができます。</span><span class="sxs-lookup"><span data-stu-id="bb82c-155">You can find conversations by using the [ExchangeService.FindConversation](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.findconversation%28v=exchg.80%29.aspx) EWS Managed API method, as shown in the following example.</span></span> <span data-ttu-id="bb82c-156">この例では、受信トレイ フォルダーのうち、件名に「news」という単語を含む最初の 10 個の会話を取得します。</span><span class="sxs-lookup"><span data-stu-id="bb82c-156">This example gets the first 10 conversations in the Inbox folder that have a subject that contains the word "news".</span></span> <span data-ttu-id="bb82c-157">その後、会話のトピック、最後の配信時間、およびグローバルな一意の受信者リストをコンソール ウィンドウに書き込みます。</span><span class="sxs-lookup"><span data-stu-id="bb82c-157">The example then writes the conversation topic, last delivery time, and global unique recipient list to the console window.</span></span> 
  
<span data-ttu-id="bb82c-158">この例では、**service** が有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーから既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="bb82c-158">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void FindConversation(ExchangeService service)
{
    // Create the view of conversations returned in the response. This view will return at most 10 results.
    ConversationIndexedItemView view = new ConversationIndexedItemView(10);
    // Create the query string to search for.
    String queryString = "subject:news";
    // Search the Inbox for conversations and return a results set with the specified view.
    // This method call results in a FindConversation call to EWS. 
    ICollection<Conversation> conversations = service.FindConversation(view, WellKnownFolderName.Inbox, queryString);
    // Examine properties on each conversation returned in the response.
    foreach (Conversation conversation in conversations)
    {
        Console.WriteLine("Conversation Topic: " + conversation.Topic);
        Console.WriteLine("Last Delivered: " + conversation.LastDeliveryTime.ToString());
        ApplyConversationActions(service, conversation);
        foreach (string GlUniqRec in conversation.GlobalUniqueRecipients)
        {
            Console.WriteLine("Global Unique Recipient: " + GlUniqRec);
        }
        Console.WriteLine("");
    }
}
```

<span data-ttu-id="bb82c-159"><a name="bk_findews"> </a></span><span class="sxs-lookup"><span data-stu-id="bb82c-159"><a name="bk_findews"> </a></span></span>

## <a name="find-a-conversation-by-using-ews"></a><span data-ttu-id="bb82c-160">EWS を使用して会話を検索する</span><span class="sxs-lookup"><span data-stu-id="bb82c-160">Find a conversation by using EWS</span></span>

<span data-ttu-id="bb82c-p106">次の例に示すように、[FindConversation](https://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) EWS 操作を使用して、会話を検索することができます。この例では、「ニュース」という単語を含む件名が入っている受信トレイ フォルダーで、最初の 10 個の会話を取得します。これは、EWS マネージ API を使用して[会話を検索する](#bk_findewsma)場合に、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="bb82c-p106">You can find conversations by using the [FindConversation](https://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) EWS operation, as shown in the following example. This example gets the first ten conversations in the Inbox folder that have a subject that contains the word "news". This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [find a conversation](#bk_findewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:FindConversation>
      <m:IndexedPageItemView MaxEntriesReturned="10"
                             Offset="0"
                             BasePoint="Beginning" />
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="inbox" />
      </m:ParentFolderId>
      <m:QueryString>subject:news</m:QueryString>
    </m:FindConversation>
  </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="bb82c-164">サーバーは、**FindConversation** 要求に対して [FindConversationResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージで応答します。このメッセージには、[ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) の値として **NoError** が含まれており、それは、操作が正常に完了したことを示しています。</span><span class="sxs-lookup"><span data-stu-id="bb82c-164">The server responds to the **FindConversation** request with a [FindConversationResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** to indicate that the operation completed successfully.</span></span> <span data-ttu-id="bb82c-165">また、この応答には、「news」という単語を含む件名が入っているメールボックス内の会話が 1 つだけ含まれています。</span><span class="sxs-lookup"><span data-stu-id="bb82c-165">The response also includes the only conversation in the mailbox that has a subject that contains the word "news".</span></span> 
  
<span data-ttu-id="bb82c-166">**ItemId**、**ChangeKey**、および **ConversationId** の属性は読みやすいよう短縮されています。</span><span class="sxs-lookup"><span data-stu-id="bb82c-166">The **ItemId**, **ChangeKey**, and **ConversationId** elements have been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="883"
                         MinorBuildNumber="10"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <FindConversationResponse ResponseClass="Success"
                              xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Conversations>
        <Conversation xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <ConversationId Id="aO2NM+Q=" />
          <ConversationTopic>Today's top news headlines</ConversationTopic>
          <UniqueRecipients>
            <String>Sadie Daniels</String>
          </UniqueRecipients>
          <GlobalUniqueRecipients>
            <String>Sadie Daniels</String>
          </GlobalUniqueRecipients>
          <UniqueUnreadSenders>
            <String>Ronnie Sturgis</String>
          </UniqueUnreadSenders>
          <GlobalUniqueUnreadSenders>
            <String>Ronnie Sturgis</String>
          </GlobalUniqueUnreadSenders>
          <UniqueSenders>
            <String>Ronnie Sturgis</String>
          </UniqueSenders>
          <GlobalUniqueSenders>
            <String>Ronnie Sturgis</String>
          </GlobalUniqueSenders>
          <LastDeliveryTime>2014-02-18T20:42:26Z</LastDeliveryTime>
          <GlobalLastDeliveryTime>2014-02-18T20:42:26Z</GlobalLastDeliveryTime>
          <HasAttachments>false</HasAttachments>
          <GlobalHasAttachments>false</GlobalHasAttachments>
          <MessageCount>1</MessageCount>
          <GlobalMessageCount>1</GlobalMessageCount>
          <UnreadCount>1</UnreadCount>
          <GlobalUnreadCount>1</GlobalUnreadCount>
          <Size>9330</Size>
          <GlobalSize>9330</GlobalSize>
          <ItemClasses>
            <ItemClass>IPM.Note</ItemClass>
          </ItemClasses>
          <GlobalItemClasses>
            <ItemClass>IPM.Note</ItemClass>
          </GlobalItemClasses>
          <Importance>Normal</Importance>
          <GlobalImportance>Normal</GlobalImportance>
          <ItemIds>
            <ItemId Id="sVCyAAA="
                    ChangeKey="CQAAAA==" />
          </ItemIds>
          <GlobalItemIds>
            <ItemId Id="sVCyAAA="
                    ChangeKey="CQAAAA==" />
          </GlobalItemIds>
          <LastModifiedTime>2014-02-18T20:42:26Z</LastModifiedTime>
          <InstanceKey>AQAAAAAAAQABAAAACbFYggAAAAA=</InstanceKey>
          <HasIrm>false</HasIrm>
          <GlobalHasIrm>false</GlobalHasIrm>
        </Conversation>
      </Conversations>
      <TotalConversationsInView>1</TotalConversationsInView>
      <IndexedOffset>1</IndexedOffset>
    </FindConversationResponse>
  </s:Body>
</s:Envelope>

```

<span data-ttu-id="bb82c-167"><a name="bk_applyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="bb82c-167"><a name="bk_applyewsma"> </a></span></span>

## <a name="apply-conversation-actions-by-using-the-ews-managed-api"></a><span data-ttu-id="bb82c-168">EWS マネージ API を使用して会話の操作を適用する</span><span class="sxs-lookup"><span data-stu-id="bb82c-168">Apply conversation actions by using the EWS Managed API</span></span>

<span data-ttu-id="bb82c-p108">次の例に示すように、いくつかの EWS マネージ API メソッドを使用して、会話の操作を会話に適用できます。この例では、会話の既存のアイテムにカテゴリを追加し、会話の将来のアイテムに同じカテゴリを適用します。また、フォルダーへの会話のアイテムの自動移動を有効にする方法も示します。この例では、アイテムが [下書き] フォルダーに移動されます。</span><span class="sxs-lookup"><span data-stu-id="bb82c-p108">You can apply conversation actions to a conversation by using a number of EWS Managed API methods, as shown in the following example. This example adds categories to existing items in a conversation and applies the same categories to future items in the conversation. It also shows how to enable the automatic moving of items in the conversation to a folder. In this example, items are moved to the Drafts folder.</span></span>
  
<span data-ttu-id="bb82c-173">この例では、**service** が有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーから既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="bb82c-173">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
<span data-ttu-id="bb82c-174">会話の操作を適用するメソッドの完全な一覧については、表 2 を参照してください。</span><span class="sxs-lookup"><span data-stu-id="bb82c-174">For a complete list of methods that apply conversation actions, see Table 2.</span></span>
  
```cs
static void ApplyConversationActions(ExchangeService service, Conversation conversation)
{
   // Create a list of categories to apply to a conversation.
   List<string> categories = new List<string>();
   categories.Add("Customer");
   categories.Add("System Integrator");
   // Apply categorization to all items in the conversation and process the request
   // synchronously after enabling this rule and after all item categorization has been applied. 
   // This method call results in an ApplyConversationAction call to EWS.
   conversation.EnableAlwaysCategorizeItems(categories, true);
   // Apply an always move rule to all items in the conversation and move the items
   // to the Drafts folder. Process the request asynchronously and return the response. 
   // immediately. This method call results in an ApplyConversationAction call to EWS.
   conversation.EnableAlwaysMoveItems(WellKnownFolderName.Drafts, false);
}

```

<span data-ttu-id="bb82c-175"><a name="bk_applyews"> </a></span><span class="sxs-lookup"><span data-stu-id="bb82c-175"><a name="bk_applyews"> </a></span></span>

## <a name="apply-conversation-actions-by-using-ews"></a><span data-ttu-id="bb82c-176">EWS を使用して会話の操作を適用する</span><span class="sxs-lookup"><span data-stu-id="bb82c-176">Apply conversation actions by using EWS</span></span>

<span data-ttu-id="bb82c-p109">次の例に示すように、[ApplyConversationAction](https://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) 操作を使用して、カテゴリ化、削除、移動などの会話の操作を適用できます。この例では、会話の既存のアイテムにカテゴリを追加し、会話の将来のアイテムに同じカテゴリを適用します。また、フォルダーへの会話のアイテムの自動移動を有効にする方法も示します。この例では、アイテムは [下書き] フォルダーに移動されます。これは、EWS マネージ API を使用して[会話の操作を適用](#bk_applyewsma)場合に、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="bb82c-p109">You can apply conversation actions, such as categorize, delete, and move, by using the [ApplyConversationAction](https://msdn.microsoft.com/library/73d7943d-d361-4f8b-9948-d85f886efa1a%28Office.15%29.aspx) operation, as shown in the following example. This example adds categories to existing items in a conversation and applies the same categories to future items in the conversation. It also shows how to enable the automatic moving of items in the conversation to a folder; in this example, items are moved to the Drafts folder. This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [apply conversation actions](#bk_applyewsma).</span></span>
  
<span data-ttu-id="bb82c-181">**ConversationId** 要素の値は読みやすいよう短縮されています。</span><span class="sxs-lookup"><span data-stu-id="bb82c-181">The **ConversationId** element has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:ApplyConversationAction>
      <m:ConversationActions>
        <t:ConversationAction>
          <t:Action>AlwaysMove</t:Action>
          <t:ConversationId Id="jG6WVpg=" />
          <t:ProcessRightAway>false</t:ProcessRightAway>
          <t:DestinationFolderId>
            <t:DistinguishedFolderId Id="drafts" />
          </t:DestinationFolderId>
        </t:ConversationAction>
      </m:ConversationActions>
    </m:ApplyConversationAction>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="bb82c-182">サーバーは、[ApplyConversationActionResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージで **ApplyConversationAction** 要求に応答します。このメッセージには、操作が正常に完了したことを示す、**NoError** の [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) の値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="bb82c-182">The server responds to the **ApplyConversationAction** request with a [ApplyConversationActionResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) value of **NoError** to indicate that the operation completed successfully.</span></span> 

<span data-ttu-id="bb82c-183"><a name="bk_getitemssingleewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="bb82c-183"><a name="bk_getitemssingleewsma"> </a></span></span>

## <a name="get-items-in-a-single-conversation-by-using-the-conversation-identifier-in-the-ews-managed-api"></a><span data-ttu-id="bb82c-184">EWS マネージ API の会話 ID を使用して 1 つの会話のアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="bb82c-184">Get items in a single conversation by using the conversation identifier in the EWS Managed API</span></span>

<span data-ttu-id="bb82c-185">[ExchangeService.GetConversationItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS マネージ API メソッドを使用して、会話内のアイテムを取得できます。</span><span class="sxs-lookup"><span data-stu-id="bb82c-185">You can get items in a conversation by using the [ExchangeService.GetConversationItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS Managed API method.</span></span> <span data-ttu-id="bb82c-186">次の使用例では、受信トレイ内の最初の会話の会話ノードのセットを提供します。</span><span class="sxs-lookup"><span data-stu-id="bb82c-186">This example provides the set of conversation nodes for the first conversation in the Inbox.</span></span> <span data-ttu-id="bb82c-187">各アイテムのアイテム識別子、件名、受信時刻が応答で返されるほかに、会話インデックスと親の会話のインデックス プロパティも返されます。</span><span class="sxs-lookup"><span data-stu-id="bb82c-187">The item identifier, subject, and received time for each item are returned in the response, along with the conversation index and parent conversation index properties.</span></span> <span data-ttu-id="bb82c-188">会話インデックス プロパティを使用すると、ノードの階層構造を再構築できます。</span><span class="sxs-lookup"><span data-stu-id="bb82c-188">You can use the conversation index properties to reconstruct the node hierarchy.</span></span> 
  
<span data-ttu-id="bb82c-189">この例では、既定の [削除済みアイテム] および [下書き] フォルダー内のすべての会話のアイテムは無視します。</span><span class="sxs-lookup"><span data-stu-id="bb82c-189">In this example, all conversation items in the default Deleted Items and Drafts folders are ignored.</span></span>
  
<span data-ttu-id="bb82c-190">この例では、**service** が有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="bb82c-190">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void GetConversationItemsSingleConversation(ExchangeService service)
{
   try
   {
      // Find the first item in the mailbox.
      // This method call results in an FindItem call to EWS.
      FindItemsResults<Item> results = service.FindItems(WellKnownFolderName.Inbox,
                                                         new ItemView(1));
      // Get the conversation identifier of the item. 
      ConversationId convId = results.Items[0].ConversationId;
      // Specify the properties that will be 
      // returned for the items in the conversation.
      PropertySet properties = new PropertySet(BasePropertySet.IdOnly,
                                                ItemSchema.Subject,
                                                ItemSchema.DateTimeReceived);
      // Identify the folders to ignore.
      Collection<FolderId> foldersToIgnore = new Collection<FolderId>() 
          { WellKnownFolderName.DeletedItems, WellKnownFolderName.Drafts };
      // Request the conversation items.
      // This method call results in an GetConversationItems call to EWS.
      ConversationResponse response = service.GetConversationItems(convId,
                                                   properties,
                                                  null,
                                                  foldersToIgnore,
                                                  ConversationSortOrder.TreeOrderDescending);
      // Get the synchronization state of the conversation.
      Console.WriteLine("SyncState: " + response.SyncState);
      Collection<Item> items = new Collection<Item>();
      // Process each node of conversation items.
      foreach (ConversationNode node in response.ConversationNodes)
      {
         Console.WriteLine("Parent conversation index: " + node.ParentConversationIndex);
         Console.WriteLine("Conversation index: " + node.ConversationIndex);
         Console.WriteLine("Conversation node items:");
         // Process each item in the conversation node.
         foreach (Item item in node.Items)
         {
            Console.WriteLine("   Item ID: " + item.Id.UniqueId);
            Console.WriteLine("   Subject: " + item.Subject);
            Console.WriteLine("   Received: " + item.DateTimeReceived);
            items.Add(item);
         }
      }
   }
   // This exception occurs if there is an error with the service.
   catch (ServiceResponseException srException)
   {
      Console.WriteLine(srException);
   }
}

```

<span data-ttu-id="bb82c-191">会話のアイテムを取得する後続の要求のために、**SyncState** プロパティをキャッシュすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="bb82c-191">We recommend that you cache the **SyncState** property for subsequent requests to get items in the conversation.</span></span> 

<span data-ttu-id="bb82c-192"><a name="bk_getitemsmanyewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="bb82c-192"><a name="bk_getitemsmanyewsma"> </a></span></span>

## <a name="get-items-in-many-conversations-by-using-the-conversationrequest-object-in-the-ews-managed-api"></a><span data-ttu-id="bb82c-193">EWS マネージ API の ConversationRequest オブジェクトを使用して多数の会話のアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="bb82c-193">Get items in many conversations by using the ConversationRequest object in the EWS Managed API</span></span>

<span data-ttu-id="bb82c-194">[ConversationRequest](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.conversationrequest%28v=exchg.80%29.aspx) オブジェクトと [ExchangeService.GetConversationItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS マネージ API メソッドを使用して、2 つ以上の会話からアイテムを取得できます。</span><span class="sxs-lookup"><span data-stu-id="bb82c-194">You can use the [ConversationRequest](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.conversationrequest%28v=exchg.80%29.aspx) object and the [ExchangeService.GetConversationItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS Managed API method to get items from two or more conversations.</span></span> <span data-ttu-id="bb82c-195">次の例では、受信トレイ内の最初の 2 つの会話の会話ノードのセットを提供します。</span><span class="sxs-lookup"><span data-stu-id="bb82c-195">This example provides a set of conversation nodes for the first two conversations in the Inbox.</span></span> <span data-ttu-id="bb82c-196">各アイテムのアイテム識別子、件名、受信時刻が応答で返されるほかに、会話インデックスと親の会話のインデックス プロパティも返されます。</span><span class="sxs-lookup"><span data-stu-id="bb82c-196">The item identifier, subject, and the received time for each item will be returned in the response, along with the conversation index and parent conversation index properties.</span></span> <span data-ttu-id="bb82c-197">会話インデックス プロパティを使用すると、ノードの階層構造を再構築できます。</span><span class="sxs-lookup"><span data-stu-id="bb82c-197">You can use the conversation index properties to reconstruct the node hierarchy.</span></span> <span data-ttu-id="bb82c-198">次の使用例は、受信トレイの最初の 2 つのアイテムが別の会話からであると想定しています。</span><span class="sxs-lookup"><span data-stu-id="bb82c-198">This example assumes that the first two items in the Inbox are from different conversations.</span></span> 
  
<span data-ttu-id="bb82c-199">この例では、既定の [削除済みアイテム] および [下書き] フォルダー内のすべての会話のアイテムは無視します。</span><span class="sxs-lookup"><span data-stu-id="bb82c-199">In this example, all conversation items in the default Deleted Items and Drafts folders are ignored.</span></span>
  
<span data-ttu-id="bb82c-200">この例では、**service** が有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="bb82c-200">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
static void GetConversationItemsManyConversations(ExchangeService service)
{
   try
   {
      // Find the first two items in the Inbox. This item will be used to call the GetConversationItems operation.
      // This method call results in an FindItem call to EWS.
      FindItemsResults<Item> results = service.FindItems(WellKnownFolderName.Inbox, new ItemView(2));
      // Get the conversation identifier of the first two items in the Inbox. 
      ConversationId convId1 = results.Items[0].ConversationId;
      ConversationId convId2 = results.Items[1].ConversationId;
      
      // Identify two conversation requests. 
      ConversationRequest convR1 = new ConversationRequest();
      convR1.ConversationId = convId1;
      ConversationRequest convR2 = new ConversationRequest();
      convR2.ConversationId = convId2;
      // Create a collection of conversations to fetch. 
      Collection<ConversationRequest> conversations = new Collection<ConversationRequest>();
      conversations.Add(convR1);
      conversations.Add(convR2);
      // Specify the properties that will be returned for the items in the conversation.
      PropertySet properties = new PropertySet(BasePropertySet.IdOnly,
                                                ItemSchema.Subject,
                                                ItemSchema.DateTimeReceived);
      // Identify the folders to ignore.
      Collection<FolderId> foldersToIgnore = new Collection<FolderId>() 
          { WellKnownFolderName.DeletedItems, WellKnownFolderName.Drafts };
      // Request the conversation items.
      // This method call results in an GetConversationItems call to EWS.
      ServiceResponseCollection<GetConversationItemsResponse> responses = 
          service.GetConversationItems(conversations, properties, foldersToIgnore, 
          ConversationSortOrder.TreeOrderDescending);
      // Process each conversation.
      foreach (GetConversationItemsResponse resp in responses)
      {
         // Identify the synchronization state of the conversation.
         Console.WriteLine("Sync State: " + resp.Conversation.SyncState);
         // Process each node in the conversation.
         foreach (ConversationNode node in resp.Conversation.ConversationNodes)
         {
            Console.WriteLine("Parent conversation index: " + node.ParentConversationIndex);
            Console.WriteLine("Conversation index: " + node.ConversationIndex);
            Console.WriteLine("Conversation node items:");
            // Process each item in the conversation node.
            foreach (Item item in node.Items)
            {
               Console.WriteLine("   Item ID: " + item.Id.UniqueId);
               Console.WriteLine("   Subject: " + item.Subject);
               Console.WriteLine("   Received: " + item.DateTimeReceived);
            }
         }
      }
   }
   // This exception occurs if there is an error with the service.
   catch (ServiceResponseException srException)
   { 
      Console.WriteLine(srException);
   }
}

```

<span data-ttu-id="bb82c-201">ベスト プラクティスとして、**BasePropertySet** クラスに **FirstClassProperties** オプションを使用するのではなく、クライアント アプリケーションに必要なプロパティだけを返すことをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="bb82c-201">As a best practice, we recommend that you return only the properties that the client application requires, rather than using the **FirstClassProperties** option for the **BasePropertySet** class.</span></span> <span data-ttu-id="bb82c-202">会話のアイテムを取得する後続の要求のために、**SyncState** プロパティをキャッシュすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="bb82c-202">We recommend that you cache the **SyncState** property for subsequent requests to get items in the conversation.</span></span> 

<span data-ttu-id="bb82c-203"><a name="bk_getitemsews"> </a></span><span class="sxs-lookup"><span data-stu-id="bb82c-203"><a name="bk_getitemsews"> </a></span></span>

## <a name="get-items-in-conversations-by-using-the-conversation-identifier-in-ews"></a><span data-ttu-id="bb82c-204">EWS の会話 ID を使用して会話のアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="bb82c-204">Get items in conversations by using the conversation identifier in EWS</span></span>

<span data-ttu-id="bb82c-p113">[GetConversationItems](https://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) EWS 操作を使用して、会話内のアイテムを取得できます。次の使用例では、受信トレイ内の最初の会話の会話ノードのセットを提供します。各アイテムのアイテム識別子、件名、受信時刻が応答で返されるほかに、会話インデックスと親の会話のインデックス プロパティも返されます。会話インデックス プロパティを使用すると、ノードの階層構造を再構築できます。</span><span class="sxs-lookup"><span data-stu-id="bb82c-p113">You can get items in a conversation by using the [GetConversationItems](https://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) EWS operation. This example provides a set of conversation nodes for the first conversation in the Inbox. The item identifier, subject, and received time for each item are returned in the response, along with the conversation index and parent conversation index properties. You can use the conversation index properties to reconstruct the node hierarchy.</span></span> 
  
<span data-ttu-id="bb82c-209">この例では、既定の [削除済みアイテム] および [下書き] フォルダー内のすべての会話のアイテムは無視します。</span><span class="sxs-lookup"><span data-stu-id="bb82c-209">In this example, all conversation items in the default Deleted Items and Drafts folders are ignored.</span></span>
  
<span data-ttu-id="bb82c-210">**ConversationId** 要素の値は読みやすいよう短縮されています。</span><span class="sxs-lookup"><span data-stu-id="bb82c-210">The **ConversationId** element has been shortened for readability.</span></span> 
  
<span data-ttu-id="bb82c-211">複数の会話からアイテムを取得するには、追加の **Conversation** 要素を含めます。</span><span class="sxs-lookup"><span data-stu-id="bb82c-211">To get items from more than one conversation, include additional **Conversation** elements.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m=https://schemas.microsoft.com/exchange/services/2006/messages
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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
          <t:ConversationId Id="LUQFH6Q=" />
        </t:Conversation>
      </m:Conversations>
    </m:GetConversationItems>
  </soap:Body>
</soap:Envelope>
```

サーバーは、**GetConversationItems** 要求に対して [GetConversationItemsResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージで応答します。このメッセージには、[ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) の値として **NoError** が含まれおり、それは、操作が正常に完了したことを示しています。 <span data-ttu-id="bb82c-213">応答は、会話の [ConversationNodes](https://msdn.microsoft.com/library/5c8a35b8-a940-4b3e-8768-9ba95766fd79%28Office.15%29.aspx) にも含まれています。</span><span class="sxs-lookup"><span data-stu-id="bb82c-213">The response also includes the [ConversationNodes](https://msdn.microsoft.com/library/5c8a35b8-a940-4b3e-8768-9ba95766fd79%28Office.15%29.aspx) in the conversation.</span></span> 
  
<span data-ttu-id="bb82c-214">**ItemId**、**SyncState**、および **ConversationId** の属性は読みやすいよう短縮されています。</span><span class="sxs-lookup"><span data-stu-id="bb82c-214">The **ItemId**, **SyncState**, and **ConversationId** elements have been shortened for readability.</span></span> 
  
```XML
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="873"
                         MinorBuildNumber="9"
                         Version="V2_9"
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
            <t:ConversationId Id="LUQFH6Q=" />
            <t:SyncState>AAAAYAm1</t:SyncState>
            <t:ConversationNodes>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;994051d7c1a346efbfce8dec2cbad509
                    @SN2SR01MB006.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;faa2b1df30074380abe3527b0cd18ca5
                    @SN2SR01MB001.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="AYB1NAAA="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYCHq" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T13:15:00Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;faa2b1df30074380abe3527b0cd18ca5
                    @SN2SR01MB001.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;6a8e7658524b41cda7cdc3f23c1074a5
                    @SN2SR01MB001.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="lQAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAu8" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T10:02:08Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;bcdb185495834370a874a1e7ebedbb96
                    @SN2SR01MB005.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;e52a4de6b98d484887e141da094a2ce6
                    @SN2SR01MB006.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="igAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAuj" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T16:20:10Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;e52a4de6b98d484887e141da094a2ce6
                    @SN2SR01MB006.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;f0db3ead01db4fe087d98022149aa16f
                    @SN2SR01MB001.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="iwAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAul" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T15:30:10Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;f0db3ead01db4fe087d98022149aa16f
                    @SN2SR01MB001.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;88b1884ecaaa4f68b081c009d827e8c6
                    @SN2SR01MB003.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="jQAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAuq" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T14:20:10Z</t:DateTimeReceived>
                  </t:Message>
                </t:Items>
              </t:ConversationNode>
              <t:ConversationNode>
                <t:InternetMessageId>&amp;lt;88b1884ecaaa4f68b081c009d827e8c6
                    @SN2SR01MB003.com&amp;gt;</t:InternetMessageId>
                <t:ParentInternetMessageId>&amp;lt;faa2b1df30074380abe3527b0cd18ca5
                    @SN2SR01MB001.com&amp;gt;</t:ParentInternetMessageId>
                <t:Items>
                  <t:Message>
                    <t:ItemId Id="kAAAAA=="
                              ChangeKey="CQAAABYAAAD/oydcA+SPQZGbKWNyvNIZAAAAYAux" />
                    <t:Subject>RE: Review Proposal for Tailspin Toys</t:Subject>
                    <t:DateTimeReceived>2014-01-02T12:52:09Z</t:DateTimeReceived>
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

<span data-ttu-id="bb82c-215"><a name="bk_versiondiffs"> </a></span><span class="sxs-lookup"><span data-stu-id="bb82c-215"><a name="bk_versiondiffs"> </a></span></span>

## <a name="version-differences"></a><span data-ttu-id="bb82c-216">バージョンの相違点</span><span class="sxs-lookup"><span data-stu-id="bb82c-216">Version differences</span></span>

<span data-ttu-id="bb82c-217">Exchange Server 2010 Service Pack 1 (SP1) を使用している場合、[FindConversation](https://msdn.microsoft.com/library/office/jj220668%28v=exchg.80%29.aspx) メソッドは利用できるオプションが少なく、[FindConversation](https://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) 操作は要求の要素が少なくなります。</span><span class="sxs-lookup"><span data-stu-id="bb82c-217">When you are using Exchange Server 2010 Service Pack 1 (SP1), the [FindConversation](https://msdn.microsoft.com/library/office/jj220668%28v=exchg.80%29.aspx) method has fewer options available, and the [FindConversation](https://msdn.microsoft.com/library/2384908a-c203-45b6-98aa-efd6a4c23aac%28Office.15%29.aspx) operation has fewer elements in the request.</span></span> 
  
<span data-ttu-id="bb82c-218">**表 3. FindConversation の Exchange 2010 SP1 バージョンのサポート**</span><span class="sxs-lookup"><span data-stu-id="bb82c-218">**Table 3. Exchange 2010 SP1 version support for FindConversation**</span></span>

|<span data-ttu-id="bb82c-219">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="bb82c-219">**EWS Managed API method**</span></span>|<span data-ttu-id="bb82c-220">**EWS 要素**</span><span class="sxs-lookup"><span data-stu-id="bb82c-220">**EWS elements**</span></span>|
|:-----|:-----|
|[<span data-ttu-id="bb82c-221">FindConversation (ViewBase、FolderId)</span><span class="sxs-lookup"><span data-stu-id="bb82c-221">FindConversation (ViewBase, FolderId)</span></span>](https://msdn.microsoft.com/library/office/jj220668%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="bb82c-222">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="bb82c-222">IndexedPageItemView</span></span>](https://msdn.microsoft.com/library/6d1b0b04-cc35-4a57-bd7a-824136d14fda%28Office.15%29.aspx) <br/> [<span data-ttu-id="bb82c-223">SortOrder</span><span class="sxs-lookup"><span data-stu-id="bb82c-223">SortOrder</span></span>](https://msdn.microsoft.com/library/c2413f0b-8c03-46ae-9990-13338b3c53a6%28Office.15%29.aspx) <br/> [<span data-ttu-id="bb82c-224">ParentFolderId</span><span class="sxs-lookup"><span data-stu-id="bb82c-224">ParentFolderId</span></span>](https://msdn.microsoft.com/library/0e3e6e5f-06d0-499b-8ca4-d36036521658%28Office.15%29.aspx) <br/> |
   
<span data-ttu-id="bb82c-225">[GetConversationItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS マネージ API メソッド、および [GetConversationItems](https://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) EWS 操作は、Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="bb82c-225">The [GetConversationItems](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.getconversationitems%28v=exchg.80%29.aspx) EWS Managed API method and the [GetConversationItems](https://msdn.microsoft.com/library/8ae00a99-b37b-4194-829c-fe300db6ab99%28Office.15%29.aspx) EWS operation were introduced in Exchange Server 2013.</span></span> <span data-ttu-id="bb82c-226">Exchange の以前のバージョンを対象とするアプリケーションは、表 2 に示すように、会話の操作のみを会話に適用できます。</span><span class="sxs-lookup"><span data-stu-id="bb82c-226">Applications that target earlier versions of Exchange can only apply conversation actions to conversations, as listed in Table 2.</span></span> 
  
<span data-ttu-id="bb82c-227">**FindConversation** EWS マネージ API メソッド、および **FindConversation** EWS メソッドは、Exchange 2010 または Exchange 2007 の最初のリリース バージョンでは利用できません。</span><span class="sxs-lookup"><span data-stu-id="bb82c-227">The **FindConversation** EWS Managed API method and the **FindConversation** EWS method are not available in the initial release version of Exchange 2010 or in Exchange 2007.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="bb82c-228">関連項目</span><span class="sxs-lookup"><span data-stu-id="bb82c-228">See also</span></span>

- [<span data-ttu-id="bb82c-229">Exchange のメールと EWS</span><span class="sxs-lookup"><span data-stu-id="bb82c-229">Email and EWS in Exchange</span></span>](email-and-ews-in-exchange.md)
- [<span data-ttu-id="bb82c-230">Exchange で EWS とともに検索フィルターを使用する</span><span class="sxs-lookup"><span data-stu-id="bb82c-230">Use search filters with EWS in Exchange</span></span>](how-to-use-search-filters-with-ews-in-exchange.md)   
- [<span data-ttu-id="bb82c-231">Exchange 2013: プログラムを使用してメールボックス内の会話を検索する</span><span class="sxs-lookup"><span data-stu-id="bb82c-231">Exchange 2013: Find conversations in mailboxes programmatically</span></span>](https://code.msdn.microsoft.com/exchange/Exchange-2013-Find-d4b6b3af)    
- [<span data-ttu-id="bb82c-232">Exchange 2013: メールボックス内の会話を管理するための操作を適用する</span><span class="sxs-lookup"><span data-stu-id="bb82c-232">Exchange 2013: Apply actions to manage conversations in a mailbox</span></span>](https://code.msdn.microsoft.com/exchange/Exchange-2013-Apply-accde0b5)
    

