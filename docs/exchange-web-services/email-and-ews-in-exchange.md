---
title: Exchange の電子メールと EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.assetid: 4d7bdb37-f7f1-409f-9749-f8bcde7dc52a
description: 電子メール メッセージの処理方法について説明します。これには、Exchange で EWS マネージ API または EWS を使用して電子メールを作成したり、他の電子メール関連タスクを実行する方法が含まれます。
localization_priority: Priority
ms.openlocfilehash: 323d9d2cc40aa86044a439ad53e53a4808916783
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: HT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44455444"
---
# <a name="email-and-ews-in-exchange"></a>Exchange の電子メールと EWS

電子メール メッセージの処理方法について説明します。これには、Exchange で EWS マネージ API または EWS を使用して電子メールを作成したり、他の電子メール関連タスクを実行する方法が含まれます。
  

  
Exchange で中核となるのは電子メールです。 ところで、電子メールとは何でしょうか?  Exchange では電子メール メッセージは[厳密に型指定されたアイテム](folders-and-items-in-ews-in-exchange.md#bk_item)です。つまり、送信する前であっても特定の[一連のプロパティ](email-properties-and-elements-in-ews-in-exchange.md)が含まれます。 電子メール メッセージは、EWS マネージ API では [EmailMessage](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx) クラスによって、EWS では [Message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) 要素とその子要素として表されます。 
  
EWS マネージ API では、**EmailMessage** オブジェクトは [Item](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx) オブジェクトから派生します。 **EmailMessage** クラスは、ほぼすべてのメッセージング シナリオで共通な [EmailMessage.Sender](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sender%28v=exchg.80%29.aspx) および [EmailMessage.IsRead](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.isread%28v=exchg.80%29.aspx) などの追加プロパティを提供して **Item** クラスを拡張します。 電子メール メッセージを取得、更新、削除するほとんどの操作は、**EmailMessage** オブジェクトまたは基本 **Item** オブジェクトを使用して行えます。作業対象のプロパティが [EmailMessageSchema](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessageschema%28v=exchg.80%29.aspx) クラスまたは [ItemSchema](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx) クラスのどちらにあるかによって使用するオブジェクトが異なります。 アイテムの作成の場合には異なります。**Item** クラスにはコンストラクターがないため、電子メールを作成する場合、[EmailMessage コンストラクター](https://msdn.microsoft.com/library/office/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx)を使用して作成し、[EmailMessage.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) または [EmailMessage.SendAndSaveCopy](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx) を使用して保存したり、送信してから保存したりします。 
  
同様に、EWS では、[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) 操作を [Message](https://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx) 要素と併用して電子メール メッセージを作成します。EWS を使用してメールを取得、更新、削除するには、追加プロパティが電子メール メッセージで使用できるという点を除き、変更対象が電子メール メッセージであるということは重要とはなりません。その他の厳密に型指定されたアイテムに使用されるのと同じ操作が電子メール メッセージにも使用されます。 
  
|**タスク**|**EWS マネージ API メソッド**|**EWS 操作**|
|:-----|:-----|:-----|
|作成  <br/> |[EmailMessage.Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) <br/> |[CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|取得  <br/> |[EmailMessage.Bind](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](https://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|更新  <br/> |[Item.Update](https://msdn.microsoft.com/library/dd635915%28v=exchg.80%29.aspx) <br/> |[UpdateItem](https://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|削除  <br/> |[Item.Delete](https://msdn.microsoft.com/library/dd635072%28v=exchg.80%29.aspx) <br/> |[DeleteItem](../web-service-reference/deleteitem-operation.md) <br/> |
   
電子メール メッセージは単純な[厳密に型指定されたアイテム](folders-and-items-in-ews-in-exchange.md#bk_item)であるため、場合によっては、[汎用アイテムを処理する](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)のと同じ方法で扱えます。  
  
## <a name="create-an-email-message-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して電子メール メッセージを作成する
<a name="bk_createewsma"> </a>

次の例のコードに示されているように、EWS マネージ API の [Save](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) メソッドを使用して電子メール メッセージを作成できます。 この例では、[下書き] フォルダーにメッセージを保存しますが、メッセージは送信しません。 メッセージを送信したり、メッセージの作成と送信を 1 ステップで行う方法については、[「Exchange で EWS を使用してメール メッセージを送信する」](how-to-send-email-messages-by-using-ews-in-exchange.md)を参照してください。
  
この例では、**service** が有効な [ExchangeService](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーから既に認証されていると想定しています。 
  
```cs
// Create a new email message.
EmailMessage message = new EmailMessage(service);
// Set properties on the email message.
message.ToRecipients.Add("mack@contoso.com");
message.Subject = "Project priorities";
message.Body = "(1) Buy pizza, (2) Eat pizza";
// Save the email message to the Drafts folder (where it can be retrieved, updated, and sent at a later time).
// This method call results in a CreateItem call to EWS.
message.Save(WellKnownFolderName.Drafts);
Console.WriteLine("A draft email message with the subject '" + message.Subject + "' has been saved to the Drafts folder.");
```

## <a name="create-an-email-message-by-using-ews"></a>EWS を使用して電子メール メッセージを作成する
<a name="bk_createews"> </a>

次の例に示されているように、EWS [CreateItem](https://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) 操作を使用して電子メール メッセージを作成できます。 また、これは[電子メール メッセージが作成](#bk_createewsma)されるときに EWS マネージ API が送信する XML 要求でもあります。 次の例では、[下書き] フォルダーにメッセージを保存しますが、メッセージは送信しません。 メッセージを送信したり、メッセージの作成と送信を 1 ステップで行う方法については、[「Exchange で EWS を使用してメール メッセージを送信する」](how-to-send-email-messages-by-using-ews-in-exchange.md)を参照してください。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010_SP2" />
  </soap:Header>
  <soap:Body>
    <m:CreateItem MessageDisposition="SaveOnly">
      <m:SavedItemFolderId>
        <t:DistinguishedFolderId Id="drafts" />
      </m:SavedItemFolderId>
      <m:Items>
        <t:Message>
          <t:Subject>Project priorities</t:Subject>
          <t:Body BodyType="HTML">(1) Buy pizza, (2) Eat pizza</t:Body>
          <t:ToRecipients>
            <t:Mailbox>
              <t:EmailAddress>mack@contoso.com</t:EmailAddress>
            </t:Mailbox>
          </t:ToRecipients>
        </t:Message>
      </m:Items>
    </m:CreateItem>
  </soap:Body>
</soap:Envelope>

```

サーバーは、**CreateItemResponse** メッセージで [CreateItem](https://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) 要求に応答します。このメッセージには、電子メールが正常に作成されたことを示す [NoError](https://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) の **ResponseCode** 値、および新しく作成されたメッセージの [ItemId](https://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) が含まれます。 
  
## <a name="get-update-and-delete-an-email-message-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して電子メール メッセージを取得、更新、削除する
<a name="bk_getewsma"> </a>

EWS マネージ API を使用すると、Exchange ストアの汎用アイテムで実行するのと同じ方法で電子メール メッセージの取得、更新、削除を行えます。 詳細は、[「Exchange で EWS を使用して Exchange メールボックス アイテムを操作する」](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)を参照してください。
  
電子メール メッセージを更新する場合は、書き込み可能な電子メール メッセージ プロパティの一覧を[「Exchange における EWS でのメールのプロパティと要素」](email-properties-and-elements-in-ews-in-exchange.md)で確認してください。 下書きメッセージを更新してから送信するには、「[EWS マネージ API を使用して下書き電子メール メッセージを送信する](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftewsma)」をご覧ください。
  
## <a name="get-update-and-delete-an-email-message-by-using-ews"></a>EWS を使用して電子メール メッセージを取得、更新、削除する
<a name="bk_getews"> </a>

EWS を使用すると、Exchange ストアの汎用アイテムで実行するのと同じ方法で電子メール メッセージの取得、更新、削除を行えます。 詳細は、[「Exchange で EWS を使用して Exchange メールボックス アイテムを操作する」](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)を参照してください。
  
電子メール メッセージを更新する場合は、書き込み可能な電子メール メッセージ プロパティの一覧を[「Exchange における EWS でのメールのプロパティと要素」](email-properties-and-elements-in-ews-in-exchange.md)で確認してください。 下書きメッセージを更新してから送信するには、「[EWS を使用して下書き電子メール メッセージを送信する](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews)」をご覧ください。
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_inthissection"> </a>

- [Exchange における EWS の電子メール プロパティと要素](email-properties-and-elements-in-ews-in-exchange.md)
    
- [Exchange で EWS を使用してメール メッセージを送信する](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [Exchange において EWS を使用してメール メッセージに応答する](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [Exchange において EWS を使用してメール メッセージを移動およびコピーする](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [Exchange において EWS を使用して会話を処理する](how-to-work-with-conversations-by-using-ews-in-exchange.md)
    
- [Exchange において EWS を使用してメール メッセージからエンティティを抽出する](how-to-extract-an-entity-from-an-email-message-by-using-ews-in-exchange.md)
    
- [Exchange で EWS を使用してバッチ処理でメール メッセージを処理する](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目


- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [Exchange の EWS のフォルダーとアイテム](folders-and-items-in-ews-in-exchange.md)
    

