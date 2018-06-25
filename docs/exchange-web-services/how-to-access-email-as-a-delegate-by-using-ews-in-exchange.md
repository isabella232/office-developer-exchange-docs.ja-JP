---
title: EWS を使用して Exchange 内で代理人として電子メールにアクセスします。
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: a8123604-c7c0-405d-a0ed-7a9b4a431bfd
description: Exchange で EWS マネージ API または EWS を使用して、代理人としてメールにアクセスする方法を説明します。
ms.openlocfilehash: 8331f337136426913347cf6941d64b4611922d74
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758914"
---
# <a name="access-email-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="581e2-103">EWS を使用して Exchange 内で代理人として電子メールにアクセスします。</span><span class="sxs-lookup"><span data-stu-id="581e2-103">Access email as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="581e2-104">Exchange で EWS マネージ API または EWS を使用して、代理人としてメールにアクセスする方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="581e2-104">Learn how to access email as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="581e2-p101">EWS マネージ API または EWS を使用して、ユーザーにメーボックス所有者の受信トレイ フォルダーへの代理人アクセス権を付与できます。代理人は、メールボックス所有者の代わりに会議出席依頼を作成し、アクセス許可に応じて、メールボックス所有者の受信トレイ フォルダーのメールの検索、取得、更新、削除を行うことができます。</span><span class="sxs-lookup"><span data-stu-id="581e2-p101">You can use the EWS Managed API or EWS to give a user delegate access to a mailbox owner's Inbox folder. The delegate can then create meeting requests on behalf of the mailbox owner, search for email, and retrieve, update, and delete email from the mailbox owner's Inbox folder, depending on their permissions.</span></span>
  
<span data-ttu-id="581e2-107">代理人は、代理人アクセスすることがなく [受信トレイ] フォルダーへのアクセスに使用するメールボックスの所有者の受信トレイ フォルダーにアクセスするのには、同じメソッドと演算を使用します。</span><span class="sxs-lookup"><span data-stu-id="581e2-107">As a delegate, you use the same methods and operations to access a mailbox owner's Inbox folder that you use to access an Inbox folder without delegate access.</span></span> <span data-ttu-id="581e2-108">主な違いは、[明示的なアクセス権](delegate-access-and-ews-in-exchange.md#bk_explicit)を使用して、検索または、電子メール アイテムを作成するのにはあり、その項目の ID を識別した後を実行して[暗黙のアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を取得、更新、またはアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="581e2-108">The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create an email item, and then after you identify the item ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="581e2-109">**表 1 です。EWS のマネージ API のメソッドとデリゲートとして電子メールにアクセスするための EWS の操作**</span><span class="sxs-lookup"><span data-stu-id="581e2-109">**Table 1. EWS Managed API methods and EWS operations for accessing email as a delegate**</span></span>

