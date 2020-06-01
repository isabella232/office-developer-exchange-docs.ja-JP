---
title: Exchange で EWS を使用して、代理人として連絡先にアクセスする
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 3cd34c14-18b0-4fe2-a4c2-d884318c88fc
description: Exchange の EWS マネージ API または EWS を使用して、代理人として連絡先にアクセスする方法を説明します。
ms.openlocfilehash: 06faf7dd7459b14792abbea21761e909c8eb9fb6
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455346"
---
# <a name="access-contacts-as-a-delegate-by-using-ews-in-exchange"></a><span data-ttu-id="dc7d6-103">Exchange で EWS を使用して、代理人として連絡先にアクセスする</span><span class="sxs-lookup"><span data-stu-id="dc7d6-103">Access contacts as a delegate by using EWS in Exchange</span></span>

<span data-ttu-id="dc7d6-104">Exchange の EWS マネージ API または EWS を使用して、代理人として連絡先にアクセスする方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-104">Learn how to access contacts as a delegate by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="dc7d6-p101">EWS マネージ API または EWS を使用して、ユーザーにメールボックス所有者の連絡先フォルダーへのアクセス権を付与できます。代理人は、メールボックス所有者の代わりに連絡先を作成し、アクセス許可に応じて、メールボックス所有者の連絡先フォルダーから連絡先を取得、更新、および削除することができます。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-p101">You can use the EWS Managed API or EWS to give a user access to a mailbox owner's Contacts folder. The delegate can then create contacts on behalf of the mailbox owner, and retrieve, update, and delete contacts from the mailbox owner's Contacts folder, depending on their permissions.</span></span>
  
<span data-ttu-id="dc7d6-p102">代理人として、同じメソッドと操作を使用して、自分の連絡先フォルダーへのアクセスに使用する、メールボックス所有者の連絡先フォルダーにアクセスします。大きな違いは、[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicit)を使用して連絡先アイテムを検索または作成する必要がある点です。アイテム ID を識別すると、[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)を使用してアイテムを取得、更新、または削除できます。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-p102">As a delegate, you use the same methods and operations to access a mailbox owner's Contacts folder that you use to access your own Contacts folder. The main difference is that you have to use [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicit) to find or create a contact item, and then after you identify the item ID, you can use [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit) to get, update, or delete the item.</span></span> 
  
<span data-ttu-id="dc7d6-109">**表 1. 代理人として連絡先にアクセスするための EWS マネージ API メソッドと EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="dc7d6-109">**Table 1. EWS Managed API methods and EWS operations for accessing a contact as a delegate**</span></span>

