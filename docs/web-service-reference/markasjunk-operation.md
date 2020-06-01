---
title: MarkAsJunk 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1f71f04d-56a9-4fee-a4e7-d1034438329e
description: MarkAsJunk EWS 操作に関する情報を検索します。
ms.openlocfilehash: 25d6b01dfff64c4e45f3382223311219d349c165
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44468573"
---
# <a name="markasjunk-operation"></a>MarkAsJunk 操作

**Markasjunk** EWS 操作に関する情報を検索します。 
  
**Markasjunk**操作は、ブロックされた電子メールリストに対してユーザーを追加および削除し、電子メールメッセージを [迷惑メール] フォルダーに移動します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-markasjunk-operation"></a>MarkAsJunk 操作の使用

**Markasjunk**操作には、電子メール送信者を受信拒否リストに追加する必要があるかどうか、および対象の電子メールメッセージを既定の迷惑メールフォルダーまたは受信トレイフォルダーに移動する必要があるかどうかを示す2つのブールオプションがあります。 アクションは、 **Isjunk メール**属性と**moveitem**属性の値によって決まります。 **Isjunk メール**属性と**moveitem**属性の値の組み合わせに基づいて、次の操作を実行できます。 
  
- **Isjunk**属性が**true**に設定されていて、 **moveitem**属性が**true**に設定されている場合、対象の電子メールメッセージの送信者は、受信拒否リストに追加され、電子メールメッセージは迷惑メールフォルダーに移動されます。
    
- **Isjunk**属性が**true**に設定されていて、 **moveitem**属性が**false**に設定されている場合、移動先の電子メールメッセージの送信者は、受信拒否リストに追加され、電子メールメッセージはフォルダーから移動されません。
    
- **Isjunk**属性が**false**に設定されていて、 **moveitem**属性が**true**に設定されている場合、移動先の電子メールメッセージの送信者は、受信拒否リストから削除され、電子メールメッセージは受信トレイフォルダーに移動されます。
    
- **Isjunk**属性が**false**に設定されていて、 **moveitem**属性が**false**に設定されている場合、移動先の電子メールメッセージの送信者は、受信拒否リストから削除され、電子メールメッセージはフォルダーから移動されません。
    
> [!IMPORTANT]
> 受信拒否リストの内容は、EWS からは検出できません。 送信者が受信拒否リストに追加されている場合は、ブロックする送信者によって送信された電子メールメッセージのコピーを保持して、送信元のブロックを解除する必要があります。 
  
### <a name="markasjunk-operation-soap-headers"></a>MarkAsJunk 操作の SOAP ヘッダー

**Markasjunk**操作では、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアントアプリケーションが偽装しているユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは応答に適用されます。  <br/> |
   
## <a name="markasjunk-operation-request-example-add-a-sender-to-the-blocked-sender-list"></a>MarkAsJunk 操作要求の例: 送信者を受信拒否リストに追加します。

次の例は、 **Markasjunk**操作要求の例で、電子メールの送信者を受信拒否リストに追加し、その電子メールを迷惑メールフォルダーに移動する方法を示しています。 **Markasjunk**操作は、受信拒否リストに追加された送信者を参照するために使用される電子メールを識別する一意の電子メールメッセージ識別子を受け取ります。 
  
> [!NOTE]
> この記事のすべてのアイテム識別子と変更キーは、読みやすくするために短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
        <t:RequestServerVersion Version="Exchange2013" />
    </soap:Header>
    <soap:Body>
        <m:MarkAsJunk IsJunk="true" MoveItem="true">
            <m:ItemIds>
                <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYA" />
            </m:ItemIds>
        </m:MarkAsJunk>
    </soap:Body>
</soap:Envelope>