|<span data-ttu-id="581e2-110">**目的…**</span><span class="sxs-lookup"><span data-stu-id="581e2-110">**If you want to…**</span></span>|<span data-ttu-id="581e2-111">**この EWS 管理 API メソッドを使用してください.**</span><span class="sxs-lookup"><span data-stu-id="581e2-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="581e2-112">**EWS 操作を使用してください.**</span><span class="sxs-lookup"><span data-stu-id="581e2-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="581e2-113">代理人としてメールを作成して送信する</span><span class="sxs-lookup"><span data-stu-id="581e2-113">Create and send an email as a delegate</span></span>  <br/> |<span data-ttu-id="581e2-114">[EmailMessage.Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) [フォルダー Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx)パラメーターが、メールボックスの所有者の [下書き] フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供</span><span class="sxs-lookup"><span data-stu-id="581e2-114">[EmailMessage.Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Drafts folder</span></span>  <br/> <span data-ttu-id="581e2-115">[EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/dd634248%28v=exchg.80%29.aspx) [フォルダー Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx)パラメーターが、メールボックスの所有者の [送信済みアイテム フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供</span><span class="sxs-lookup"><span data-stu-id="581e2-115">[EmailMessage.SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/dd634248%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Sent Items folder</span></span>  <br/> |<span data-ttu-id="581e2-116">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) [メールボックス](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx)要素がメールボックスの所有者の[EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx)を指定</span><span class="sxs-lookup"><span data-stu-id="581e2-116">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> <span data-ttu-id="581e2-117">[SendItem](http://msdn.microsoft.com/library/a966da19-b05a-4504-ac98-91acc1667b9a%28Office.15%29.aspx) [メールボックス](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx)要素がメールボックスの所有者の[EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx)を指定</span><span class="sxs-lookup"><span data-stu-id="581e2-117">[SendItem](http://msdn.microsoft.com/library/a966da19-b05a-4504-ac98-91acc1667b9a%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="581e2-118">代理人として複数のメール メッセージを作成する</span><span class="sxs-lookup"><span data-stu-id="581e2-118">Create multiple email messages as a delegate</span></span>  <br/> |<span data-ttu-id="581e2-119">[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) **フォルダー Id**パラメーターが、メールボックスの所有者の受信トレイ フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供</span><span class="sxs-lookup"><span data-stu-id="581e2-119">[ExchangeService.CreateItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Inbox folder</span></span>  <br/> |<span data-ttu-id="581e2-120">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) [メールボックス](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx)要素がメールボックスの所有者の[EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx)を指定</span><span class="sxs-lookup"><span data-stu-id="581e2-120">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="581e2-121">代理人としてメールを検索する</span><span class="sxs-lookup"><span data-stu-id="581e2-121">Search for or find an email as a delegate</span></span>  <br/> |<span data-ttu-id="581e2-122">[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) **フォルダー Id**パラメーターが、メールボックスの所有者の受信トレイ フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供</span><span class="sxs-lookup"><span data-stu-id="581e2-122">[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Inbox folder</span></span>  <br/> |<span data-ttu-id="581e2-123">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) [メールボックス](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx)要素がメールボックスの所有者の[EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx)を指定</span><span class="sxs-lookup"><span data-stu-id="581e2-123">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="581e2-124">代理人としてメールを取得</span><span class="sxs-lookup"><span data-stu-id="581e2-124">Get an email as a delegate</span></span>  <br/> |[<span data-ttu-id="581e2-125">EmailMessage.Bind</span><span class="sxs-lookup"><span data-stu-id="581e2-125">EmailMessage.Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="581e2-126">GetItem</span><span class="sxs-lookup"><span data-stu-id="581e2-126">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="581e2-127">代理人としてメールを更新する</span><span class="sxs-lookup"><span data-stu-id="581e2-127">Update an email as a delegate</span></span>  <br/> |<span data-ttu-id="581e2-128">[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)の後に</span><span class="sxs-lookup"><span data-stu-id="581e2-128">[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [EmailMessage.Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="581e2-129">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)に続いて</span><span class="sxs-lookup"><span data-stu-id="581e2-129">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="581e2-130">代理人としてメールを削除する</span><span class="sxs-lookup"><span data-stu-id="581e2-130">Delete an email as a delegate</span></span>  <br/> |<span data-ttu-id="581e2-131">[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) [EmailMessage.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)の後に</span><span class="sxs-lookup"><span data-stu-id="581e2-131">[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [EmailMessage.Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="581e2-132">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)の後に</span><span class="sxs-lookup"><span data-stu-id="581e2-132">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span></span> <br/> |
   
<span data-ttu-id="581e2-133">代理人としてメールを操作する場合、次の点に注意してください。</span><span class="sxs-lookup"><span data-stu-id="581e2-133">Keep the following things in mind when working with emails as a delegate:</span></span>
  
- <span data-ttu-id="581e2-134">デリゲートは、会議出席依頼や出欠の返答を操作するだけ必要とする場合、デリゲートは、[受信トレイ] フォルダーへのアクセスを必要はありません。</span><span class="sxs-lookup"><span data-stu-id="581e2-134">If a delegate only needs to work with meeting requests and responses, the delegate does not need access to the Inbox folder.</span></span> <span data-ttu-id="581e2-135">詳細については、[代理人に予定表にアクセスするための前提条件のタスク](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md#bk_prereq)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="581e2-135">For more information, see [prerequisite tasks for accessing calendars as a delegate](how-to-access-a-calendar-as-a-delegate-by-using-ews-in-exchange.md#bk_prereq).</span></span>
    
- <span data-ttu-id="581e2-136">受信者は、メールボックス所有者の代理として送信されたメッセージを受信する「*代理人**のメールボックス所有者*の代理として。」として、送信者が表示されます。</span><span class="sxs-lookup"><span data-stu-id="581e2-136">When a recipient receives a message that was sent on behalf of a mailbox owner, the sender appears as " *Delegate*  on behalf of  *mailbox owner*  ."</span></span> 
    
> [!NOTE]
> <span data-ttu-id="581e2-137">この記事のコード例では、primary@contoso.com がメールボックス所有者です。</span><span class="sxs-lookup"><span data-stu-id="581e2-137">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 
  
## <a name="prerequisite-tasks"></a><span data-ttu-id="581e2-138">事前に必要なタスク</span><span class="sxs-lookup"><span data-stu-id="581e2-138">Prerequisite tasks</span></span>
<span data-ttu-id="581e2-139"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="581e2-139"></span></span>

<span data-ttu-id="581e2-140">ユーザーは、メールボックス所有者の代理人として受信トレイ] フォルダーにアクセスできる、前にメールボックスの所有者の受信トレイ フォルダーに[アクセス許可を持つ代理人として追加](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)のユーザーである必要があります。</span><span class="sxs-lookup"><span data-stu-id="581e2-140">Before a user can access the mailbox owner's Inbox folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Inbox folder.</span></span> 
  
## <a name="create-and-send-an-email-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="581e2-141">EWS マネージ API を使用して、代理人としてメールを作成および送信する</span><span class="sxs-lookup"><span data-stu-id="581e2-141">Create and send an email as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="581e2-142"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="581e2-142"></span></span>

<span data-ttu-id="581e2-143">EWS のマネージ API を使用すると、代理ユーザーのサービス オブジェクトを使用して作成し、メールボックス所有者の代理として電子メールを送信できます。</span><span class="sxs-lookup"><span data-stu-id="581e2-143">The EWS Managed API enables you to use the service object for the delegate user to create and send email on behalf of the mailbox owner.</span></span> <span data-ttu-id="581e2-144">この例では、[保存](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx)されたメッセージをメールボックスの所有者の [下書き] フォルダーに保存して、メールを送信し、メッセージをメールボックスの所有者の [送信済みアイテム フォルダーに保存するには、 [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/dd634248%28v=exchg.80%29.aspx)メソッドを使用する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="581e2-144">This example shows how to use the [Save](http://msdn.microsoft.com/en-us/library/dd635209%28v=exchg.80%29.aspx) method to save the message in the mailbox owner's Drafts folder, and then the [SendAndSaveCopy](http://msdn.microsoft.com/en-us/library/dd634248%28v=exchg.80%29.aspx) method to send the mail and save the message in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="581e2-145">この例ではその**サービス**は、デリゲートの有効な[ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトと代理人に[メールボックスの所有者の受信トレイ、下書き、送信済みアイテム フォルダーに対して適切なアクセス許可](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)が付与されています。</span><span class="sxs-lookup"><span data-stu-id="581e2-145">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the [appropriate permissions for the mailbox owner's Inbox, Drafts, and Sent Items folder](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md).</span></span>
  
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

## <a name="create-and-send-an-email-as-a-delegate-by-using-ews"></a><span data-ttu-id="581e2-146">EWS を使用して代理人としてメールを作成して送信する</span><span class="sxs-lookup"><span data-stu-id="581e2-146">Create and send an email as a delegate by using EWS</span></span>
<span data-ttu-id="581e2-147"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="581e2-147"></span></span>

<span data-ttu-id="581e2-148">EWS を使用すると、代理ユーザーのサービス オブジェクトを使用して作成し、メールボックス所有者の代理として電子メールを送信できます。</span><span class="sxs-lookup"><span data-stu-id="581e2-148">EWS enables you to use the service object for the delegate user to create and send email on behalf of the mailbox owner.</span></span> <span data-ttu-id="581e2-149">次の使用例は、 [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx)操作を使用して、電子メールと[SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx)操作の時間を送信し、メールボックスの所有者の [送信済みアイテム フォルダーに保存するを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="581e2-149">This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create an email and the [SendItem](http://msdn.microsoft.com/library/337b89ef-e1b7-45ed-92f3-8abe4200e4c7%28Office.15%29.aspx) operation to send the time and save it in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="581e2-150">これは、最初の XML 要求**を保存**するメソッド[を作成し電子メールで送信](#bk_createewsma)を使用する場合、EWS のマネージ API を送信します。</span><span class="sxs-lookup"><span data-stu-id="581e2-150">This is also the first XML request that the EWS Managed API sends when you use the **Save** method to [create and send an email](#bk_createewsma).</span></span>
  
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

<span data-ttu-id="581e2-151">サーバーは、 **CreateItem**要求**NoError**電子メールが作成され、正常に保存されたことを示すは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値を含む[CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx)メッセージに応答します。</span><span class="sxs-lookup"><span data-stu-id="581e2-151">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the email was created and saved successfully.</span></span> <span data-ttu-id="581e2-152">応答には、新しく作成された電子メールの項目の ID も含まれています。</span><span class="sxs-lookup"><span data-stu-id="581e2-152">The response also contains the item ID of the newly created email.</span></span>
  
<span data-ttu-id="581e2-153">**ItemId**の値が小さすぎると読みやすくするためです。</span><span class="sxs-lookup"><span data-stu-id="581e2-153">The **ItemId** value has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="581e2-154">**SendItem**操作を使用してメールボックス所有者の代理としてメッセージを送信し、メールボックスの所有者の [送信済みアイテム フォルダーに保存します。</span><span class="sxs-lookup"><span data-stu-id="581e2-154">Next, use the **SendItem** operation to send the message on behalf of the mailbox owner and save it in the mailbox owner's Sent Items folder.</span></span> 
  
<span data-ttu-id="581e2-155">**ItemId**の値が小さすぎると読みやすくするためです。</span><span class="sxs-lookup"><span data-stu-id="581e2-155">The **ItemId** value has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="581e2-156">サーバー要求に応答し、 **SendItem** **NoError**電子メールが送信され、メールボックスの所有者の [送信済みアイテム フォルダーに保存されることを示すは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値が含まれています[SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx)メッセージ正常にします。</span><span class="sxs-lookup"><span data-stu-id="581e2-156">The server responds to the **SendItem** request with a [SendItemResponse](http://msdn.microsoft.com/library/26ac41c7-57d9-473e-ab7a-bae93e1d2aba%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the email was sent and saved to the mailbox owner's Sent Items folder successfully.</span></span>
  
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

## <a name="search-for-an-email-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="581e2-157">EWS マネージ API を使用して、代理人としてメールを検索する</span><span class="sxs-lookup"><span data-stu-id="581e2-157">Search for an email as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="581e2-158"><a name="bk_searchewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="581e2-158"></span></span>

<span data-ttu-id="581e2-159">電子メールを検索するにする必要があります使用する[フォルダー Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx)パラメーターを含む[ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx)の方法のいずれかのメールボックスの所有者の受信トレイ フォルダーを指定することができますように。</span><span class="sxs-lookup"><span data-stu-id="581e2-159">To search for an email, you must use one of the [ExchangeService.FindItems](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) methods that includes a [FolderId](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Inbox folder.</span></span> 
  
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

<span data-ttu-id="581e2-160">**FindItems**の呼び出しには、ID を使用して応答が返されます後を表示できるよう、更新または削除 ID および[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)- を使用して電子メールを送信する必要はありませんメールボックス所有者の SMTP アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="581e2-160">After the **FindItems** call returns a response with an ID, you can get, update or delete that email by using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) - and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="search-for-an-email-as-a-delegate-by-using-ews"></a><span data-ttu-id="581e2-161">EWS を使用して代理人としてメールを検索する</span><span class="sxs-lookup"><span data-stu-id="581e2-161">Search for an email as a delegate by using EWS</span></span>
<span data-ttu-id="581e2-162"><a name="bk_searchews"> </a></span><span class="sxs-lookup"><span data-stu-id="581e2-162"></span></span>

<span data-ttu-id="581e2-163">EWS を使用すると、代理ユーザーのサービス オブジェクトを使用して、検索条件のセットに一致する電子メールを検索することができます。</span><span class="sxs-lookup"><span data-stu-id="581e2-163">EWS enables you to use the service object for the delegate user to search for emails that meet a set of search criteria.</span></span> <span data-ttu-id="581e2-164">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx)操作を使用して、件名に「サッカー」という単語が含まれている所有者の受信トレイ フォルダーのメッセージを検索する方法を次の使用例に示します。</span><span class="sxs-lookup"><span data-stu-id="581e2-164">This example shows how to use the [FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) operation to find messages in the owner's Inbox folder that contain the word "soccer" in the subject.</span></span> 
  
<span data-ttu-id="581e2-165">これは、XML の要求の場合、EWS のマネージ API を送信する[電子メールの検索](#bk_searchewsma)をします。</span><span class="sxs-lookup"><span data-stu-id="581e2-165">This is also the XML request that the EWS Managed API sends when you [search for an email](#bk_searchewsma).</span></span>
  
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

<span data-ttu-id="581e2-166">**FindItem**要求に対して、 **NoError**を示すは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値の検索が正常に完了を含む[FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx)メッセージは、サーバーが応答します。</span><span class="sxs-lookup"><span data-stu-id="581e2-166">The server responds to the **FindItem** request with a [FindItemResponse](http://msdn.microsoft.com/library/c8b316df-d4ab-49b8-96d4-8e9a016730ef%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the search completed successfully.</span></span> <span data-ttu-id="581e2-167">応答には、検索条件に一致するすべての電子メールの[メッセージ](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx)の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="581e2-167">The response contains a [Message](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) element for any emails that met the search criteria.</span></span> <span data-ttu-id="581e2-168">この例では、1 つだけのメールが見つかりました。</span><span class="sxs-lookup"><span data-stu-id="581e2-168">In this case, only one email is found.</span></span> 
  
<span data-ttu-id="581e2-169">[ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) 要素の値は読みやすいよう短縮されています。</span><span class="sxs-lookup"><span data-stu-id="581e2-169">The value of the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) element has been shortened for readability.</span></span> 
  
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

<span data-ttu-id="581e2-170">条件を満たす電子メール**アイテム Id**がある場合は、これで表示できるように、update、または delete の**ItemId**と[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)- を使用して電子メールを送信する必要はありませんメールボックス所有者の SMTP アドレスを指定します。</span><span class="sxs-lookup"><span data-stu-id="581e2-170">Now that you have the **ItemId** for the email that meets your criteria, you can get, update, or delete that email by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) - and you do not need to specify the mailbox owner's SMTP address.</span></span> 
  
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="581e2-171">EWS マネージ API を使用して、代理人としてメール アイテムを取得、更新、削除する</span><span class="sxs-lookup"><span data-stu-id="581e2-171">Get, update, or delete email items as a delegate by using the EWS Managed API</span></span>
<span data-ttu-id="581e2-172"><a name="bk_geteswma"> </a></span><span class="sxs-lookup"><span data-stu-id="581e2-172"></span></span>

<span data-ttu-id="581e2-173">取得、更新、または代理人アクセスを使用していないときにこれらのアクションを実行すると同じ方法で電子メールを削除するのには、EWS のマネージ API を使用できます。</span><span class="sxs-lookup"><span data-stu-id="581e2-173">You can use the EWS Managed API to get, update, or delete an email in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="581e2-174">唯一の違いは、 **ExchangeService**オブジェクトの代理人のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="581e2-174">The only difference is that the **ExchangeService** object is for the delegate user.</span></span> <span data-ttu-id="581e2-175">**バインド**メソッドの呼び出しを一意に含まれる項目 ID では、メールボックスの所有者の受信トレイ フォルダーに、メールボックス ストア内の項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="581e2-175">The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Inbox folder.</span></span> 
  
<span data-ttu-id="581e2-176">**表 2 になります。EWS のマネージ API のメソッドを代理人に電子メールを使用**</span><span class="sxs-lookup"><span data-stu-id="581e2-176">**Table 2. EWS Managed API methods working with email as a delegate**</span></span>

|<span data-ttu-id="581e2-177">**タスク**</span><span class="sxs-lookup"><span data-stu-id="581e2-177">**Task**</span></span>|<span data-ttu-id="581e2-178">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="581e2-178">**EWS Managed API method**</span></span>|<span data-ttu-id="581e2-179">**コードの例**</span><span class="sxs-lookup"><span data-stu-id="581e2-179">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="581e2-180">メールを取得する</span><span class="sxs-lookup"><span data-stu-id="581e2-180">Get an email</span></span>  <br/> |[<span data-ttu-id="581e2-181">バインド</span><span class="sxs-lookup"><span data-stu-id="581e2-181">Bind</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="581e2-182">EWS のマネージ API を使用してアイテムを取得します。</span><span class="sxs-lookup"><span data-stu-id="581e2-182">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="581e2-183">メールを更新する</span><span class="sxs-lookup"><span data-stu-id="581e2-183">Update an email</span></span>  <br/> |<span data-ttu-id="581e2-184">[バインド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx)[の更新](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)の後に</span><span class="sxs-lookup"><span data-stu-id="581e2-184">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [Update](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="581e2-185">EWS のマネージ API を使用してアイテムを更新します。</span><span class="sxs-lookup"><span data-stu-id="581e2-185">Update an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|<span data-ttu-id="581e2-186">メールを削除する</span><span class="sxs-lookup"><span data-stu-id="581e2-186">Delete an email</span></span>  <br/> |<span data-ttu-id="581e2-187">の[バインド](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx)[を削除](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)後に</span><span class="sxs-lookup"><span data-stu-id="581e2-187">[Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) followed by [Delete](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="581e2-188">EWS のマネージ API を使用して項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="581e2-188">Delete an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |
   
## <a name="get-update-or-delete-email-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="581e2-189">EWS を使用して、代理人としてメール アイテムを取得、更新、削除する</span><span class="sxs-lookup"><span data-stu-id="581e2-189">Get, update, or delete email items as a delegate by using EWS</span></span>
<span data-ttu-id="581e2-190"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="581e2-190"></span></span>

<span data-ttu-id="581e2-191">取得、更新、または代理人アクセスを使用していないときにこれらのアクションを実行すると同じ方法で電子メールを削除するのには、EWS のマネージ API を使用できます。</span><span class="sxs-lookup"><span data-stu-id="581e2-191">You can use the EWS Managed API to get, update, or delete an email in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="581e2-192">唯一の違いは、サービス オブジェクトの代理人のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="581e2-192">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="581e2-193">**GetItem**要求内で一意に含まれている項目の ID は、メールボックスの所有者の受信トレイ フォルダーに、メールボックス ストア内の項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="581e2-193">The item ID included in the **GetItem** request uniquely identifies the item in the mailbox store, in the mailbox owner's Inbox folder.</span></span> 
  
<span data-ttu-id="581e2-194">**表 3。代理人に電子メールを操作するための EWS の操作**</span><span class="sxs-lookup"><span data-stu-id="581e2-194">**Table 3. EWS operations for working with email as a delegate**</span></span>

|<span data-ttu-id="581e2-195">**タスク**</span><span class="sxs-lookup"><span data-stu-id="581e2-195">**Task**</span></span>|<span data-ttu-id="581e2-196">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="581e2-196">**EWS operation**</span></span>|<span data-ttu-id="581e2-197">**コードの例**</span><span class="sxs-lookup"><span data-stu-id="581e2-197">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="581e2-198">メールを取得する</span><span class="sxs-lookup"><span data-stu-id="581e2-198">Get an email</span></span>  <br/> |[<span data-ttu-id="581e2-199">GetItem</span><span class="sxs-lookup"><span data-stu-id="581e2-199">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="581e2-200">EWS を使用してアイテムを取得します。</span><span class="sxs-lookup"><span data-stu-id="581e2-200">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="581e2-201">メールを更新する</span><span class="sxs-lookup"><span data-stu-id="581e2-201">Update an email</span></span>  <br/> |<span data-ttu-id="581e2-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)に続いて</span><span class="sxs-lookup"><span data-stu-id="581e2-202">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="581e2-203">EWS を使用してアイテムを更新します。</span><span class="sxs-lookup"><span data-stu-id="581e2-203">Update an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|<span data-ttu-id="581e2-204">メールを削除する</span><span class="sxs-lookup"><span data-stu-id="581e2-204">Delete an email</span></span>  <br/> |<span data-ttu-id="581e2-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)の後に</span><span class="sxs-lookup"><span data-stu-id="581e2-205">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="581e2-206">EWS を使用して項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="581e2-206">Delete an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="581e2-207">関連項目</span><span class="sxs-lookup"><span data-stu-id="581e2-207">See also</span></span>

- [<span data-ttu-id="581e2-208">Exchange での代理人アクセスと EWS</span><span class="sxs-lookup"><span data-stu-id="581e2-208">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)    
- [<span data-ttu-id="581e2-209">追加し、Exchange の EWS を使用して、デリゲートを削除します。</span><span class="sxs-lookup"><span data-stu-id="581e2-209">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="581e2-210">Exchange EWS を使用して別のユーザーのフォルダーのアクセス許可を設定します。</span><span class="sxs-lookup"><span data-stu-id="581e2-210">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)    
- [<span data-ttu-id="581e2-211">Calendars and EWS in Exchange</span><span class="sxs-lookup"><span data-stu-id="581e2-211">Calendars and EWS in Exchange</span></span>](calendars-and-ews-in-exchange.md)
    

