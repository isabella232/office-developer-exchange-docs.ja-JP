---
title: Exchange で EWS を使用して、代理人としてメールにアクセスする
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: a8123604-c7c0-405d-a0ed-7a9b4a431bfd
description: Exchange で EWS マネージ API または EWS を使用して、代理人としてメールにアクセスする方法を説明します。
ms.openlocfilehash: 23dd35f95b1303ff643e3760aa408e308725cb12
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21354037"
---
# <a name="access-email-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="5e6d2-103">Exchange で EWS を使用して、代理人としてメールにアクセスする</span><span class="sxs-lookup"><span data-stu-id="5e6d2-103">How to: Access email as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="5e6d2-104">Exchange で EWS マネージ API または EWS を使用して、代理人としてメールにアクセスする方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-104">Learn how to access email as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="5e6d2-p101">EWS マネージ API または EWS を使用して、ユーザーにメーボックス所有者の受信トレイ フォルダーへの代理人アクセス権を付与できます。代理人は、メールボックス所有者の代わりに会議出席依頼を作成し、アクセス許可に応じて、メールボックス所有者の受信トレイ フォルダーのメールの検索、取得、更新、削除を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-p101">You can use the EWS Managed API or EWS to give a user delegate access to a mailbox owner's Inbox folder. The delegate can then create meeting requests on behalf of the mailbox owner, search for email, and retrieve, update, and delete email from the mailbox owner's Inbox folder, depending on their permissions.</span></span>
  
