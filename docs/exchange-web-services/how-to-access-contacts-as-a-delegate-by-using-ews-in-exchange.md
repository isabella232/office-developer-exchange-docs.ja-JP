---
title: Exchange EWS を使用して代理人としてアクセス連絡先
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3cd34c14-18b0-4fe2-a4c2-d884318c88fc
description: Exchange の EWS マネージ API または EWS を使用して、代理人として連絡先にアクセスする方法を説明します。
ms.openlocfilehash: a7f695dcbe0693809817de84284294dff872aa9c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758913"
---
# <a name="access-contacts-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="b9b4a-103">Exchange EWS を使用して代理人としてアクセス連絡先</span><span class="sxs-lookup"><span data-stu-id="b9b4a-103">Access contacts as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="b9b4a-104">Exchange の EWS マネージ API または EWS を使用して、代理人として連絡先にアクセスする方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-104">Learn how to access contacts as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="b9b4a-p101">EWS マネージ API または EWS を使用して、ユーザーにメールボックス所有者の連絡先フォルダーへのアクセス権を付与できます。代理人は、メールボックス所有者の代わりに連絡先を作成し、アクセス許可に応じて、メールボックス所有者の連絡先フォルダーから連絡先を取得、更新、および削除することができます。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-p101">You can use the EWS Managed API or EWS to give a user access to a mailbox owner's Contacts folder. The delegate can then create contacts on behalf of the mailbox owner, and retrieve, update, and delete contacts from the mailbox owner's Contacts folder, depending on their permissions.</span></span>
  
<span data-ttu-id="b9b4a-107">代理人は、自分の連絡先フォルダーへのアクセスに使用するメールボックスの所有者の連絡先フォルダーにアクセスするのには、同じメソッドと演算を使用します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-107">As a delegate, you use the same methods and operations to access a mailbox owner's Contacts folder that you use to access your own Contacts folder.</span></span> <span data-ttu-id="b9b4a-108">主な違いは[明示的なアクセス権](delegate-access-and-ews-in-exchange.md#bk_explicit)を使用して検索したり、連絡先アイテムを作成するのにはあり、その項目の ID を識別した後を実行して[暗黙のアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を取得、更新、またはアイテムを削除します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-108">The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create a contact item, and then after you identify the item ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="b9b4a-109">**表 1 です。EWS のマネージ API のメソッドと代理人の連絡先にアクセスするための EWS の操作**</span><span class="sxs-lookup"><span data-stu-id="b9b4a-109">**Table 1. EWS Managed API methods and EWS operations for accessing a contact as a delegate**</span></span>

