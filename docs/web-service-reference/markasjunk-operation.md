---
title: MarkAsJunk 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 1f71f04d-56a9-4fee-a4e7-d1034438329e
description: MarkAsJunk EWS 操作に関する情報を検索します。
ms.openlocfilehash: b165b415ce9380846b49d15dd321bfddba72b749
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59524736"
---
# <a name="markasjunk-operation"></a>MarkAsJunk 操作

**MarkAsJunk** EWS 操作に関する情報を検索します。 
  
**MarkAsJunk** 操作では、ブロックされた電子メール リストからユーザーを追加および削除し、電子メール メッセージを迷惑メール フォルダーに移動します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-markasjunk-operation"></a>MarkAsJunk 操作の使用

**MarkAsJunk** 操作には、受信拒否リストにメール送信者を追加する必要があるかどうか、およびターゲット電子メール メッセージを既定の迷惑メール フォルダーまたは受信トレイ フォルダーに移動するかどうかを示すブール型 (Boolean) の 2 つのオプションが含まれている。 アクションは **、IsJunk** 属性と MoveItem 属性の **値によって決** まります。 **IsJunk** 属性と MoveItem 属性の値の組み合わせに基づいて実行できるアクションを次 **に示** します。 
  
- **IsJunk** 属性が **true** に設定され **、MoveItem** 属性が **true** に設定されている場合、ターゲット電子メール メッセージの送信者がブロックされた送信者リストに追加され、電子メール メッセージが迷惑メール フォルダーに移動されます。
    
- **IsJunk** 属性が **true** に設定され **、MoveItem** 属性が **false** に設定されている場合、ターゲット電子メール メッセージの送信者がブロックされた送信者リストに追加され、電子メール メッセージはフォルダーから移動されません。
    
- **IsJunk** 属性が **false** に設定され **、MoveItem** 属性が **true** に設定されている場合、ターゲット電子メール メッセージの送信者はブロックされた送信者リストから削除され、電子メール メッセージは受信トレイ フォルダーに移動されます。
    
- **IsJunk** 属性が **false** に設定され **、MoveItem** 属性が **false** に設定されている場合、ターゲット電子メール メッセージの送信者はブロックされた送信者リストから削除され、電子メール メッセージはフォルダーから移動されません。
    
> [!IMPORTANT]
> ブロックされた送信者リストの内容は、EWS から検出できません。 送信者がブロックされた送信者リストに追加される場合は、ブロックされた送信者から送信された電子メール メッセージのコピーを保持して、今後送信者のブロックを解除する必要があります。 
  
### <a name="markasjunk-operation-soap-headers"></a>MarkAsJunk 操作 SOAP ヘッダー

**MarkAsJunk 操作** では、次の表に示す SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**Element**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装しているユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |メールボックスへのアクセスに使用する RFC 3066「言語の識別用タグ」で定義されているカルチャを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマ バージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="markasjunk-operation-request-example-add-a-sender-to-the-blocked-sender-list"></a>MarkAsJunk 操作要求の例: 受信拒否リストに送信者を追加する

**MarkAsJunk** 操作要求の次の例は、電子メールの送信者をブロックされた送信者リストに追加し、電子メールを迷惑メール フォルダーに移動する方法を示しています。 **MarkAsJunk** 操作は、一意の電子メール メッセージ識別子を受け入れ、ブロックされた送信者リストに追加される送信者を参照するために使用される電子メールを識別します。 
  
> [!NOTE]
> この記事のすべてのアイテム識別子と変更キーは、読みやすさを維持するために短縮されています。 
  
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
    
## <a name="successful-markasjunk-operation-response"></a>MarkAsJunk 操作応答の成功

次の例は、受信拒否リストに送信者を追加し、電子メール メッセージを迷惑メール フォルダーに移動する **MarkAsJunk** 操作要求に対する正常な応答を示しています。 
  
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
    
## <a name="markasjunk-operation-request-example-remove-a-sender-from-the-blocked-sender-list"></a>MarkAsJunk 操作要求の例: ブロックされた送信者リストから送信者を削除する

**MarkAsJunk** 操作要求の次の例は、ブロックされた送信者リストから電子メール メッセージの送信者を削除し、電子メール メッセージを受信トレイ フォルダーに移動する方法を示しています。 ブロックされた送信者リストから送信者を削除するには、ブロックされた送信者から送信された電子メール メッセージを保持する必要があります。 送信者の電子メール アドレスは、送信者によって送信された電子メール メッセージに関連付けられている。 参照電子メール メッセージがユーザーのメールボックスに存在しなくなった場合、ブロックされた送信者リストから送信者を削除すると成功しません。 電子メール メッセージを送信者に関連付ける場合に使用するアイテム識別子は、メールボックス内に存在するアイテムExchange必要があります。 以前にブロックされた送信者によって送信されたアイテムを格納する隠しフォルダーを作成して、送信者をクライアント アプリケーションからブロック解除することをお勧めします。 Exchange メールボックスからアイテムが削除された場合、管理者は Exchange 管理コンソール を使用して、ブロックされた送信者リストにアクセスしてリストから送信者を削除する必要があります。 Exchange 管理コンソール を使用してユーザーのブロックを解除する方法については、「Office 365 で差出人セーフ リストと受信拒否の設定を構成する方法」[を参照してください](https://support.microsoft.com/kb/2545137)。
  
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

受信拒否リストから送信者を削除するための正常な応答は、受信拒否リストに送信者を追加する応答と同じです。
  
要求 SOAP 本文には、次の要素が含まれています。
  
- [MarkAsJunk](markasjunk.md)
    
- [ItemIds](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="markasjunk-operation-error-response"></a>MarkAsJunk 操作エラー応答

次の例は **、MarkAsJunk** 操作要求に対するエラー応答を示しています。 これは、アイテム識別子で指定された電子メール メッセージがメールボックスに存在しなくなった場合に、受信拒否リストに送信者を追加または削除する要求に対する応答です。 
  
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

- [EWS 操作 (Exchange](ews-operations-in-exchange.md)
    
- [GetItem 操作](getitem-operation.md) GetItem 操作 
    
- [FindItem 操作](finditem-operation.md)
    