```

要求 SOAP 本文には、次の要素が含まれています。
  
- [MarkAsJunk](markasjunk.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="successful-markasjunk-operation-response"></a>正常な MarkAsJunk 操作の応答

次の例は、[ブロックする差出人のリスト] に送信者を追加し、その電子メールメッセージを迷惑メールフォルダーに移動するための、 **Markasjunk**操作要求に対する正常な応答を示しています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                             MinorVersion="0" 
                             MajorBuildNumber="545" 
                             MinorBuildNumber="11" 
                             Version="Exchange2013" 
                             xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                             xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
        <m:MarkAsJunkResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
           <m:ResponseMessages>
               <m:MarkAsJunkResponseMessage ResponseClass="Success">
                  <m:ResponseCode>NoError</m:ResponseCode>
                 <m:MovedItemId Id="AAMkAD=" ChangeKey="CQAAABYu" />
               </m:MarkAsJunkResponseMessage>
           </m:ResponseMessages>
        </m:MarkAsJunkResponse>
    </s:Body>
</s:Envelope>
```

応答 SOAP 本文には、次の要素が含まれています。
  
- [MarkAsJunkResponse](markasjunkresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
    
- [ResponseCode](responsecode.md)
    
- [MovedItemId](moveditemid.md)
    
## <a name="markasjunk-operation-request-example-remove-a-sender-from-the-blocked-sender-list"></a>MarkAsJunk 操作要求の例: 受信拒否リストから送信者を削除します

次の例は、 **Markasjunk**操作要求の例で、電子メールメッセージの送信者を受信拒否リストから削除し、その電子メールメッセージを受信トレイフォルダーに移動する方法を示しています。 受信拒否リストから送信者を削除するには、ブロックする送信者によって送信される電子メールメッセージを保持する必要があります。 送信者の電子メールアドレスは、送信者によって送信された電子メールメッセージに関連付けられています。 参照電子メールメッセージがユーザーのメールボックスに存在しなくなった場合、受信拒否リストからの送信者の削除は成功しません。 送信者に電子メールメッセージを関連付けるために使用されるアイテム識別子は、Exchange メールボックス内に存在するアイテムに関連付けられている必要があります。 以前にブロックされた送信者が送信したアイテムを格納するための非表示のフォルダーを作成して、クライアントアプリケーションからの送信者のブロックを解除できるようにすることをお勧めします。 Exchange メールボックスからアイテムが削除された場合は、管理者が Exchange 管理コンソールを使用して、受信拒否リストにアクセスして送信者を一覧から削除する必要があります。 Exchange 管理コンソールを使用してユーザーのブロックを解除する方法については、「 [Office 365 で差出人セーフリストと受信拒否設定を構成する方法](https://support.microsoft.com/kb/2545137)」を参照してください。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
    <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
    </soap:Header>
    <soap:Body>
      <m:MarkAsJunk IsJunk="false" MoveItem="true">
        <m:ItemIds>
          <t:ItemId Id="AAMkAD=" ChangeKey="CQAAABYu" />
        </m:ItemIds>
      </m:MarkAsJunk>
    </soap:Body>
 </soap:Envelope>

```

受信拒否リストから送信者を削除するための正常な応答は、受信拒否リストに送信者を追加する際の応答と同じです。
  
要求 SOAP 本文には、次の要素が含まれています。
  
- [MarkAsJunk](markasjunk.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="markasjunk-operation-error-response"></a>MarkAsJunk 操作エラー応答

次の例は、 **Markasjunk**操作要求へのエラー応答を示しています。 これは、アイテム識別子によって指定された電子メールメッセージがメールボックスに存在しなくなったときに、受信拒否リストに送信者を追加または削除する要求に対する応答です。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="545" 
                         MinorBuildNumber="11" 
                         Version="Exchange2013" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:MarkAsJunkResponseMessage ResponseClass="Error">
          <m:MessageText>The specified object was not found in the store.</m:MessageText>
          <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
          <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
        </m:MarkAsJunkResponseMessage>
      </m:ResponseMessages>
    </m:MarkAsJunkResponse>
  </s:Body>
</s:Envelope>
```

エラー応答 SOAP 本文には、次の要素が含まれています。
  
- [MarkAsJunkResponse](markasjunkresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>関連項目

- [Exchange での EWS 操作](ews-operations-in-exchange.md)
    
- [GetItem 操作](getitem-operation.md)GetItem 操作 
    
- [FindItem 操作](finditem-operation.md)
    