|<span data-ttu-id="b9b4a-110">**目的…**</span><span class="sxs-lookup"><span data-stu-id="b9b4a-110">**If you want to…**</span></span>|<span data-ttu-id="b9b4a-111">**この EWS 管理 API メソッドを使用してください.**</span><span class="sxs-lookup"><span data-stu-id="b9b4a-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="b9b4a-112">**EWS 操作を使用してください.**</span><span class="sxs-lookup"><span data-stu-id="b9b4a-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b9b4a-113">代理人として連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-113">Create a contact as a delegate</span></span>  <br/> |<span data-ttu-id="b9b4a-114">[Item.Save](http://msdn.microsoft.com/ja-jp/library/dd635209%28v=exchg.80%29.aspx) [フォルダー Id](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx)パラメーターが、メールボックスの所有者の連絡先フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供</span><span class="sxs-lookup"><span data-stu-id="b9b4a-114">[Item.Save](http://msdn.microsoft.com/ja-jp/library/dd635209%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="b9b4a-115">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) [メールボックス](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx)要素がメールボックスの所有者の[EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx)を指定</span><span class="sxs-lookup"><span data-stu-id="b9b4a-115">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="b9b4a-116">代理人として複数の連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-116">Create multiple contacts as a delegate</span></span>  <br/> |<span data-ttu-id="b9b4a-117">[ExchangeService.CreateItems](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) **フォルダー Id**パラメーターが、メールボックスの所有者の連絡先フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供</span><span class="sxs-lookup"><span data-stu-id="b9b4a-117">[ExchangeService.CreateItems](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="b9b4a-118">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) [メールボックス](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx)要素がメールボックスの所有者の[EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx)を指定</span><span class="sxs-lookup"><span data-stu-id="b9b4a-118">[CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="b9b4a-119">代理人として連絡先を解決する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-119">Resolve a contact as a delegate</span></span>  <br/> |<span data-ttu-id="b9b4a-120">[ExchangeService.ResolveName](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) [フォルダー Id](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx)パラメーターが、メールボックスの所有者の連絡先フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供</span><span class="sxs-lookup"><span data-stu-id="b9b4a-120">[ExchangeService.ResolveName](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) where the [FolderId](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="b9b4a-121">[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) [メールボックス](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx)要素がメールボックスの所有者の[EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx)を指定</span><span class="sxs-lookup"><span data-stu-id="b9b4a-121">[ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="b9b4a-122">代理人として連絡先を検索する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-122">Search for or find a contact as a delegate</span></span>  <br/> |<span data-ttu-id="b9b4a-123">[ExchangeService.FindItems](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) **フォルダー Id**パラメーターが、メールボックスの所有者の連絡先フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供</span><span class="sxs-lookup"><span data-stu-id="b9b4a-123">[ExchangeService.FindItems](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="b9b4a-124">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) [メールボックス](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx)要素がメールボックスの所有者の[EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx)を指定</span><span class="sxs-lookup"><span data-stu-id="b9b4a-124">[FindItem](http://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](http://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](http://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="b9b4a-125">代理人として連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-125">Get a contact as a delegate</span></span>  <br/> |[<span data-ttu-id="b9b4a-126">Contact.Bind</span><span class="sxs-lookup"><span data-stu-id="b9b4a-126">Contact.Bind</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="b9b4a-127">GetItem</span><span class="sxs-lookup"><span data-stu-id="b9b4a-127">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="b9b4a-128">代理人として連絡先を更新する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-128">Update a contact as a delegate</span></span>  <br/> |<span data-ttu-id="b9b4a-129">[Contact.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) [Contact.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx)の後に</span><span class="sxs-lookup"><span data-stu-id="b9b4a-129">[Contact.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) followed by [Contact.Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="b9b4a-130">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)に続いて</span><span class="sxs-lookup"><span data-stu-id="b9b4a-130">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="b9b4a-131">代理人として連絡先を削除する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-131">Delete a contact as a delegate</span></span>  <br/> |<span data-ttu-id="b9b4a-132">[Contact.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) [Contact.Delete](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)の後に</span><span class="sxs-lookup"><span data-stu-id="b9b4a-132">[Contact.Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) followed by [Contact.Delete](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="b9b4a-133">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)の後に</span><span class="sxs-lookup"><span data-stu-id="b9b4a-133">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span></span> <br/> |
   
> [!NOTE]
> <span data-ttu-id="b9b4a-134">この記事のコード例では、primary@contoso.com がメールボックス所有者です。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-134">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 

<span data-ttu-id="b9b4a-135"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="b9b4a-135"></span></span>

## <a name="prerequisite-tasks"></a><span data-ttu-id="b9b4a-136">事前に必要なタスク</span><span class="sxs-lookup"><span data-stu-id="b9b4a-136">Prerequisite tasks</span></span>

<span data-ttu-id="b9b4a-137">ユーザーは、代理人のメールボックスの所有者の連絡先フォルダーにアクセスできる、前に、ユーザーがメールボックスの所有者の連絡先フォルダーに[アクセス許可を持つ代理人として追加](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)をする必要があります。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-137">Before a user can access the mailbox owner's Contacts folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Contacts folder.</span></span> 

<span data-ttu-id="b9b4a-138"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b9b4a-138"></span></span>

## <a name="create-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="b9b4a-139">EWS マネージ API を使用して、代理人として連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-139">Create a contact as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="b9b4a-140">EWS のマネージ API を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックスの所有者の連絡先を作成することができます。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-140">The EWS Managed API enables you to use the service object for the delegate user to create contacts for the mailbox owner.</span></span> <span data-ttu-id="b9b4a-141">この例では、 [Save](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx)メソッドを使用して、会議を作成し、出席者に会議出席依頼を送信する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-141">This example shows how to use the [Save](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="b9b4a-142">この例ではその**サービス**は、デリゲートの有効な[ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx)オブジェクトと代理人にメールボックスの所有者の連絡先フォルダーの適切なアクセス許可が付与されています。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-142">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the appropriate permissions for the mailbox owner's Contacts folder.</span></span> 
  
```cs
 public static void DelegateAccessCreateContact(ExchangeService service)
{
    // Create the contact.
    Contact contact = new Contact(service);
    // Specify the name and how the contact should be filed.
    contact.GivenName = "Brian";
    contact.MiddleName = "David";
    contact.Surname = "Johnson";
    contact.FileAsMapping = FileAsMapping.SurnameCommaGivenName;
    // Specify the company name.
    contact.CompanyName = "Contoso";
    // Specify the business, home, and car phone numbers.
    contact.PhoneNumbers[PhoneNumberKey.BusinessPhone] = "425-555-0110";
    contact.PhoneNumbers[PhoneNumberKey.HomePhone] = "425-555-0120";
    contact.PhoneNumbers[PhoneNumberKey.CarPhone] = "425-555-0130";
    // Specify two email addresses.
    contact.EmailAddresses[EmailAddressKey.EmailAddress1] = 
        new EmailAddress("brian_1@contoso.com");
    contact.EmailAddresses[EmailAddressKey.EmailAddress2] = 
        new EmailAddress("brian_2@contoso.com");
    // Save the contact in the mailbox owner's Contacts folder.
    // This method call results in a CreateItem call to EWS. 
    // The contact identifier contains the context for the mailbox owner's 
    // Contact folder. Any additional actions take on this contact will 
    // be performed in the mailbox owner's mailbox. 
    contact.Save(new FolderId(WellKnownFolderName.Contacts, 
        "primary@contoso.com"));
    // Verify that the contact was created.
    // This method call results in a GetItem call to EWS
    // to load the display name property on the contact. 
    contact.Load(new PropertySet (ContactSchema.DisplayName));
    Console.WriteLine("\nContact created: " + contact.DisplayName + "\n");
}
```

<span data-ttu-id="b9b4a-143">アイテムを保存するとき[保存](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx)メソッドの呼び出しは、メールボックスの所有者の連絡先フォルダーを識別する必要があることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-143">Note that when you save the item, the [Save](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method call must identify the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="b9b4a-144">メールボックスの所有者の連絡先フォルダーを指定しない場合、会議出席依頼が代理人の連絡先フォルダーおよびメールボックスの所有者の連絡先フォルダーではなく保存されます。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-144">If the mailbox owner's Contacts folder is not specified, the meeting request gets saved to the delegate's Contacts folder and not the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="b9b4a-145">**保存**メソッドの呼び出しで 2 つの方法では、メールボックスの所有者の連絡先フォルダーを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-145">You can include the mailbox owner's Contacts folder in the **Save** method call in two way.</span></span> <span data-ttu-id="b9b4a-146">[WellKnownFolderName](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx)とメールボックス所有者の SMTP アドレスを使用して、[フォルダー Id](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx)のオブジェクトの新しいインスタンスをインスタンス化することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-146">We recommend that you instantiate a new instance of the [FolderId](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) object by using the [WellKnownFolderName](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) and the SMTP address of the mailbox owner.</span></span> 
  
```cs
contact.Save(new FolderId(WellKnownFolderName.Contacts, "primary@contoso.com"));
```

<span data-ttu-id="b9b4a-147">ただし、することも[バインド](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx)の連絡先フォルダーに最初に、し、**保存**メソッドの呼び出し内のフォルダーの ID を使用します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-147">However, you can also [Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) to the Contacts folder first, and then use the ID of the folder in the **Save** method call.</span></span> <span data-ttu-id="b9b4a-148">注意してください、ただし、この EWS 呼び出しを作成します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-148">Be aware, however, that this creates an extra EWS call.</span></span> 
  
```cs
    // Identify the mailbox owner's SMTP address 
    // and bind to their Contacts folder.
    Mailbox primary = new Mailbox("primary@contoso.com"); 
    Folder primaryContacts = Folder.Bind(service, new FolderId(WellKnownFolderName.Contacts, primary)); 
…
    // Save the contact to the mailbox owner's Contacts folder.
    meeting.Save(primaryContacts.Id);
```

<span data-ttu-id="b9b4a-149"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="b9b4a-149"></span></span>

## <a name="create-a-contact-as-a-delegate-by-using-ews"></a><span data-ttu-id="b9b4a-150">EWS を使用して、代理人として連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-150">Create a contact as a delegate by using EWS</span></span>

<span data-ttu-id="b9b4a-151">EWS を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックスの所有者の連絡先アイテムを作成することができます。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-151">EWS enables you to use the service object for the delegate user to create contact items for the mailbox owner.</span></span> <span data-ttu-id="b9b4a-152">次の使用例は、 [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx)操作を使用して連絡先を作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-152">This example shows how to use the [CreateItem](http://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a contact.</span></span> 
  
<span data-ttu-id="b9b4a-153">EWS のマネージ API が[、連絡先を作成](#bk_createewsma)するのには**Save**メソッドを使用する場合に送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-153">This is also the XML request that the EWS Managed API sends when you use the **Save** method to [create a contact](#bk_createewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="contacts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:SavedItemFolderId>
      <m:Items>
        <t:Contact>
          <t:FileAsMapping>LastCommaFirst</t:FileAsMapping>
          <t:GivenName>Brian</t:GivenName>
          <t:MiddleName>David</t:MiddleName>
          <t:CompanyName>Contoso</t:CompanyName>
          <t:EmailAddresses>
            <t:Entry Key="EmailAddress1">brian_1@contoso.com</t:Entry>
            <t:Entry Key="EmailAddress2">brian_2@contoso.com</t:Entry>
          </t:EmailAddresses>
          <t:PhoneNumbers>
            <t:Entry Key="BusinessPhone">425-555-0110</t:Entry>
            <t:Entry Key="HomePhone">425-555-0120</t:Entry>
            <t:Entry Key="CarPhone">425-555-0130</t:Entry>
          </t:PhoneNumbers>
          <t:Surname>Johnson</t:Surname>
        </t:Contact>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="b9b4a-154">サーバーは、 **CreateItem**要求**NoError**連絡先が正常に作成されたことを示すは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値を含む[CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx)メッセージに応答します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-154">The server responds to the **CreateItem** request with a [CreateItemResponse](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the contact was created successfully.</span></span> <span data-ttu-id="b9b4a-155">応答には、新しく作成された連絡先の項目の ID も含まれています。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-155">The response also contains the item ID of the newly created contact.</span></span>

<span data-ttu-id="b9b4a-156"><a name="bk_resolveewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b9b4a-156"></span></span>

## <a name="resolve-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="b9b4a-157">EWS マネージ API を使用して、代理人として連絡先を解決する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-157">Resolve a contact as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="b9b4a-158">可能性のあるあいまいな名前または語句に基づいて連絡先を検索するには、必要があります使用する[フォルダー Id](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx)パラメーターを含む[ExchangeService.ResolveName](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx)の方法のいずれかのメールボックスの所有者の連絡先フォルダーを指定することができますように。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-158">To find a contact based on a possibly ambiguous name or term, you must use one of the [ExchangeService.ResolveName](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) methods that includes a [FolderId](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Contacts folder.</span></span> 
  
```cs
private static void DelegateAccessResolveContacts(ExchangeService service)
{
    // Create a list to store folders to search.
    List<FolderId> folders = new List<FolderId>();
   
    // Add the mailbox owner's folder to the list.
    folders.Add(new FolderId(WellKnownFolderName.Contacts, 
        "primary@contoso.com"));
    
    // Resolve the ambiguous name "Johnson".
    // This method call results in a ResolveNames call to EWS.
    NameResolutionCollection resolvedNames = service.ResolveName(
        "johnson", folders, ResolveNameSearchLocation.ContactsOnly, true);
    // Output the list of candidate email addresses and contact names.
    foreach (NameResolution nameRes in resolvedNames)
    {
        Console.WriteLine("Contact e-mail address: " + nameRes.Mailbox.Address);
        Console.WriteLine("Contact ID: " + nameRes.Mailbox.Id);
    }
}
```

<span data-ttu-id="b9b4a-159">**ResolveNames**メソッドの呼び出しには、ID を使用して応答が返された後、することができます[を取得、更新、または取引先担当者を削除](#bk_getewsma)ID と[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用して&mdash;と、メールボックス所有者の SMTP アドレスを指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-159">After the **ResolveNames** method call returns a response with an ID, you can [get, update or delete the contact](#bk_getewsma) using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;and you do not need to specify the mailbox owner's SMTP address.</span></span> 

<span data-ttu-id="b9b4a-160"><a name="bk_resolveews"> </a></span><span class="sxs-lookup"><span data-stu-id="b9b4a-160"></span></span>

## <a name="resolve-a-contact-as-a-delegate-by-using-ews"></a><span data-ttu-id="b9b4a-161">EWS を使用して、代理人として連絡先を解決する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-161">Resolve a contact as a delegate by using EWS</span></span>

<span data-ttu-id="b9b4a-162">EWS を使用すると、メールボックスの所有者の連絡先フォルダーの名前の一部を解決するのには代理人のユーザーのサービス オブジェクトを使用できます。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-162">EWS enables you to use the service object for the delegate user to resolve partial names in the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="b9b4a-163">この例では、完全に同一の単語が含まれているメールボックスの所有者の連絡先フォルダー内の会議を検索するのには、 [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx)操作を使用する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-163">This example shows how to use the [ResolveNames](http://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation to find meetings in the mailbox owner's Contacts folder that contain the word "johnson".</span></span> 
  
<span data-ttu-id="b9b4a-164">EWS のマネージ API が[連絡先を解決するの](#bk_resolveewsma)には**ResolveName**メソッドを使用するときに送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-164">This is also the XML request that the EWS Managed API sends when you use the **ResolveName** method to [resolve a contact](#bk_resolveewsma).</span></span>
  
```xml
 <?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2007_SP1" />
  </soap:Header>
  <soap:Body>
    <m:ResolveNames ReturnFullContactData="true"
                    SearchScope="Contacts">
      <m:ParentFolderIds>
        <t:DistinguishedFolderId Id="contacts">
          <t:Mailbox>
            <t:EmailAddress>primary@contoso.com</t:EmailAddress>
          </t:Mailbox>
        </t:DistinguishedFolderId>
      </m:ParentFolderIds>
      <m:UnresolvedEntry>johnson</m:UnresolvedEntry>
    </m:ResolveNames>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="b9b4a-165">サーバー要求に応答し、 **ResolveNames**操作が正常に完了し、1 つだけ見つかった**NoError**を示すは、 [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx)要素の値が含まれています[ResolveNamesResponse](http://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx)メッセージ結果、または**ErrorNameResolutionMultipleResults**場合は、複数の結果が見つかりました - [EWS のマネージ API を使用して、代理人として連絡先を作成する](#bk_createewsma)連絡先の 3 番目のコード例に表示される内容であります。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-165">The server responds to the **ResolveNames** request with a [ResolveNamesResponse](http://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) message that includes a [ResponseCode](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the operation completed successfully and found only one result, or **ErrorNameResolutionMultipleResults** if multiple results were found - which is what's shown in third code example based on the contact [Create a contact as a delegate by using the EWS Managed API](#bk_createewsma).</span></span> <span data-ttu-id="b9b4a-166">応答には、各結果の[アイテム Id](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx)が含まれています。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-166">The response also contains the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of each result.</span></span> 
  
<span data-ttu-id="b9b4a-167">**ItemId** 要素の値は読みやすいよう短縮されています。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-167">The value of the **ItemId** element has been shortened for readability.</span></span> 
  
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
    <m:ResolveNamesResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
                            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:ResolveNamesResponseMessage ResponseClass="Warning">
          <m:MessageText>Multiple results were found.</m:MessageText>
          <m:ResponseCode>ErrorNameResolutionMultipleResults</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
          <m:ResolutionSet TotalItemsInView="2"
                           IncludesLastItemInRange="true">
            <t:Resolution>
              <t:Mailbox>
                <t:Name>brian_1@contoso.com</t:Name>
                <t:EmailAddress>brian_1@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Contact</t:MailboxType>
                <t:ItemId Id="iMihAAA="
                          ChangeKey="EQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiPQo" />
              </t:Mailbox>
            </t:Resolution>
            <t:Resolution>
              <t:Mailbox>
                <t:Name>brian_2@contoso.com</t:Name>
                <t:EmailAddress>brian_2@contoso.com</t:EmailAddress>
                <t:RoutingType>SMTP</t:RoutingType>
                <t:MailboxType>Contact</t:MailboxType>
                <t:ItemId Id="iMihAAA="
                          ChangeKey="EQAAABYAAADOilbYa8KaT7ZgMoTz2P+hAAABiPQo" />
              </t:Mailbox>
            </t:Resolution>
          </m:ResolutionSet>
        </m:ResolveNamesResponseMessage>
      </m:ResponseMessages>
    </m:ResolveNamesResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="b9b4a-168">あいまいな名前に一致する連絡先の**アイテム Id**がある場合は、これですることができます[を取得、更新、または代理人は EWS を使用して連絡先アイテムの削除](#bk_getews)**アイテム Id**と[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用して&mdash;を指定する必要はありませんしメールボックス所有者の SMTP アドレスです。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-168">Now that you have the **ItemId** for the contacts that match the ambiguous name, you can [Get, update, or delete contact items as a delegate by using EWS](#bk_getews) by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;and you do not need to specify the mailbox owner's SMTP address.</span></span> 

<span data-ttu-id="b9b4a-169"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="b9b4a-169"></span></span>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="b9b4a-170">EWS マネージ API を使用して、代理人として連絡先アイテムを取得、更新、または削除する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-170">Get, update, or delete contact items as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="b9b4a-171">取得、更新、または代理人アクセスを使用していないときにこれらのアクションを実行すると同じ方法で連絡先を削除するのには、EWS のマネージ API を使用できます。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-171">You can use the EWS Managed API to get, update, or delete a contact in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="b9b4a-172">唯一の違いは、サービス オブジェクトの代理人のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-172">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="b9b4a-173">**バインド**メソッドの呼び出しを一意に含まれる項目 ID では、メールボックスの所有者の連絡先フォルダーに、メールボックス ストア内の項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-173">The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Contacts folder.</span></span> 
  
<span data-ttu-id="b9b4a-174">**表 2 になります。EWS のマネージ API のメソッドを代理人として取引先担当者の操作**</span><span class="sxs-lookup"><span data-stu-id="b9b4a-174">**Table 2. EWS Managed API methods working with a contact as a delegate**</span></span>

|<span data-ttu-id="b9b4a-175">**タスク**</span><span class="sxs-lookup"><span data-stu-id="b9b4a-175">**Task**</span></span>|<span data-ttu-id="b9b4a-176">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="b9b4a-176">**EWS Managed API method**</span></span>|<span data-ttu-id="b9b4a-177">**コードの例**</span><span class="sxs-lookup"><span data-stu-id="b9b4a-177">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b9b4a-178">連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-178">Get a contact</span></span>  <br/> |[<span data-ttu-id="b9b4a-179">バインド</span><span class="sxs-lookup"><span data-stu-id="b9b4a-179">Bind</span></span>](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="b9b4a-180">EWS のマネージ API を使用してアイテムを取得します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-180">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="b9b4a-181">連絡先を更新する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-181">Update a contact</span></span>  <br/> |<span data-ttu-id="b9b4a-182">[バインド](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx)[の更新](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)の後に</span><span class="sxs-lookup"><span data-stu-id="b9b4a-182">[Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Update](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="b9b4a-183">EWS のマネージ API を使用してアイテムを更新します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-183">Update an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|<span data-ttu-id="b9b4a-184">連絡先を削除する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-184">Delete a contact</span></span>  <br/> |<span data-ttu-id="b9b4a-185">の[バインド](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx)[を削除](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)後に</span><span class="sxs-lookup"><span data-stu-id="b9b4a-185">[Bind](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Delete](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="b9b4a-186">EWS のマネージ API を使用して項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-186">Delete an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |

<span data-ttu-id="b9b4a-187"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="b9b4a-187"></span></span>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="b9b4a-188">EWS を使用して、代理人として連絡先アイテムを取得、更新、または削除する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-188">Get, update, or delete contact items as a delegate by using EWS</span></span>

<span data-ttu-id="b9b4a-189">取得、更新、または代理人アクセスを使用していないときに、これらのアクションを実行することと同じ方法で会議出席依頼や予定の取引先担当者を削除するのには、EWS を使用できます。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-189">You can use EWS to get, update, or delete a meeting or appointment contact in the same way that you perform these actions when you're not using delegate access.</span></span> <span data-ttu-id="b9b4a-190">唯一の違いは、サービス オブジェクトの代理人のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-190">The only difference is that the service object is for the delegate user.</span></span> <span data-ttu-id="b9b4a-191">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx)要求内で一意に含まれている項目の ID は、メールボックスの所有者の連絡先フォルダーに、メールボックス ストア内の項目を識別します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-191">The item ID included in the [GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) request uniquely identifies the item in the mailbox store, in the mailbox owner's Contacts folder.</span></span> 
  
<span data-ttu-id="b9b4a-192">**表 3。代理人として連絡先を操作するための EWS の操作**</span><span class="sxs-lookup"><span data-stu-id="b9b4a-192">**Table 3. EWS operations for working with a contact as a delegate**</span></span>

|<span data-ttu-id="b9b4a-193">**タスク**</span><span class="sxs-lookup"><span data-stu-id="b9b4a-193">**Task**</span></span>|<span data-ttu-id="b9b4a-194">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="b9b4a-194">**EWS operation**</span></span>|<span data-ttu-id="b9b4a-195">**サンプル**</span><span class="sxs-lookup"><span data-stu-id="b9b4a-195">**Sample**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="b9b4a-196">連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-196">Get a contact</span></span>  <br/> |[<span data-ttu-id="b9b4a-197">GetItem</span><span class="sxs-lookup"><span data-stu-id="b9b4a-197">GetItem</span></span>](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="b9b4a-198">EWS を使用してアイテムを取得します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-198">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="b9b4a-199">連絡先を更新する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-199">Update a contact</span></span>  <br/> |<span data-ttu-id="b9b4a-200">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)に続いて</span><span class="sxs-lookup"><span data-stu-id="b9b4a-200">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="b9b4a-201">EWS を使用してアイテムを更新します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-201">Update an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|<span data-ttu-id="b9b4a-202">連絡先を削除する</span><span class="sxs-lookup"><span data-stu-id="b9b4a-202">Delete a contact</span></span>  <br/> |<span data-ttu-id="b9b4a-203">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)の後に</span><span class="sxs-lookup"><span data-stu-id="b9b4a-203">[GetItem](http://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="b9b4a-204">EWS を使用して項目を削除します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-204">Delete an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="b9b4a-205">関連項目</span><span class="sxs-lookup"><span data-stu-id="b9b4a-205">See also</span></span>

- [<span data-ttu-id="b9b4a-206">Exchange での代理人アクセスと EWS</span><span class="sxs-lookup"><span data-stu-id="b9b4a-206">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
- [<span data-ttu-id="b9b4a-207">追加し、Exchange の EWS を使用して、デリゲートを削除します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-207">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [<span data-ttu-id="b9b4a-208">Exchange EWS を使用して別のユーザーのフォルダーのアクセス許可を設定します。</span><span class="sxs-lookup"><span data-stu-id="b9b4a-208">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
- [<span data-ttu-id="b9b4a-209">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="b9b4a-209">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
- [<span data-ttu-id="b9b4a-210">Exchange 2013 の EWS を使用してあいまいな名前を解決するには</span><span class="sxs-lookup"><span data-stu-id="b9b4a-210">Resolve ambiguous names by using EWS in Exchange 2013</span></span>](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)
    

