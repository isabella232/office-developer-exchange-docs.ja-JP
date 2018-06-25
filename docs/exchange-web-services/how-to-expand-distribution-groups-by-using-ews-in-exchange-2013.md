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
# <a name="expand-distribution-groups-by-using-ews-in-exchange-2013"></a>Exchange 2013 の EWS を使用して配布グループを展開します。

Exchange で EWS マネージ API または EWS を使用して配布グループを展開する方法について説明します。
  
[ExchangeService.ExpandGroup](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドまたは[ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx)の EWS の操作を使用するには、すべての受信者を識別するのに配布グループを展開します。 
  
[ExpandGroup](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx)メソッドをオーバー ロードするためは、いくつかの方法で呼び出すことができます。 
  
- [ExpandGroup(String)](http://msdn.microsoft.com/en-us/library/office/ee343988%28v=exchg.80%29.aspx)では、SMTP アドレスによって識別されるグループを展開します。 
    
- [ExpandGroup(EmailAddress)](http://msdn.microsoft.com/en-us/library/office/ee344007%28v=exchg.80%29.aspx) - は、電子メール アドレスで識別されるグループを展開します。 
    
- [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx) ・ グループ ID で識別されるグループを展開します。 
    
- [ExpanGroup (文字列、文字列)](http://msdn.microsoft.com/en-us/library/office/ee356468%28v=exchg.80%29.aspx)では、SMTP アドレスとそのアドレスのルーティングの種類によって識別されるグループを展開します。 
    
## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews-managed-api"></a>EWS マネージ API を使用してユニバーサル配布グループまたはセキュリティ グループを展開する
<a name="bk_ExpandDGEWSMA"> </a>

次の例では、最も簡単な方法には、電子メール アドレスを使用して、ユニバーサル配布グループまたはセキュリティ グループを展開する方法を示します。 この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。 
  
```cs
// Return the expanded group.
   ExpandGroupResults myGroupMembers = service.ExpandGroup("employees@contoso.com");
// Display the group members.
   foreach (EmailAddress address in myGroupMembers.Members)
   {
      Console.WriteLine("Email Address: {0}", address);
   }

```

これは長いコードではなく、非常に基本的であり、お探しのものとは異なる可能性があります。ではもう一歩踏み込んでみましょう。配布グループには、他の配布グループを含めることもできます。単に展開した場合、含まれている配布グループのメール アドレスは出力されますが、グループが展開されるわけではありません。数行のコードを追加すると、グループを再帰的に展開して、すべての連絡先を出力できます。
  
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

これで、この新しい関数をコード内で呼び出して、最初のグループに含まれているすべてのパブリックな配布グループを展開できます。
  
```cs
ExpandDistributionLists(service, "employees@contoso.com");

```

## <a name="expand-a-contact-group-by-using-ews-managed-api"></a>EWS マネージ API を使用して連絡先グループを展開する
<a name="bk_ExpandDGEWSMA"> </a>

連絡先グループに関連付けられた電子メール アドレスがないために、 [ExpandGroup(ItemId)](http://msdn.microsoft.com/en-us/library/office/ee356407%28v=exchg.80%29.aspx)メソッドを使用して、アイテムの Id に基づくグループを展開する必要があります。 前の例のように、関数を作成し、[アイテム Id](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx)を文字列から 2 番目のパラメーターの型を変更できます。
  
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

これで、Exchange サービスのオブジェクトと連絡先のグループの**アイテム Id**を使用してこの関数を呼び出すことができます。 例では**アイテム Id**が読みやすさに省略されていることを注意してください。 
  
```cs
ExpandContactGroup(service, new ItemId("AAMkADBlY…");

```

## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews"></a>EWS を使用して、ユニバーサル配布グループまたはセキュリティ グループを展開する
<a name="bk_ExpandDGEWSMA"> </a>

[ExpandDL](http://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx)操作を使用する場合、サーバーへのクライアントから送信された XML 要求メッセージの例を次に示します。 EWS のマネージ API は、[ユニバーサル配布グループを展開](#bk_ExpandDGEWSMA)する EWS のマネージ API を使用する場合を送信する XML 要求にもです。 
  
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

次の例では、サーバーからクライアントに送信される XML 応答メッセージを示します。メールボックスとユニバーサル配布グループの両方が返されることにご注意ください。
  
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

EWS マネージ API を使用する場合とは異なり、EWS を使用してユニバーサル配布グループを展開する場合は、返される配布グループを再帰的に展開できません。応答に含まれている各配布グループを展開するには、追加の要求を送信する必要があります。
  
## <a name="expand-a-contact-group-by-using-ews"></a>EWS を使用して連絡先グループを展開する
<a name="bk_ExpandDGEWSMA"> </a>

連絡先グループを展開するのには XML の要求は、配布グループを展開するための要求に似ています。 メール ・ アドレスの代わりに、連絡先のグループの[アイテム Id](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx)を使用します。 この例では**アイテム Id**は、読みやすくするために短縮されます。 
  
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

連絡先グループを展開するための要求に対する XML 応答の構造は、ユニバーサル配布グループを展開するための要求への応答と同じです。
  
## <a name="see-also"></a>関連項目


- [Exchange の配布グループと EWS](distribution-groups-and-ews-in-exchange.md)
    
- [Exchange EWS を使用して連絡先グループを作成します。](how-to-create-contact-groups-by-using-ews-in-exchange.md)
    

