---
title: Exchange 2013 の EWS を使用して配布グループを展開する
manager: sethgros
ms.date: 11/16/2014
ms.audience: Developer
localization_priority: Normal
ms.assetid: 25ee84e7-63bc-4f51-9b7d-e7f46fd574d5
description: Exchange で EWS マネージ API または EWS を使用して配布グループを展開する方法について説明します。
ms.openlocfilehash: 2cbeb65b5a722bce4d5cab8fd716230874a6afca
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44528119"
---
# <a name="expand-distribution-groups-by-using-ews-in-exchange-2013"></a>Exchange 2013 の EWS を使用して配布グループを展開する

Exchange で EWS マネージ API または EWS を使用して配布グループを展開する方法について説明します。
  
[ExchangeService.ExpandGroup](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.exchangeservice.expandgroup%28v=exchg.80%29.aspx) EWS マネージ API メソッドまたは [ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) EWS 操作を使用して、配布グループを展開し、すべての受信者を識別できます。 
  
[ExpandGroup](https://msdn.microsoft.com/library/office/ee344007%28v=exchg.80%29.aspx) メソッドはオーバーロードされているため、いくつかの方法で呼び出すことができます。 
  
- [ExpandGroup(String)](https://msdn.microsoft.com/library/office/ee343988%28v=exchg.80%29.aspx): SMTP アドレスによって識別されるグループを展開します。 
    
- [ExpandGroup(EmailAddress)](https://msdn.microsoft.com/library/office/ee344007%28v=exchg.80%29.aspx): メール アドレスによって識別されるグループを展開します。 
    
- [ExpandGroup(ItemId)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx): グループ ID によって識別されるグループを展開します。 
    
- [ExpanGroup(String, String)](https://msdn.microsoft.com/library/office/ee356468%28v=exchg.80%29.aspx): SMTP アドレスと、そのアドレスのルーティングの種類によって識別されるグループを展開します。 
    
## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews-managed-api"></a>EWS マネージ API を使用してユニバーサル配布グループまたはセキュリティ グループを展開する
<a name="bk_ExpandDGEWSMA"> </a>

次の例では、メール アドレスを使ってユニバーサル配布グループまたはセキュリティ グループを展開する方法を示します。これは最も簡単なアプローチです。 この例では、**service** が有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。 
  
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

連絡先グループには関連付けられているメール アドレスがないため、[ExpandGroup(ItemId)](https://msdn.microsoft.com/library/office/ee356407%28v=exchg.80%29.aspx) メソッドを使用して、ItemId に基づいてグループを展開する必要があります。 前の例のように関数を作成し、2 番目のパラメーターの型を文字列から [ItemId](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemid%28v=exchg.80%29.aspx) に変更できます。
  
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

これで、Exchange サービスのオブジェクトと連絡先グループの **ItemId** を使用してこの関数を呼び出すことができます。 この例の **ItemId** は、読みやすさのために短くしてあることに注意してください。 
  
```cs
ExpandContactGroup(service, new ItemId("AAMkADBlY…");

```

## <a name="expand-a-universal-distribution-group-or-security-group-by-using-ews"></a>EWS を使用して、ユニバーサル配布グループまたはセキュリティ グループを展開する
<a name="bk_ExpandDGEWSMA"> </a>

次の例では、[ExpandDL](https://msdn.microsoft.com/library/1f7837e7-9eff-4e10-9577-c40f7ed6af94%28Office.15%29.aspx) 操作を使用するときにクライアントからサーバーに送信される XML 要求メッセージを示します。これは、EWS マネージ API を使用して[ユニバーサル配布グループを展開する](#bk_ExpandDGEWSMA)場合に、EWS マネージ API が送信する XML 要求でもあります。  
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
<s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
     xmlns:xsd="http://www.w3.org/2001/XMLSchema">
<ExpandDLResponse xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                      xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <ResponseMessages xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
    <ExpandDLResponseMessage ResponseClass="Success">
      <ResponseCode>NoError</ResponseCode>
      <DLExpansion IncludesLastItemInRange="true" TotalItemsInView="4">
        <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Sadie Daniels</Name>
          <EmailAddress>sadie@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Alfred Welker</Name>
          <EmailAddress>alfred@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>Mailbox</MailboxType>
        </Mailbox>
        <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Contoso Sales</Name>
          <EmailAddress>sales@contoso.com</EmailAddress>
          <RoutingType>SMTP</RoutingType>
          <MailboxType>PublicDL</MailboxType>
        </Mailbox>
        <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

連絡先グループを展開するための XML 要求は、配布グループを展開するための要求に似ています。 メール アドレスの代わりに、連絡先グループの [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) を使用します。 この例の **ItemId** は、読みやすさのために短くしてあります。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <ExpandDL xmlns="https://schemas.microsoft.com/exchange/services/2006/messages"
              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <Mailbox>
         <ItemId xmlns="https://schemas.microsoft.com/exchange/services/2006/types" Id="AAMkADBlY…" />
      </Mailbox>
    </ExpandDL>
  </soap:Body>
</soap:Envelope>
```

連絡先グループを展開するための要求に対する XML 応答の構造は、ユニバーサル配布グループを展開するための要求への応答と同じです。
  
## <a name="see-also"></a>関連項目


- [Exchange の配布グループと EWS](distribution-groups-and-ews-in-exchange.md)
    
- [Exchange で EWS を使用して連絡先グループを作成する](how-to-create-contact-groups-by-using-ews-in-exchange.md)
    