|<span data-ttu-id="dc7d6-110">**目的**</span><span class="sxs-lookup"><span data-stu-id="dc7d6-110">**If you want to…**</span></span>|<span data-ttu-id="dc7d6-111">**使用する EWS マネージ API メソッド…**</span><span class="sxs-lookup"><span data-stu-id="dc7d6-111">**Use this EWS Managed API method…**</span></span>|<span data-ttu-id="dc7d6-112">**使用する EWS 操作…**</span><span class="sxs-lookup"><span data-stu-id="dc7d6-112">**Use this EWS operation…**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="dc7d6-113">代理人として連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-113">Create a contact as a delegate</span></span>  <br/> |<span data-ttu-id="dc7d6-114">[Item.Save](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx): [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) パラメーターがメールボックス所有者の連絡先フォルダーへの[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) を提供する場合</span><span class="sxs-lookup"><span data-stu-id="dc7d6-114">[Item.Save](https://msdn.microsoft.com/library/dd635209%28v=exchg.80%29.aspx) where the [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="dc7d6-115">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx): [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する場合</span><span class="sxs-lookup"><span data-stu-id="dc7d6-115">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="dc7d6-116">代理人として複数の連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-116">Create multiple contacts as a delegate</span></span>  <br/> |<span data-ttu-id="dc7d6-117">[ExchangeService.CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx): **FolderId** パラメーターがメールボックス所有者の連絡先フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する場合</span><span class="sxs-lookup"><span data-stu-id="dc7d6-117">[ExchangeService.CreateItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.createitems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="dc7d6-118">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx): [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する場合</span><span class="sxs-lookup"><span data-stu-id="dc7d6-118">[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="dc7d6-119">代理人として連絡先を解決する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-119">Resolve a contact as a delegate</span></span>  <br/> |<span data-ttu-id="dc7d6-120">[ExchangeService.ResolveName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx): [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) パラメーターがメールボックス所有者の連絡先フォルダーへの[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する場合</span><span class="sxs-lookup"><span data-stu-id="dc7d6-120">[ExchangeService.ResolveName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) where the [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="dc7d6-121">[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx): [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する場合</span><span class="sxs-lookup"><span data-stu-id="dc7d6-121">[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="dc7d6-122">代理人として連絡先を検索する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-122">Search for or find a contact as a delegate</span></span>  <br/> |<span data-ttu-id="dc7d6-123">[ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx): **FolderId** パラメーターがメールボックス所有者の連絡先フォルダーに[明示的なアクセス](delegate-access-and-ews-in-exchange.md#bk_explicitewsma)を提供する場合</span><span class="sxs-lookup"><span data-stu-id="dc7d6-123">[ExchangeService.FindItems](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.finditems%28v=exchg.80%29.aspx) where the **FolderId** parameter provides [explicit access](delegate-access-and-ews-in-exchange.md#bk_explicitewsma) to the mailbox owner's Contacts folder</span></span>  <br/> |<span data-ttu-id="dc7d6-124">[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx): [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) 要素がメールボックス所有者の [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) を指定する場合</span><span class="sxs-lookup"><span data-stu-id="dc7d6-124">[FindItem](https://msdn.microsoft.com/library/ebad6aae-16e7-44de-ae63-a95b24539729%28Office.15%29.aspx) where the [Mailbox](https://msdn.microsoft.com/library/befc70fd-51cb-4258-884c-80c9050f0e82%28Office.15%29.aspx) element specifies the [EmailAddress](https://msdn.microsoft.com/library/922c8b21-04a9-4229-b48c-187c3095422e%28Office.15%29.aspx) of the mailbox owner</span></span>  <br/> |
|<span data-ttu-id="dc7d6-125">代理人として連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-125">Get a contact as a delegate</span></span>  <br/> |[<span data-ttu-id="dc7d6-126">Contact.Bind</span><span class="sxs-lookup"><span data-stu-id="dc7d6-126">Contact.Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="dc7d6-127">GetItem</span><span class="sxs-lookup"><span data-stu-id="dc7d6-127">GetItem</span></span>](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |
|<span data-ttu-id="dc7d6-128">代理人として連絡先を更新する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-128">Update a contact as a delegate</span></span>  <br/> |<span data-ttu-id="dc7d6-129">[Contact.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) の後に [Contact.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx) を使用する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-129">[Contact.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) followed by [Contact.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.update%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="dc7d6-130">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="dc7d6-130">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |
|<span data-ttu-id="dc7d6-131">代理人として連絡先を削除する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-131">Delete a contact as a delegate</span></span>  <br/> |<span data-ttu-id="dc7d6-132">[Contact.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) の後に [Contact.Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx) 使用する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-132">[Contact.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.contact.bind%28v=exchg.80%29.aspx) followed by [Contact.Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item.delete%28v=exchg.80%29.aspx)</span></span> <br/> |<span data-ttu-id="dc7d6-133">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [DeleteItem](../web-service-reference/deleteitem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="dc7d6-133">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |
   
> [!NOTE]
> <span data-ttu-id="dc7d6-134">この記事のコード例では、primary@contoso.com がメールボックス所有者です。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-134">In the code examples in this article, primary@contoso.com is the mailbox owner.</span></span> 

<span data-ttu-id="dc7d6-135"><a name="bk_prereq"> </a></span><span class="sxs-lookup"><span data-stu-id="dc7d6-135"><a name="bk_prereq"> </a></span></span>

## <a name="prerequisite-tasks"></a><span data-ttu-id="dc7d6-136">事前に必要なタスク</span><span class="sxs-lookup"><span data-stu-id="dc7d6-136">Prerequisite tasks</span></span>

<span data-ttu-id="dc7d6-137">ユーザーは、代理人としてメールボックス所有者の連絡先フォルダーにアクセスできるようにするために、[アクセス許可を持つ代理人として](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)メールボックス所有者の連絡先フォルダーに追加される必要があります。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-137">Before a user can access the mailbox owner's Contacts folder as a delegate, the user must be [added as a delegate with permissions](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md) to the mailbox owner's Contacts folder.</span></span> 

<span data-ttu-id="dc7d6-138"><a name="bk_createewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="dc7d6-138"><a name="bk_createewsma"> </a></span></span>

## <a name="create-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="dc7d6-139">EWS マネージ API を使用して、代理人として連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-139">Create a contact as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="dc7d6-140">EWS マネージ API を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックス所有者の連絡先を作成することができます。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-140">The EWS Managed API enables you to use the service object for the delegate user to create contacts for the mailbox owner.</span></span> <span data-ttu-id="dc7d6-141">この例は、[Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) メソッドを使用して会議を作成し、出席者に会議出席依頼を送信する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-141">This example shows how to use the [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method to create a meeting and send meeting requests to the attendees.</span></span> 
  
<span data-ttu-id="dc7d6-142">この例では、**service** が代理人の有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、代理人にメールボックス所有者の連絡先フォルダーの適切なアクセス許可が付与されていることを前提にしています。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-142">This example assumes that **service** is a valid [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object for the delegate and that the delegate has been granted the appropriate permissions for the mailbox owner's Contacts folder.</span></span> 
  
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

<span data-ttu-id="dc7d6-143">アイテムの保存時には、[Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) メソッド呼び出しでメールボックス所有者の連絡先フォルダーを識別する必要があることにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-143">Note that when you save the item, the [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.save%28v=exchg.80%29.aspx) method call must identify the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="dc7d6-144">メールボックス所有者の連絡先フォルダーを指定しない場合、会議出席依頼はメールボックス所有者の連絡先フォルダーではなく、代理人の連絡先フォルダーに保存されます。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-144">If the mailbox owner's Contacts folder is not specified, the meeting request gets saved to the delegate's Contacts folder and not the mailbox owner's Contacts folder.</span></span> <span data-ttu-id="dc7d6-145">メールボックス所有者の連絡先フォルダーは、2 つの方法で **Save** メソッド呼び出しに含めることができます。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-145">You can include the mailbox owner's Contacts folder in the **Save** method call in two way.</span></span> <span data-ttu-id="dc7d6-146">メールボックス所有者の [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) と SMTP アドレスを使用して、[FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) オブジェクトの新しいインスタンスをインスタンス化することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-146">We recommend that you instantiate a new instance of the [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) object by using the [WellKnownFolderName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.wellknownfoldername%28v=exchg.80%29.aspx) and the SMTP address of the mailbox owner.</span></span> 
  
```cs
contact.Save(new FolderId(WellKnownFolderName.Contacts, "primary@contoso.com"));
```

<span data-ttu-id="dc7d6-147">ただし、最初に連絡先フォルダーへの [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) を使用してから、 **Save** メソッド呼び出しでフォルダーの ID を使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-147">However, you can also [Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folder.bind%28v=exchg.80%29.aspx) to the Contacts folder first, and then use the ID of the folder in the **Save** method call.</span></span> <span data-ttu-id="dc7d6-148">ただし、これにより追加の EWS 呼び出しが作成されることにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-148">Be aware, however, that this creates an extra EWS call.</span></span> 
  
```cs
    // Identify the mailbox owner's SMTP address 
    // and bind to their Contacts folder.
    Mailbox primary = new Mailbox("primary@contoso.com"); 
    Folder primaryContacts = Folder.Bind(service, new FolderId(WellKnownFolderName.Contacts, primary)); 
…
    // Save the contact to the mailbox owner's Contacts folder.
    meeting.Save(primaryContacts.Id);
```

<span data-ttu-id="dc7d6-149"><a name="bk_createews"> </a></span><span class="sxs-lookup"><span data-stu-id="dc7d6-149"><a name="bk_createews"> </a></span></span>

## <a name="create-a-contact-as-a-delegate-by-using-ews"></a><span data-ttu-id="dc7d6-150">EWS を使用して、代理人として連絡先を作成する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-150">Create a contact as a delegate by using EWS</span></span>

<span data-ttu-id="dc7d6-p106">EWS を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックス所有者の連絡先アイテムを作成することができます。この例では、[CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) を使用して連絡先を作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-p106">EWS enables you to use the service object for the delegate user to create contact items for the mailbox owner. This example shows how to use the [CreateItem](https://msdn.microsoft.com/library/aa4a7c94-f668-4bd2-8079-c855f6ab17e1%28Office.15%29.aspx) operation to create a contact.</span></span> 
  
<span data-ttu-id="dc7d6-153">これは、[連絡先の作成](#bk_createewsma)に **Save** メソッドを使用する場合、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-153">This is also the XML request that the EWS Managed API sends when you use the **Save** method to [create a contact](#bk_createewsma).</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="dc7d6-p107">サーバーは、[CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) メッセージを含む **CreateItem** 要求に応答します。このメッセージには、連絡先が正常に作成されたことを示す、**NoError** の [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素の値が含まれます。また、応答には新しく作成された連絡先のアイテム ID も含まれます。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-p107">The server responds to the **CreateItem** request with a [CreateItemResponse](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the contact was created successfully. The response also contains the item ID of the newly created contact.</span></span>

<span data-ttu-id="dc7d6-156"><a name="bk_resolveewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="dc7d6-156"><a name="bk_resolveewsma"> </a></span></span>

## <a name="resolve-a-contact-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="dc7d6-157">EWS マネージ API を使用して、代理人として連絡先を解決する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-157">Resolve a contact as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="dc7d6-158">場合によって、あいまいな名前または語句に基づいて連絡先を検索するには、メールボックス所有者の連絡先フォルダーを指定するようにするため、[FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) を含む [ExchangeService.ResolveName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) メソッドのいずれかを使用する必要があります。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-158">To find a contact based on a possibly ambiguous name or term, you must use one of the [ExchangeService.ResolveName](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.resolvename%28v=exchg.80%29.aspx) methods that includes a [FolderId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.folderid%28v=exchg.80%29.aspx) parameter, so that you can specify the mailbox owner's Contacts folder.</span></span> 
  
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

<span data-ttu-id="dc7d6-159">**ResolveNames** メソッドの呼び出しが ID と共に応答を返すと、ID と[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;を使用して[連絡先を取得、更新または削除](#bk_getewsma)できます。メールボックス所有者の SMTP アドレスを指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-159">After the **ResolveNames** method call returns a response with an ID, you can [get, update or delete the contact](#bk_getewsma) using the ID and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;and you do not need to specify the mailbox owner's SMTP address.</span></span> 

<span data-ttu-id="dc7d6-160"><a name="bk_resolveews"> </a></span><span class="sxs-lookup"><span data-stu-id="dc7d6-160"><a name="bk_resolveews"> </a></span></span>

## <a name="resolve-a-contact-as-a-delegate-by-using-ews"></a><span data-ttu-id="dc7d6-161">EWS を使用して、代理人として連絡先を解決する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-161">Resolve a contact as a delegate by using EWS</span></span>

<span data-ttu-id="dc7d6-p108">EWS を使用すると、代理ユーザーのサービス オブジェクトを使用して、メールボックス所有者の連絡先内の部分的な名前を解決できます。この例では、[ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) 操作を使用して、"johnson" という単語が含まれるメールボックス所有者の連絡先フォルダー内で会議を検索する方法を示します。 </span><span class="sxs-lookup"><span data-stu-id="dc7d6-p108">EWS enables you to use the service object for the delegate user to resolve partial names in the mailbox owner's Contacts folder. This example shows how to use the [ResolveNames](https://msdn.microsoft.com/library/6b4eb4b3-9ad6-4804-a09f-7e20cfea4dbb%28Office.15%29.aspx) operation to find meetings in the mailbox owner's Contacts folder that contain the word "johnson".</span></span> 
  
<span data-ttu-id="dc7d6-164">これは、[連絡先の解決](#bk_resolveewsma)に **ResolvName** メソッドを使用する場合、EWS マネージ API が送信する XML 要求でもあります。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-164">This is also the XML request that the EWS Managed API sends when you use the **ResolveName** method to [resolve a contact](#bk_resolveewsma).</span></span>
  
```xml
 <?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
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

<span data-ttu-id="dc7d6-165">サーバーは、**ResolveNames** 要求に対して[ResolveNamesResponse](https://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) メッセージで応答します。このメッセージには、操作が正常に完了され、結果が 1 つだけ検出されたことを示す **NoError** と、複数の結果が検出された場合は **ErrorNameResolutionMultipleResults** という [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) 要素値が含まれます。これは、連絡先 (「[EWS マネージ API を使用して、代理人として連絡先を作成する](#bk_createewsma)」) に基づく 3 番目のコード例で示されています。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-165">The server responds to the **ResolveNames** request with a [ResolveNamesResponse](https://msdn.microsoft.com/library/5e7be1e2-44ea-403f-9135-2388d030078c%28Office.15%29.aspx) message that includes a [ResponseCode](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) element value of **NoError**, which indicates that the operation completed successfully and found only one result, or **ErrorNameResolutionMultipleResults** if multiple results were found - which is what's shown in third code example based on the contact [Create a contact as a delegate by using the EWS Managed API](#bk_createewsma).</span></span> <span data-ttu-id="dc7d6-166">応答には各結果の [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) も含まれます。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-166">The response also contains the [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of each result.</span></span> 
  
<span data-ttu-id="dc7d6-167">**ItemId** 要素の値は読みやすいよう短縮されています。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-167">The value of the **ItemId** element has been shortened for readability.</span></span> 
  
```XML
 <?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15"
                         MinorVersion="0"
                         MajorBuildNumber="893"
                         MinorBuildNumber="17"
                         Version="V2_10"
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body>
    <m:ResolveNamesResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
                            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="dc7d6-168">あいまいな名前と一致する連絡先の **ItemId** がわかると、**ItemId** と[暗黙的なアクセス](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;を使用して、[EWS を使用して、代理人として連絡先アイテムを取得、更新、または削除する](#bk_getews)ことができます。メールボックス所有者の SMTP アドレスを指定する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-168">Now that you have the **ItemId** for the contacts that match the ambiguous name, you can [Get, update, or delete contact items as a delegate by using EWS](#bk_getews) by using the **ItemId** and [implicit access](delegate-access-and-ews-in-exchange.md#bk_implicit)&mdash;and you do not need to specify the mailbox owner's SMTP address.</span></span> 

<span data-ttu-id="dc7d6-169"><a name="bk_getewsma"> </a></span><span class="sxs-lookup"><span data-stu-id="dc7d6-169"><a name="bk_getewsma"> </a></span></span>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-the-ews-managed-api"></a><span data-ttu-id="dc7d6-170">EWS マネージ API を使用して、代理人として連絡先アイテムを取得、更新、または削除する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-170">Get, update, or delete contact items as a delegate by using the EWS Managed API</span></span>

<span data-ttu-id="dc7d6-p110">EWS マネージ API を使用すると、代理人アクセスを使用していない場合に取得、更新、または削除のアクションを実行するのと同じ方法で、連絡先アイテムを取得、更新、または削除することができます。唯一の違いは、サービス オブジェクトが代理ユーザーを対象にしている点です。**Bind** メソッド呼び出しに含まれるアイテム ID は、メールボックス所有者の連絡先フォルダー内のメールボックス ストアにあるアイテムを一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-p110">You can use the EWS Managed API to get, update, or delete a contact in the same way that you perform these actions when you're not using delegate access. The only difference is that the service object is for the delegate user. The item ID included in the **Bind** method call uniquely identifies the item in the mailbox store, in the mailbox owner's Contacts folder.</span></span> 
  
<span data-ttu-id="dc7d6-174">**表 2. 代理人として連絡先を操作する EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="dc7d6-174">**Table 2. EWS Managed API methods working with a contact as a delegate**</span></span>

|<span data-ttu-id="dc7d6-175">**Task**</span><span class="sxs-lookup"><span data-stu-id="dc7d6-175">**Task**</span></span>|<span data-ttu-id="dc7d6-176">**EWS マネージ API メソッド**</span><span class="sxs-lookup"><span data-stu-id="dc7d6-176">**EWS Managed API method**</span></span>|<span data-ttu-id="dc7d6-177">**コード例**</span><span class="sxs-lookup"><span data-stu-id="dc7d6-177">**Code example**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="dc7d6-178">連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-178">Get a contact</span></span>  <br/> |[<span data-ttu-id="dc7d6-179">Bind</span><span class="sxs-lookup"><span data-stu-id="dc7d6-179">Bind</span></span>](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) <br/> |[<span data-ttu-id="dc7d6-180">EWS マネージ API を使用してアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-180">Get an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getewsma) <br/> |
|<span data-ttu-id="dc7d6-181">連絡先を更新する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-181">Update a contact</span></span>  <br/> |<span data-ttu-id="dc7d6-182">[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) の後に [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="dc7d6-182">[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Update](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.update%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="dc7d6-183">EWS マネージ API を使用してアイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-183">Update an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateewsma) <br/> |
|<span data-ttu-id="dc7d6-184">連絡先を削除する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-184">Delete a contact</span></span>  <br/> |<span data-ttu-id="dc7d6-185">[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) の後に [Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span><span class="sxs-lookup"><span data-stu-id="dc7d6-185">[Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.bind%28v=exchg.80%29.aspx) followed by [Delete](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.appointment.delete%28v=exchg.80%29.aspx)</span></span> <br/> |[<span data-ttu-id="dc7d6-186">EWS マネージ API を使用してアイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-186">Delete an item by using the EWS Managed API</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteewsma) <br/> |

<span data-ttu-id="dc7d6-187"><a name="bk_getews"> </a></span><span class="sxs-lookup"><span data-stu-id="dc7d6-187"><a name="bk_getews"> </a></span></span>

## <a name="get-update-or-delete-contact-items-as-a-delegate-by-using-ews"></a><span data-ttu-id="dc7d6-188">EWS を使用して、代理人として連絡先アイテムを取得、更新、または削除する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-188">Get, update, or delete contact items as a delegate by using EWS</span></span>

<span data-ttu-id="dc7d6-p111">EWS を使用すると、代理人アクセスを使用していない場合に取得、更新、または削除のアクションを実行するのと同じ方法で、連絡先アイテムを取得、更新、または削除することができます。唯一の違いは、サービス オブジェクトが代理ユーザーを対象にしている点です。[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) 要求に含まれるアイテム ID は、メールボックス所有者の連絡先フォルダー内のメールボックス ストアにあるアイテムを一意に識別します。</span><span class="sxs-lookup"><span data-stu-id="dc7d6-p111">You can use EWS to get, update, or delete a meeting or appointment contact in the same way that you perform these actions when you're not using delegate access. The only difference is that the service object is for the delegate user. The item ID included in the [GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) request uniquely identifies the item in the mailbox store, in the mailbox owner's Contacts folder.</span></span> 
  
<span data-ttu-id="dc7d6-192">**表 3. 代理人として連絡先を操作するための EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="dc7d6-192">**Table 3. EWS operations for working with a contact as a delegate**</span></span>

|<span data-ttu-id="dc7d6-193">**タスク**</span><span class="sxs-lookup"><span data-stu-id="dc7d6-193">**Task**</span></span>|<span data-ttu-id="dc7d6-194">**EWS 操作**</span><span class="sxs-lookup"><span data-stu-id="dc7d6-194">**EWS operation**</span></span>|<span data-ttu-id="dc7d6-195">**サンプル**</span><span class="sxs-lookup"><span data-stu-id="dc7d6-195">**Sample**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="dc7d6-196">連絡先を取得する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-196">Get a contact</span></span>  <br/> |[<span data-ttu-id="dc7d6-197">GetItem</span><span class="sxs-lookup"><span data-stu-id="dc7d6-197">GetItem</span></span>](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) <br/> |[<span data-ttu-id="dc7d6-198">EWS を使用してアイテムを取得する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-198">Get an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_getews) <br/> |
|<span data-ttu-id="dc7d6-199">連絡先を更新する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-199">Update a contact</span></span>  <br/> |<span data-ttu-id="dc7d6-200">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) を使用する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-200">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx)</span></span> <br/> |[<span data-ttu-id="dc7d6-201">EWS を使用してアイテムを更新する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-201">Update an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_updateews) <br/> |
|<span data-ttu-id="dc7d6-202">連絡先を削除する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-202">Delete a contact</span></span>  <br/> |<span data-ttu-id="dc7d6-203">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) の後に [DeleteItem](../web-service-reference/deleteitem-operation.md) を使用する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-203">[GetItem](https://msdn.microsoft.com/library/a41c29c9-c4e6-4aa4-8e28-ccb0b478fee8%28Office.15%29.aspx) followed by [DeleteItem](../web-service-reference/deleteitem-operation.md)</span></span> <br/> |[<span data-ttu-id="dc7d6-204">EWS を使用してアイテムを削除する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-204">Delete an item by using EWS</span></span>](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md#bk_deleteews) <br/> |
   
## <a name="see-also"></a><span data-ttu-id="dc7d6-205">関連項目</span><span class="sxs-lookup"><span data-stu-id="dc7d6-205">See also</span></span>

- [<span data-ttu-id="dc7d6-206">Exchange での代理人アクセスと EWS</span><span class="sxs-lookup"><span data-stu-id="dc7d6-206">Delegate access and EWS in Exchange</span></span>](delegate-access-and-ews-in-exchange.md)
- [<span data-ttu-id="dc7d6-207">Exchange で EWS を使用して代理人を追加および削除する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-207">Add and remove delegates by using EWS in Exchange</span></span>](how-to-add-and-remove-delegates-by-using-ews-in-exchange.md)
- [<span data-ttu-id="dc7d6-208">Exchange で EWS を使用して別のユーザーのフォルダーのアクセス許可を設定する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-208">Set folder permissions for another user by using EWS in Exchange</span></span>](how-to-set-folder-permissions-for-another-user-by-using-ews-in-exchange.md)
- [<span data-ttu-id="dc7d6-209">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="dc7d6-209">People and contacts in EWS in Exchange</span></span>](people-and-contacts-in-ews-in-exchange.md)
- [<span data-ttu-id="dc7d6-210">Exchange 2013 の EWS を使用して、あいまいな名前を解決する</span><span class="sxs-lookup"><span data-stu-id="dc7d6-210">Resolve ambiguous names by using EWS in Exchange 2013</span></span>](how-to-resolve-ambiguous-names-by-using-ews-in-exchange-2013.md)
    

