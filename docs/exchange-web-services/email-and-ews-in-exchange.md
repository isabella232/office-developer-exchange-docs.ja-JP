---
title: Exchange の電子メールと EWS
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: 4d7bdb37-f7f1-409f-9749-f8bcde7dc52a
description: 電子メール メッセージの処理方法について説明します。これには、Exchange で EWS マネージ API または EWS を使用して電子メールを作成したり、他の電子メール関連タスクを実行する方法が含まれます。
ms.openlocfilehash: d222be7409a3c3f4613a2be39b83b977fabb09e8
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758886"
---
# <a name="email-and-ews-in-exchange"></a>Exchange の電子メールと EWS

電子メール メッセージの処理方法について説明します。これには、Exchange で EWS マネージ API または EWS を使用して電子メールを作成したり、他の電子メール関連タスクを実行する方法が含まれます。
  

  
中核となる、Exchange はメールです。 電子メール e メールは、何でしょうか。 電子メール メッセージは[厳密に型指定の項目](folders-and-items-in-ews-in-exchange.md#bk_item)のいずれかの Exchange に含まれること、特定[のプロパティの設定](email-properties-and-elements-in-ews-in-exchange.md)、送信することにも。 電子メール メッセージは、EWS のマネージ API の[なか](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage%28v=exchg.80%29.aspx)のクラスと[メッセージ](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx)の要素および EWS では、その子要素によって表されます。 
  
EWS のマネージ API では、 **email メッセージ**オブジェクトは、 [Item](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.item%28v=exchg.80%29.aspx)オブジェクトから派生します。 **なか**クラスは、ほぼすべてのメッセージング シナリオに共通では[EmailMessage.Sender](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sender%28v=exchg.80%29.aspx)と[EmailMessage.IsRead](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.isread%28v=exchg.80%29.aspx)のような追加のプロパティを提供することにより**項目**クラスを拡張します。 取得、更新、または**なか**オブジェクトまたは[EmailMessageSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessageschema%28v=exchg.80%29.aspx)または、[プロパティを扱う場合は、基本**項目**オブジェクトを使用して行うことができますほとんどの場合、電子メール メッセージを削除するときItemSchema](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.itemschema%28v=exchg.80%29.aspx)クラス。 アイテムの作成とは異なる**項目**クラスがコンス トラクターを持たないためため、電子メールを作成するときに使用する[コンス トラクターのなか](http://msdn.microsoft.com/en-us/library/office/microsoft.exchange.webservices.data.emailmessage.emailmessage%28v=exchg.80%29.aspx)と、 [EmailMessage.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx)または[EmailMessage.SendAndSaveCopy を作成するには](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.sendandsavecopy%28v=exchg.80%29.aspx)保存または送信し、それを保存するためのメソッドです。 
  
同様に、EWS でを使用して[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx)操作[メッセージ](http://msdn.microsoft.com/library/2400b33c-43b2-4fc2-b6fb-275a99e0e810%28Office.15%29.aspx)要素を使用して電子メール メッセージを作成します。 取得、更新、または EWS を使用して電子メールを削除、変更されている項目が電子メール メッセージであることは重要ですが、追加のプロパティが電子メール メッセージで使用可能であること以外ではありません。 電子メール メッセージを他の厳密に型指定された項目に使用されるのと同じ操作が使用されます。 
  
|**タスク**|**EWS マネージ API メソッド**|**EWS 操作**|
|:-----|:-----|:-----|
|作成  <br/> |[EmailMessage.Save](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx) <br/> |[CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx) <br/> |
|取得  <br/> |[EmailMessage.Bind](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.bind%28v=exchg.80%29.aspx) <br/> |[GetItem](http://msdn.microsoft.com/library/e8492e3b-1c8d-4b14-8070-9530f8306edd%28Office.15%29.aspx) <br/> |
|更新  <br/> |[Item.Update](http://msdn.microsoft.com/en-us/library/dd635915%28v=exchg.80%29.aspx) <br/> |[UpdateItem](http://msdn.microsoft.com/library/5d027523-e0bc-4da2-b60b-0cb9fc1fdfe4%28Office.15%29.aspx) <br/> |
|削除  <br/> |[Item.Delete](http://msdn.microsoft.com/en-us/library/dd635072%28v=exchg.80%29.aspx) <br/> |[DeleteItem](http://msdn.microsoft.com/library/3e26c416-fa12-476e-bfd2-5c1f4bb7b348%28Office.15%29.aspx) <br/> |
   
電子メールは、メッセージの[項目を厳密に型指定](folders-and-items-in-ews-in-exchange.md#bk_item)をするだけであるため場合によっては、作業中と同じようにその[汎用的な項目を操作します](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)。 
  
## <a name="create-an-email-message-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して電子メール メッセージを作成する
<a name="bk_createewsma"> </a>

次の例のコードに示すように、EWS のマネージ API の[保存](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.emailmessage.save%28v=exchg.80%29.aspx)メソッドを使用して、電子メール メッセージを作成します。 例は、下書きフォルダーにメッセージを保存するだけで、メッセージは送信されないことを確認します。 メッセージを送信または作成し、1 つのステップで、メッセージを送信する方法の詳細については、 [Exchange での EWS を使用して、電子メール メッセージの送信](how-to-send-email-messages-by-using-ews-in-exchange.md)を参照してください。
  
この例では、 **service** が有効な [ExchangeService](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice%28v=exchg.80%29.aspx) オブジェクトであり、ユーザーが Exchange サーバーに既に認証されていると想定しています。 
  
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

EWS [CreateItem](http://msdn.microsoft.com/library/fe6bb7fc-8918-4e6e-b0a1-b7e0ef44c3d1%28Office.15%29.aspx)操作を使用して電子メール メッセージを作成するには、次の例のようにします。 これは、XML の要求の場合、EWS のマネージ API を送信する[電子メール メッセージを作成](#bk_createewsma)します。 注意してください次の例は、下書きフォルダーにメッセージを保存するだけのメッセージを送信しません。 メッセージを送信または作成し、1 つのサイトで、メッセージを送信する方法の詳細については、 [Exchange での EWS を使用して、電子メール メッセージの送信](how-to-send-email-messages-by-using-ews-in-exchange.md)を参照してください。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
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

サーバーは、**CreateItemResponse** メッセージで [CreateItem](http://msdn.microsoft.com/library/742a46a0-2475-45a0-b44f-90639a3f5a43%28Office.15%29.aspx) 要求に応答します。このメッセージには、電子メールが正常に作成されたことを示す [NoError](http://msdn.microsoft.com/library/4b84d670-74c9-4d6d-84e7-f0a9f76f0d93%28Office.15%29.aspx) の **ResponseCode** 値、および新しく作成されたメッセージの [ItemId](http://msdn.microsoft.com/library/3350b597-57a0-4961-8f44-8624946719b4%28Office.15%29.aspx) が含まれます。 
  
## <a name="get-update-and-delete-an-email-message-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して電子メール メッセージを取得、更新、削除する
<a name="bk_getewsma"> </a>

取得、更新、または Exchange ストアからの任意の一般的な項目では、これらのアクションを実行することと同じ方法で電子メール メッセージを削除するのには、EWS のマネージ API を使用できます。 詳細については、 [Exchange EWS を使用して Exchange メールボックスのアイテムの作業](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)を参照してください。
  
電子メール メッセージを更新する場合は、書き込み可能な電子メール メッセージのプロパティの一覧については[プロパティおよび EWS での要素を Exchange メール](email-properties-and-elements-in-ews-in-exchange.md)を参照してください。 下書きメッセージを送信するには、それを更新した後に、 [EWS のマネージ API を使用して、下書き電子メール メッセージを送信する](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftewsma)を参照してください。
  
## <a name="get-update-and-delete-an-email-message-by-using-ews"></a>EWS を使用して電子メール メッセージを取得、更新、削除する
<a name="bk_getews"> </a>

取得、更新、および Exchange ストアからの任意の一般的な項目では、これらのアクションを実行することと同じ方法で電子メール メッセージを削除するのには、EWS を使用できます。 詳細については、 [Exchange EWS を使用して Exchange メールボックスのアイテムの作業](how-to-work-with-exchange-mailbox-items-by-using-ews-in-exchange.md)を参照してください。
  
電子メール メッセージを更新する場合は、書き込み可能な電子メール メッセージのプロパティの一覧については[プロパティおよび EWS での要素を Exchange メール](email-properties-and-elements-in-ews-in-exchange.md)を参照してください。 下書きメッセージを送信するは、それを更新した後、 [EWS を使用して、下書き電子メール メッセージを送信する](how-to-send-email-messages-by-using-ews-in-exchange.md#bk_senddraftews)を参照してください。
  
## <a name="in-this-section"></a>このセクションの内容
<a name="bk_inthissection"> </a>

- [EWS での要素のプロパティとの Exchange 電子メールします。](email-properties-and-elements-in-ews-in-exchange.md)
    
- [EWS を使用して Exchange が電子メール メッセージを送信します。](how-to-send-email-messages-by-using-ews-in-exchange.md)
    
- [EWS を使用して Exchange が電子メール メッセージに応答します。](how-to-respond-to-email-messages-by-using-ews-in-exchange.md)
    
- [移動し、EWS を使用して Exchange が電子メール メッセージをコピー](how-to-move-and-copy-email-messages-by-using-ews-in-exchange.md)
    
- [Exchange EWS を使用して会話を扱う](how-to-work-with-conversations-by-using-ews-in-exchange.md)
    
- [EWS を使用して Exchange が電子メール メッセージからエンティティを抽出します。](how-to-extract-an-entity-from-an-email-message-by-using-ews-in-exchange.md)
    
- [電子メール メッセージを Exchange で EWS を使用してバッチ プロセス](how-to-process-email-messages-in-batches-by-using-ews-in-exchange.md)
    
## <a name="see-also"></a>関連項目


- [Exchange の Web サービス クライアントを開発する](develop-web-service-clients-for-exchange.md)
    
- [Exchange の EWS のフォルダーとアイテム](folders-and-items-in-ews-in-exchange.md)
    