<span data-ttu-id="5e6d2-p102">代理人として、代理人アクセス権なしで受信トレイ フォルダーへのアクセスに使用するのと同じメソッドと操作を使用して、メールボックス所有者の受信トレイ フォルダーにアクセスします。大きな違いは、[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicit)を使用してメール アイテムを検索または作成する必要がある点です。アイテム ID を識別すると、[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用してアイテムを取得、更新、削除できます。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-p102">As a delegate, you use the same methods and operations to access a mailbox owner's Inbox folder that you use to access an Inbox folder without delegate access. The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create an email item, and then after you identify the item ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="5e6d2-109">**表 1. 代理人としてメールにアクセスするための EWS マネージ API メソッドと EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="5e6d2-109">**Table 1.  EWS Managed API methods and EWS operations for accessing email as a delegate**</span></span>

|<span data-ttu-id="5e6d2-110">**目的**</span><span class="sxs-lookup"><span data-stu-id="5e6d2-110">**If you want to…**</span></span>|<span data-ttu-id="5e6d2-111">**使用する EWS マネージ API メソッド…**</span><span class="sxs-lookup"><span data-stu-id="5e6d2-111">**Use this EWS Managed API method**</span></span>|<span data-ttu-id="5e6d2-112">**使用する EWS 操作…**</span><span class="sxs-lookup"><span data-stu-id="5e6d2-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5e6d2-113">代理人としてメールを作成して送信する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-113">Create and send an email as a delegate</span></span>  <br/> |<span data-ttu-id="5e6d2-114">[EmailMessage.Save](http://msdn.microsoft.com/ja-JP/library/dd635209%28v=exchg.80%29.aspx): [FolderId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) パラメーターがメールボックス所有者の下書きフォルダーへの[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-114">[EmailMessage.Save](http://msdn.microsoft.com/ja-JP/library/dd635209%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Drafts folder</span></span>  <br/> <span data-ttu-id="5e6d2-115">[EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/ja-JP/library/dd634248%28v=exchg.80%29.aspx): [FolderId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) パラメーターがメールボックス所有者の送信済みアイテム フォルダーへの[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-115">[EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/ja-JP/library/dd634248%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Sent Items folder</span></span>  <br/> |<span data-ttu-id="5e6d2-116">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx): [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-116">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> <span data-ttu-id="5e6d2-117">[SendItem](http://msdn.microsoft.com/library/a966da19-b05a-4504-ac98-91acc1667b9a%28Office.15%29.aspx): [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-117">[SendItem](http://msdn.microsoft.com/library/a966da19-b05a-4504-ac98-91acc1667b9a%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="5e6d2-118">代理人として複数のメール メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-118">Create multiple email messages as a delegate</span></span>  <br/> |<span data-ttu-id="5e6d2-119">[ExchangeService.CreateItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx): **FolderId** パラメーターがメールボックス所有者の受信トレイ フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-119">[ExchangeService.CreateItemshttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Inbox folder</span></span>  <br/> |<span data-ttu-id="5e6d2-120">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx): [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-120">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="5e6d2-121">代理人としてメールを検索する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-121">Search for or find an email as a delegate</span></span>  <br/> |<span data-ttu-id="5e6d2-122">[ExchangeService.FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx): **FolderId** パラメーターがメールボックス所有者の受信トレイ フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-122">[ExchangeService.FindItemshttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Inbox folder</span></span>  <br/> |<span data-ttu-id="5e6d2-123">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx): [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-123">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="5e6d2-124">代理人としてメールを取得</span><span class="sxs-lookup"><span data-stu-id="5e6d2-124">Get an email as a delegate</span></span>  <br/> |[<span data-ttu-id="5e6d2-125">EmailMessage.Bind</span><span class="sxs-lookup"><span data-stu-id="5e6d2-125">EmailMessage.Bind</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="5e6d2-126">GetItem</span><span class="sxs-lookup"><span data-stu-id="5e6d2-126">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="5e6d2-127">代理人としてメールを更新する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-127">Update an email as a delegate</span></span>  <br/> |<span data-ttu-id="5e6d2-128">[EmailMessage.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) の後に [EmailMessage.Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="5e6d2-128">[EmailMessage.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [EmailMessage.Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="5e6d2-129">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="5e6d2-129">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="5e6d2-130">代理人としてメールを削除する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-130">Delete an email as a delegate</span></span>  <br/> |<span data-ttu-id="5e6d2-131">[EmailMessage.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) の後に [EmailMessage.Delete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="5e6d2-131">[EmailMessage.Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [EmailMessage.Delete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="5e6d2-132">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="5e6d2-132">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |
   
<span data-ttu-id="5e6d2-133">代理人としてメールを操作する場合、次の点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-133">Keep the following things in mind when working with emails as a delegate:</span></span>
  
- <span data-ttu-id="5e6d2-p103">代理人が行う必要がある操作が会議出席依頼と出欠の返答だけである場合、受信トレイ フォルダーへのアクセスは必要ありません。詳しくは、「[代理人として予定表にアクセスするために事前に必要なタスク](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md#bk_prereq)」をご覧ください。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-p103">If a delegate only needs to work with meeting requests and responses, the delegate does not need access to the Inbox folder. For more information, see [prerequisite tasks for accessing calendars as a delegate](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md#bk_prereq).</span></span>
    
- <span data-ttu-id="5e6d2-136">メールボックス所有者の代理として送信したメッセージを受信者が受信すると、送信者は「*メールボックス所有者*の*代理人*」として表示されます。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-136">When a recipient receives a message that was sent on behalf of a mailbox owner, the sender appears as "*Delegate* on behalf of *mailbox owner*."</span></span> 
    
> [!NOTE]
> <span data-ttu-id="5e6d2-137">この記事のコード例では、primary@contoso.com は、メールボックス所有者です。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-137">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 
  
## <a name="prerequisite-tasks"></a><span data-ttu-id="5e6d2-138">事前に必要なタスク</span><span class="sxs-lookup"><span data-stu-id="5e6d2-138">Prerequisite tasks</span></span>
<span data-ttu-id="5e6d2-139"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="5e6d2-139"></span></span>

<span data-ttu-id="5e6d2-140">ユーザーは、代理人としてメールボックス所有者の受信トレイ フォルダーにアクセスできるようにするために、[アクセス許可を持つ代理人として](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)メールボックス所有者の受信トレイ フォルダーに追加される必要があります。 </span><span class="sxs-lookup"><span data-stu-id="5e6d2-140">Before a user can access the mailbox owner's Inbox folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Inbox folder.</span></span> 
  
## <a name="create-and-send-an-email-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="5e6d2-141">EWS マネージ API を使用して、代理人としてメールを作成および送信する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-141">Create and send an email as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="5e6d2-142"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="5e6d2-142"></span></span>

<span data-ttu-id="5e6d2-143">EWS マネージ API を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックス所有者の代わりにメールを作成および送信することができます。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-143">The EWS Managed API enables you to use the service object for the delegate user to create and send email on behalf of the mailbox owner.</span></span> <span data-ttu-id="5e6d2-144">次の例は、[Save](http://msdn.microsoft.com/ja-JP/library/dd635209%28v=exchg.80%29.aspx) メソッドを使用してメールボックス所有者の下書きフォルダーにメッセージを保存し、[SendAndSaveCopy](http://msdn.microsoft.com/ja-JP/library/dd634248%28v=exchg.80%29.aspx) メソッドを使用してそのメールを送信してそのメッセージをメールボックス所有者の送信済みアイテム フォルダーに保存する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-144">The EWS Managed API enables you to use the service object for the delegate user to create and send email on behalf of the mailbox owner. This example shows how to use the [Savehttp://msdn.microsoft.com/en-us/library/dd635209(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/dd635209%28v=exchg.80%29.aspx) method to save the message in the mailbox owner's Drafts folder, and then the [SendAndSaveCopyhttp://msdn.microsoft.com/en-us/library/dd634248(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/dd634248%28v=exchg.80%29.aspx) method to send the mail and save the message in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="5e6d2-145">この例は、**service** が代理人の有効な [ExchangeService](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、代理人に[メールボックス所有者の受信トレイ、下書き、送信済みアイテムの各フォルダーの適切なアクセス許可](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)が付与されていることを前提にしています。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-145">This example assumes that **service** is a valid [ExchangeServicehttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the [appropriate permissions for the mailbox owner's Inbox, Drafts, and Sent Items folder](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span></span>
  
```cs
public static void DelegateAccessCreateEmail(ExchangeService service)
{
    // Create an email message and provide it with connection 
    // configuration information by using an ExchangeService 
    // object named service.
    EmailMessage message = new EmailMessage(service);
    // Set properties on the email message.
    message.Subject = "Company Soccer Team";
    message.Body = "Are you interested in joining?";
    message.ToRecipients.Add("sadie@contoso.com");
    // Save the email to the mailbox owner's Drafts folder.
    // This method call results in a CreateItem call to EWS.
    // The FolderId parameter contains the context for the 
    // mailbox owner's Inbox folder. Any additional actions 
    // taken on this message will be performed in the mailbox 
    // owner's mailbox. 
    message.Save(new FolderId(WellKnownFolderName.Drafts, new Mailbox("primary@contoso.com")));
    // Send the email and save the message in the mailbox owner's 
    // Sent Items folder.
    // This method call results in a SendItem call to EWS.
    message.SendAndSaveCopy(new FolderId(WellKnownFolderName.SentItems, new Mailbox("primary@contoso.com")));
    Console.WriteLine("An email with the subject '" + message.Subject + "' has been sent to '" 
    + message.ToRecipients[0] + "' and saved in the Sent Items folder of the mailbox owner.");
}
```

## <a name="create-and-send-an-email-as-a-delegate-by-using-ews"></a><span data-ttu-id="5e6d2-146">EWS を使用して代理人としてメールを作成して送信する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-146">Create and send an email as a delegate by using EWS</span></span>
<span data-ttu-id="5e6d2-147"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="5e6d2-147"></span></span>

<span data-ttu-id="5e6d2-p105">EWS を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックス所有者の代わりにメールを作成および送信することができます。次の例は、[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) 操作を使用してメールを作成し、[SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) 操作によって送信してメールボックス所有者の送信済みアイテム フォルダーに保存する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-p105">EWS enables you to use the service object for the delegate user to create and send email on behalf of the mailbox owner. This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create an email and the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation to send the time and save it in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="5e6d2-150">またこれは、[メールの作成と送信](#bk_createewsma)に **Save** メソッドを使用する際に、EWS マネージ API が送信する最初の XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-150">This is also the first XML request that the EWS Managed API sends when you use the **Save** method to [create and send an email](#bk_createewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Company Soccer Team</t:Subject>
          <t:Body BodyType="HTML">Are you interested in joining?</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>sadie@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="5e6d2-p106">サーバーは、**CreateItem** 要求に [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージで応答します。このメッセージには、メールが正常に作成および保存されたことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素の値が含まれます。また、この応答には新しく作成されたメールのアイテム ID も含まれます。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-p106">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the email was created and saved successfully. The response also contains the item ID of the newly created email.</span></span>
  
<span data-ttu-id="5e6d2-153">**ItemId** 値は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-153">The **ItemId** value has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:CreateItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:CreateItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:Items>
            <t:Message>
              <t:ItemId Id="iNRaAAA="
                        ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQPU" />
            </t:Message>
          </m:Items>
        </m:CreateItemResponseMessage>
      </m:ResponseMessages>
    </m:CreateItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="5e6d2-154">次に、**SendItem** 操作を使用してメールボックス所有者の代理としてメッセージを送信し、メールボックス所有者の送信済みアイテム フォルダーに保存します。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-154">Next, use the **SendItem** operation to send the message on behalf of the mailbox owner and save it in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="5e6d2-155">**ItemId** 値は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-155">The **ItemId** value has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:SendItem SaveItemToFolder="true">
      <m:ItemIds>
        <t:ItemId Id="iNRaAAA="
                  ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQPU" />
      </m:ItemIds>
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="sentitems">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
    </m:SendItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="5e6d2-156">サーバーは、**SendItem** 要求に [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) メッセージで応答します。このメッセージには、メールがメールボックス所有者の送信済みアイテム フォルダーに正常に送信および保存されたことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素の値が含まれます。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-156">The server responds to the **SendItem** request with a [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the email was sent and saved to the mailbox owner's Sent Items folder successfully.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:SendItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:SendItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
        </m:SendItemResponseMessage>
      </m:ResponseMessages>
    </m:SendItemResponse>
  </s:Body>
</s:Envelope>
```

## <a name="search-for-an-email-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="5e6d2-157">EWS マネージ API を使用して、代理人としてメールを検索する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-157">Search for an email as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="5e6d2-158"><a name="bk_searchewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="5e6d2-158"></span></span>

<span data-ttu-id="5e6d2-159">メールを検索するには、[FolderId](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) パラメーターが含まれるいずれかの [ExchangeService.FindItems](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) メソッドを使用し、メールボックス所有者の受信トレイ フォルダーを指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-159">To search for an email, you must use one of the [ExchangeService.FindItemshttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) methods that includes a [FolderIdhttp://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid(v=exchg.80).aspx](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Inbox folder.</span></span> 
  
```cs
static void DelegateAccessSearchEmailWithFilter(ExchangeService service)
{
    // Limit the result set to 10 items.
    ItemView view = new ItemView(10);
    // Define the search filter.
    SearchFilter.ContainsSubstring filter = new SearchFilter.ContainsSubstring(ItemSchema.Subject, 
        "soccer", ContainmentMode.Substring, ComparisonMode.IgnoreCase);
    view.PropertySet = new PropertySet(ItemSchema.Subject,
                                       ItemSchema.DateTimeReceived,
                                       EmailMessageSchema.IsRead);
    // Item searches do not support deep traversal.
    view.Traversal = ItemTraversal.Shallow;
    // Sorting.
    view.OrderBy.Add(ItemSchema.DateTimeReceived, SortDirection.Descending);
    try
    {
        // Call FindItems to find matching Inbox items. 
        // The parameters of FindItems must denote the mailbox owner,
        // mailbox, and Inbox folder.
        // This call results in a FindItem call to EWS.
        FindItemsResults<Item> results = service.FindItems(new 
            FolderId(WellKnownFolderName.Inbox, "primary@contoso.com"), 
            filter, view);
        foreach (Item item in results.Items)
        {
            Console.WriteLine("Subject: {0}", item.Subject);
            Console.WriteLine("Id: {0}", item.Id.ToString());
            if (item is EmailMessage)
            {
                EmailMessage message = item as EmailMessage;
                Console.WriteLine("Read: {0}", message.IsRead.ToString());
            }
        }
    }
    catch (Exception ex)
    {
        Console.WriteLine("Exception while enumerating results: {0}", ex.Message);
    }
}
```

<span data-ttu-id="5e6d2-160">**FindItems** 呼び出しが ID と共に応答を返すと、ID と[暗黙的アクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用して対象のメールを取得、更新、削除できます。その際、メールボックス所有者の SMTP アドレスを指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-160">After the **FindItems** call returns a response with an ID, you can get, update or delete that email by using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) – and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="search-for-an-email-as-a-delegate-by-using-ews"></a><span data-ttu-id="5e6d2-161">EWS を使用して代理人としてメールを検索する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-161">Search for an email as a delegate by using EWS</span></span>
<span data-ttu-id="5e6d2-162"><a name="bk_searchews"> </a></span><span class="sxs-lookup"><span data-stu-id="5e6d2-162"></span></span>

<span data-ttu-id="5e6d2-p107">EWS を使用すると、代理ユーザーのサービス オブジェクトを使用して、一連の検索条件に一致するメールを検索できます。次の例は、[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) 操作を使用して、件名に「soccer」という語が含まれる、所有者の受信トレイ フォルダー内のメッセージを検索する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-p107">EWS enables you to use the service object for the delegate user to search for emails that meet a set of search criteria. This example shows how to use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find messages in the owner's Inbox folder that contain the word "soccer" in the subject.</span></span> 
  
<span data-ttu-id="5e6d2-165">また、これは、[メールを検索する](#bk_searchewsma)際に、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-165">This is also the XML request that the EWS Managed API sends when you [search for an email](#bk_searchewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version=" Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:FindItem Traversal="Shallow">
      <m:ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="item:Subject" />
          <t:FieldURI FieldURI="item:DateTimeReceived" />
          <t:FieldURI FieldURI="message:IsRead" />
        </t:AdditionalProperties>
      </m:ItemShape>
      <m:IndexedPageItemView MaxEntriesReturned="10"
                             Offset="0"
                             BasePoint="Beginning" />
      <m:Restriction>
        <t:Contains ContainmentMode="Substring"
                    ContainmentComparison="IgnoreCase">
          <t:FieldURI FieldURI="item:Subject" />
          <t:Constant Value="soccer" />
        </t:Contains>
      </m:Restriction>
      <m:SortOrder>
        <t:FieldOrder Order="Descending">
          <t:FieldURI FieldURI="item:DateTimeReceived" />
        </t:FieldOrder>
      </m:SortOrder>
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="inbox">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:ParentFolderIds>
    </m:FindItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="5e6d2-p108">サーバーは、**FindItem** 要求に [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) メッセージで応答します。このメッセージには、検索が正常に完了したことを示す、**NoError** の [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素の値が含まれます。この応答には、検索条件と一致するすべての [Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) 要素が含まれます。この例では、1 つのメールのみが検出されました。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-p108">The server responds to the **FindItem** request with a [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the search completed successfully. The response contains a [Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) element for any emails that met the search criteria. In this case, only one email is found.</span></span> 
  
<span data-ttu-id="5e6d2-169">[ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) 要素の値は読みやすいよう短縮されています。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-169">The value of the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element has been shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:FindItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:FindItemResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:RootFolder IndexedPagingOffset="1"
                        TotalItemsInView="1"
                        IncludesLastItemInRange="true">
            <t:Items>
              <t:Message>
                <t:ItemId Id="iNwoAAA="
                          ChangeKey="CQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiQuu" />
                <t:Subject>Soccer team</t:Subject>
                <t:DateTimeReceived>2014-03-10T06:16:55Z</t:DateTimeReceived>
                <t:IsRead>false</t:IsRead>
              </t:Message>
            </t:Items>
          </m:RootFolder>
        </m:FindItemResponseMessage>
      </m:ResponseMessages>
    </m:FindItemResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="5e6d2-170">この時点で、条件と一致するメールの **ItemId** がわかったので **ItemId** と[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用してメールの取得、更新、削除を行えます。その際、メールボックス所有者の SMTP アドレスを指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-170">Now that you have the **ItemId** for the email that meets your criteria, you can get, update, or delete that email by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) – and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="5e6d2-171">EWS マネージ API を使用して、代理人としてメール アイテムを取得、更新、削除する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-171">Get, update, or delete email items as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="5e6d2-172"><a name="bk_geteswma"> </a></span><span class="sxs-lookup"><span data-stu-id="5e6d2-172"></span></span>

<span data-ttu-id="5e6d2-p109">EWS マネージ API を使用すると、代理人アクセスを使用していない場合と同じように、メール アイテムを取得、更新、削除できます。唯一の違いは、**ExchangeService** オブジェクトが代理ユーザーを対象にしている点です。**Bind** メソッド呼び出しに含まれるアイテム ID は、メールボックス所有者の受信トレイ フォルダー内のメールボックス ストアにあるアイテムを一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-p109">You can use the EWS Managed API to get, update, or delete an email in the same way that you perform these actions when you're not using delegate access. The only difference is that the **ExchangeService** object is for the delegate user. The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Inbox folder.</span></span> 
  
<span data-ttu-id="5e6d2-176">**表 2. 代理人としてメールを操作する EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="5e6d2-176">**Table 2.  EWS Managed API methods working with email as a delegate**</span></span>

|<span data-ttu-id="5e6d2-177">**タスク**</span><span class="sxs-lookup"><span data-stu-id="5e6d2-177">**Task**</span></span>|<span data-ttu-id="5e6d2-178">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="5e6d2-178">**EWS Managed API method**</span></span>|<span data-ttu-id="5e6d2-179">**コード例**</span><span class="sxs-lookup"><span data-stu-id="5e6d2-179">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5e6d2-180">メールを取得する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-180">Get an email</span></span>  <br/> |[<span data-ttu-id="5e6d2-181">Bind</span><span class="sxs-lookup"><span data-stu-id="5e6d2-181">Bind</span></span>](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="5e6d2-182">EWS マネージ API を使用してアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-182">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="5e6d2-183">メールを更新する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-183">Update an email</span></span>  <br/> |<span data-ttu-id="5e6d2-184">[Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) の後に [Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="5e6d2-184">[Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [Update](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="5e6d2-185">EWS マネージ API を使用してアイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-185">Update an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|<span data-ttu-id="5e6d2-186">メールを削除する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-186">Delete an email</span></span>  <br/> |<span data-ttu-id="5e6d2-187">[Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) の後に [Delete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="5e6d2-187">[Bind](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [Delete](http://msdn.microsoft.com/ja-JP/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="5e6d2-188">EWS マネージ API を使用してアイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-188">Delete an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |
   
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="5e6d2-189">EWS を使用して、代理人としてメール アイテムを取得、更新、削除する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-189">Get, update, or delete email items as a delegate by using EWS</span></span>
<span data-ttu-id="5e6d2-190"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="5e6d2-190"></span></span>

<span data-ttu-id="5e6d2-p110">EWS マネージ API を使用すると、代理人アクセスを使用していない場合と同じように、メール アイテムを取得、更新、削除できます。唯一の違いは、サービス オブジェクトが代理ユーザーを対象にしている点です。**GetItem** 要求に含まれるアイテム ID は、メールボックス所有者の受信トレイ フォルダー内のメールボックス ストアにあるアイテムを一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="5e6d2-p110">You can use the EWS Managed API to get, update, or delete an email in the same way that you perform these actions when you're not using delegate access. The only difference is that the service object is for the delegate user. The item ID included in the **GetItem** request uniquely identifies the item in the mailbox store, in the mailbox owner's Inbox folder.</span></span> 
  
<span data-ttu-id="5e6d2-194">**表 3. 代理人としてメールを操作するための EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="5e6d2-194">**Table 3.  EWS operations for working with email as a delegate**</span></span>

|<span data-ttu-id="5e6d2-195">**タスク**</span><span class="sxs-lookup"><span data-stu-id="5e6d2-195">**Task**</span></span>|<span data-ttu-id="5e6d2-196">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="5e6d2-196">**EWS operation**</span></span>|<span data-ttu-id="5e6d2-197">**コード例**</span><span class="sxs-lookup"><span data-stu-id="5e6d2-197">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="5e6d2-198">メールを取得する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-198">Get an email</span></span>  <br/> |[<span data-ttu-id="5e6d2-199">GetItem</span><span class="sxs-lookup"><span data-stu-id="5e6d2-199">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="5e6d2-200">EWS を使用してアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-200">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="5e6d2-201">メールを更新する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-201">Update an email</span></span>  <br/> |<span data-ttu-id="5e6d2-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="5e6d2-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="5e6d2-203">EWS を使用してアイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-203">Update an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|<span data-ttu-id="5e6d2-204">メールを削除する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-204">Delete an email</span></span>  <br/> |<span data-ttu-id="5e6d2-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="5e6d2-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |[<span data-ttu-id="5e6d2-206">EWS を使用してアイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-206">Delete an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="5e6d2-207">関連項目</span><span class="sxs-lookup"><span data-stu-id="5e6d2-207">See also</span></span>

- [<span data-ttu-id="5e6d2-208">Exchange での代理人アクセスと EWS</span><span class="sxs-lookup"><span data-stu-id="5e6d2-208">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)    
- [<span data-ttu-id="5e6d2-209">Exchange で EWS を使用して代理人を追加および削除する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-209">How to: Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="5e6d2-210">Exchange で EWS を使用して別のユーザーのフォルダーのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="5e6d2-210">How to: Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="5e6d2-211">Exchange の予定表と EWS</span><span class="sxs-lookup"><span data-stu-id="5e6d2-211">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    

