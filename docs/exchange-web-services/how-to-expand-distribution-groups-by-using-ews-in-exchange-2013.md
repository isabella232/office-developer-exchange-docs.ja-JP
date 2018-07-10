---
title: Exchange 2013 の EWS を使用して配布グループを展開します。
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 25ee84e7-63bc-4f51-9b7d-e7f46fd574d5
description: Exchange で EWS マネージ API または EWS を使用して配布グループを展開する方法について説明します。
ms.openlocfilehash: 0f9186fb71b3005c71a70e89aafb674ae15e4814
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19758942"
---
# <a name="expand-distribution-groups-by-using-ews-in-exchange-2013"></a><span data-ttu-id="6d0d2-103">Exchange 2013 の EWS を使用して配布グループを展開します。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-103">Expand distribution groups by using EWS in Exchange 2013</span></span>

<span data-ttu-id="6d0d2-104">Exchange で EWS マネージ API または EWS を使用して配布グループを展開する方法について説明します。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-104">Learn how to expand a distribution group by using the EWS Managed API or EWS in Exchange.</span></span>
  
<span data-ttu-id="6d0d2-105">[ExchangeService.ExpandGroup](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドまたは[ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx)の EWS の操作を使用するには、すべての受信者を識別するのに配布グループを展開します。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-105">You can use the [ExchangeService.ExpandGroup](http://msdn.microsoft.com/ja-jp/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) EWS Managed API method or the [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) EWS operation to expand a distribution group to identify all recipients.</span></span> 
  
<span data-ttu-id="6d0d2-106">[ExpandGroup](http://msdn.microsoft.com/ja-jp/library/office/ee344007%28v=exchg.80%29.aspx)メソッドをオーバー ロードするためは、いくつかの方法で呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-106">Because the [ExpandGroup](http://msdn.microsoft.com/ja-jp/library/office/ee344007%28v=exchg.80%29.aspx) method is overloaded, you can call it in several ways:</span></span> 
  
- <span data-ttu-id="6d0d2-107">[ExpandGroup(String)](http://msdn.microsoft.com/ja-jp/library/office/ee343988%28v=exchg.80%29.aspx)では、SMTP アドレスによって識別されるグループを展開します。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-107">[ExpandGroup(String)](http://msdn.microsoft.com/ja-jp/library/office/ee343988%28v=exchg.80%29.aspx) - Expands a group identified by an SMTP address.</span></span> 
    
- <span data-ttu-id="6d0d2-108">[ExpandGroup(EmailAddress)](http://msdn.microsoft.com/ja-jp/library/office/ee344007%28v=exchg.80%29.aspx) - は、電子メール アドレスで識別されるグループを展開します。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-108">[ExpandGroup(EmailAddress)](http://msdn.microsoft.com/ja-jp/library/office/ee344007%28v=exchg.80%29.aspx) - Expands a group identified by an email address.</span></span> 
    
- <span data-ttu-id="6d0d2-109">[ExpandGroup(ItemId)](http://msdn.microsoft.com/ja-jp/library/office/ee356407%28v=exchg.80%29.aspx) ・ グループ ID で識別されるグループを展開します。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-109">[ExpandGroup(ItemId)](http://msdn.microsoft.com/ja-jp/library/office/ee356407%28v=exchg.80%29.aspx) - Expands a group identified by a group ID.</span></span> 
    
- <span data-ttu-id="6d0d2-110">[ExpanGroup (文字列、文字列)](http://msdn.microsoft.com/ja-jp/library/office/ee356468%28v=exchg.80%29.aspx)では、SMTP アドレスとそのアドレスのルーティングの種類によって識別されるグループを展開します。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-110">[ExpanGroup(String, String)](http://msdn.microsoft.com/ja-jp/library/office/ee356468%28v=exchg.80%29.aspx) - Expands a group identified by an SMTP address and the routing type of that address.</span></span> 
    
## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews-managed-api"></a><span data-ttu-id="6d0d2-111">EWS マネージ API を使用してユニバーサル配布グループまたはセキュリティ グループを展開する</span><span class="sxs-lookup"><span data-stu-id="6d0d2-111">Expand a universal distribution group or security group by using EWS Managed API</span></span>
<span data-ttu-id="6d0d2-112"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="6d0d2-112"></span></span>

<span data-ttu-id="6d0d2-113">次の例では、最も簡単な方法には、電子メール アドレスを使用して、ユニバーサル配布グループまたはセキュリティ グループを展開する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-113">The following example shows how to expand a universal distribution group or security group by using an email address, which is the simplest approach.</span></span> <span data-ttu-id="6d0d2-114">この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-114">This example assumes that **service** is a valid [ExchangeService](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) object and that the user has been authenticated to an Exchange server.</span></span> 
  
```cs
// Return the expanded group.
   ExpandGroupResults myGroupMembers = service.ExpandGroup("employees@contoso.com");
// Display the group members.
   foreach (EmailAddress address in myGroupMembers.Members)
   {
      Console.WriteLine("Email Address: {0}", address);
   }

```

<span data-ttu-id="6d0d2-p102">これは長いコードではなく、非常に基本的であり、お探しのものとは異なる可能性があります。ではもう一歩踏み込んでみましょう。配布グループには、他の配布グループを含めることもできます。単に展開した場合、含まれている配布グループのメール アドレスは出力されますが、グループが展開されるわけではありません。数行のコードを追加すると、グループを再帰的に展開して、すべての連絡先を出力できます。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-p102">That's not a lot of code, but it's also pretty basic and might not give you what you are looking for. So let's take it a step further. Distribution groups can also contain other distribution groups. Simply expanding it will output the email address of the contained distribution groups but not expand them. By adding a few more lines of code, you can recursively expand the groups to output every contact.</span></span>
  
```cs
private static void ExpandDistributionLists(ExchangeService service, string Mailbox)
{
   // Return the expanded group.
      ExpandGroupResults myGroupMembers = service.ExpandGroup(Mailbox);
   // Display the group members.
      foreach (EmailAddress address in myGroupMembers.Members)
      {
         // Check to see if the mailbox is a public group
         if (address.MailboxType == MailboxType.PublicGroup)
      {
         // Call the function again to expand the contained
         // distribution group.
         ExpandDistributionLists(service, address.Address);
      }
      else
      {
         // Output the address of the mailbox.
         Console.WriteLine("Email Address: {0}", address);
      }
   }
}

```

<span data-ttu-id="6d0d2-120">これで、この新しい関数をコード内で呼び出して、最初のグループに含まれているすべてのパブリックな配布グループを展開できます。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-120">And now you can call this new function in the your code and expand all the public distribution groups contained within the first one.</span></span>
  
```cs
ExpandDistributionLists(service, "employees@contoso.com");

```

## <a name="expand-a-contact-group-by-using-ews-managed-api"></a><span data-ttu-id="6d0d2-121">EWS マネージ API を使用して連絡先グループを展開する</span><span class="sxs-lookup"><span data-stu-id="6d0d2-121">Expand a contact group by using EWS Managed API</span></span>
<span data-ttu-id="6d0d2-122"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="6d0d2-122"></span></span>

<span data-ttu-id="6d0d2-123">連絡先グループに関連付けられた電子メール アドレスがないために、 [ExpandGroup(ItemId)](http://msdn.microsoft.com/ja-jp/library/office/ee356407%28v=exchg.80%29.aspx)メソッドを使用して、アイテムの Id に基づくグループを展開する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-123">Because contact groups do not have an associated email address, you need to expand the group based on the ItemId by using the [ExpandGroup(ItemId)](http://msdn.microsoft.com/ja-jp/library/office/ee356407%28v=exchg.80%29.aspx) method.</span></span> <span data-ttu-id="6d0d2-124">前の例のように、関数を作成し、[アイテム Id](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx)を文字列から 2 番目のパラメーターの型を変更できます。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-124">You can create a function, as shown in the previous example, and change the second parameter type from a string to an [ItemId](http://msdn.microsoft.com/ja-jp/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx).</span></span>
  
```cs
private static void ExpandContactGroup(ExchangeService service, ItemId groupID)
{
   // Return the expanded group.
      ExpandGroupResults myGroupMembers = service.ExpandGroup(groupID);
   // Display the group members.
      foreach (EmailAddress address in myGroupMembers.Members)
      {
         if (address.MailboxType == MailboxType.PublicGroup)
         {
            ExpandDistributionLists(service, address.Address);
         }
         else
         {
            Console.WriteLine("Email Address: {0}", address);
         }
      }
}
```

<span data-ttu-id="6d0d2-125">これで、Exchange サービスのオブジェクトと連絡先のグループの**アイテム Id**を使用してこの関数を呼び出すことができます。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-125">Now you can call this function by using the Exchange service object and the **ItemId** of the contact group.</span></span> <span data-ttu-id="6d0d2-126">例では**アイテム Id**が読みやすさに省略されていることを注意してください。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-126">Note that the **ItemId** in the example is shortened for readability.</span></span> 
  
```cs
ExpandContactGroup(service, new ItemId("AAMkADBlY…");

```

## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews"></a><span data-ttu-id="6d0d2-127">EWS を使用して、ユニバーサル配布グループまたはセキュリティ グループを展開する</span><span class="sxs-lookup"><span data-stu-id="6d0d2-127">Expand a universal distribution group or security group by using EWS</span></span>
<span data-ttu-id="6d0d2-128"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="6d0d2-128"></span></span>

<span data-ttu-id="6d0d2-129">[ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx)操作を使用する場合、サーバーへのクライアントから送信された XML 要求メッセージの例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-129">The following example shows the XML request message that is sent from the client to the server when you use the [ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) operation.</span></span> <span data-ttu-id="6d0d2-130">EWS のマネージ API は、[ユニバーサル配布グループを展開](#bk_ExpandDGEWSMA)する EWS のマネージ API を使用する場合を送信する XML 要求にもです。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-130">This is also the XML request that the EWS Managed API sends when you use the EWS Managed API to [expand a universal distribution group](#bk_ExpandDGEWSMA).</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
        <t:EmailAddress>employees@contoso.com</t:EmailAddress>
      </Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="6d0d2-p106">次の例では、サーバーからクライアントに送信される XML 応答メッセージを示します。メールボックスとユニバーサル配布グループの両方が返されることにご注意ください。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-p106">The following example shows the XML response message that is sent from the server to the client. Notice that both mailboxes and universal distribution groups are returned.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
     xmlns:xsd="http://www.w3.org/2001/XMLSchema">
<ExpandDLResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                      xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
    <ExpandDLResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <DLExpansion IncludesLastItemInRange="true" TotalItemsInView="4">
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Sadie Daniels</Name>
          <EmailAddress>sadie@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Alfred Welker</Name>
          <EmailAddress>alfred@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Contoso Sales</Name>
          <EmailAddress>sales@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>PublicDL</MailboxType>
        </Mailbox>
        <Mailbox xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Contoso Support</Name>
          <EmailAddress>support@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>PublicDL</MailboxType>
        </Mailbox>
      </DLExpansion>
    </ExpandDLResponseMessage>
  </ResponseMessages>
</ExpandDLResponse>
</s:Body>
</s:Envelope>
```

<span data-ttu-id="6d0d2-p107">EWS マネージ API を使用する場合とは異なり、EWS を使用してユニバーサル配布グループを展開する場合は、返される配布グループを再帰的に展開できません。応答に含まれている各配布グループを展開するには、追加の要求を送信する必要があります。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-p107">Unlike when you use the EWS Managed API, when you use EWS to expand a universal distribution group, you can't recursively expand the distribution groups that are returned. You will need to send an additional request to expand each of the distribution groups included in the response.</span></span>
  
## <a name="expand-a-contact-group-by-using-ews"></a><span data-ttu-id="6d0d2-135">EWS を使用して連絡先グループを展開する</span><span class="sxs-lookup"><span data-stu-id="6d0d2-135">Expand a contact group by using EWS</span></span>
<span data-ttu-id="6d0d2-136"><a name="bk_ExpandDGEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="6d0d2-136"></span></span>

<span data-ttu-id="6d0d2-137">連絡先グループを展開するのには XML の要求は、配布グループを展開するための要求に似ています。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-137">The XML request to expand a contact group is similar to a request to expand a distribution group.</span></span> <span data-ttu-id="6d0d2-138">メール ・ アドレスの代わりに、連絡先のグループの[アイテム Id](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx)を使用します。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-138">Instead of an email address, you use the [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) of the contact group.</span></span> <span data-ttu-id="6d0d2-139">この例では**アイテム Id**は、読みやすくするために短縮されます。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-139">The **ItemId** in this example is shortened for readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="http://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
         <ItemId xmlns="http://schemas.microsoft.com/exchange/services/2006/types" Id="AAMkADBlY…" />
      </Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="6d0d2-140">連絡先グループを展開するための要求に対する XML 応答の構造は、ユニバーサル配布グループを展開するための要求への応答と同じです。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-140">The structure of the XML response to a request to expand a contact group is the same as the response to a request to expand a universal distribution group.</span></span>
  
## <a name="see-also"></a><span data-ttu-id="6d0d2-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="6d0d2-141">See also</span></span>


- [<span data-ttu-id="6d0d2-142">Exchange の配布グループと EWS</span><span class="sxs-lookup"><span data-stu-id="6d0d2-142">Distribution groups and EWS in Exchange</span></span>](distribution-groups-and-ews-in-exchange.md)
    
- [<span data-ttu-id="6d0d2-143">Exchange EWS を使用して連絡先グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="6d0d2-143">Create contact groups by using EWS in Exchange</span></span>](how-to-create-contact-groups-by-using-ews-in-exchange.md)
    

