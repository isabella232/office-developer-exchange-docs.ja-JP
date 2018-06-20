---
title: MarkAsJunk の操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1f71f04d-56a9-4fee-a4e7-d1034438329e
description: 操作 MarkAsJunk EWS についての情報を検索します。
ms.openlocfilehash: b9d79e6fbec87ce41030b4981f3c16f2f9ce9507
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832353"
---
# <a name="markasjunk-operation"></a>MarkAsJunk の操作

**MarkAsJunk** EWS の操作に関する情報を検索します。 
  
**MarkAsJunk**操作は、追加しブロックされた電子メール] ボックスの一覧からユーザーを削除し、電子メール メッセージを [迷惑メール フォルダーに移動します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-markasjunk-operation"></a>MarkAsJunk 操作を使用します。

**MarkAsJunk**操作には、受信拒否リストに、電子メールの送信者を追加するか、移行先の電子メール メッセージを既定の [迷惑メール] フォルダーまたは [受信トレイ] フォルダーに移動するかどうかを示すために 2 つのブール型のオプションが含まれています。 アクションは、**引数 IsJunk**と**MoveItem**属性の値によって決まります。 **引数 IsJunk**と**MoveItem**属性の値の組み合わせに基づいて使用可能なアクションは、次のように。 
  
- **引数 IsJunk**属性が**true**に設定すると、 **MoveItem**属性が**true**に設定、ターゲットの電子メール メッセージの送信者がブロックされる送信者の一覧に追加し、Dmail を迷惑メール フォルダーに電子メール メッセージを移動します。
    
- **引数 IsJunk**属性が**true**に設定すると、 **MoveItem**属性が**false**に設定、ターゲットの電子メール メッセージの送信者がブロックされる送信者の一覧に追加し、フォルダーから電子メール メッセージが移動しません。
    
- **引数 IsJunk**属性が設定されている場合**は true**、ブロックする送信者の一覧から削除対象の電子メール ティーの送信者に**false を指定**し、 **MoveItem**属性が設定されてし、電子メール メッセージは [受信トレイ] フォルダーに移動します。
    
- **引数 IsJunk**属性が**false**に設定されて場合は、 **MoveItem**属性が**false**に設定対象の電子メール メッセージの送信者がブロックされる送信者の一覧から削除し、フォルダーから電子メール メッセージが移動しません。
    
> [!IMPORTANT]
> 受信拒否リストの内容は、EWS から検出可能ではありません。 受信拒否リストに送信者を追加する場合、将来的に、送信者のブロックを解除するのには、ブロックされている送信者から送信された電子メール メッセージのコピーを保持する必要があります。 
  
### <a name="markasjunk-operation-soap-headers"></a>MarkAsJunk 操作の SOAP ヘッダー

**MarkAsJunk**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装するユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="markasjunk-operation-request-example-add-a-sender-to-the-blocked-sender-list"></a>MarkAsJunk 操作の要求の使用例: 受信拒否リストに送信者を追加

**MarkAsJunk**操作要求の次の例では、電子メールの送信者を受信拒否リストに追加し、[迷惑メール] フォルダーに電子メールを移動する方法を示します。 **MarkAsJunk**操作では、送信者が受信拒否リストに追加するを参照するために使用される電子メールを識別する一意の電子メール メッセージの id を受け取ります。 
  
> [!NOTE]
> すべての項目の識別子と変更キーをこの資料では、読みやすさを保持するために短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
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

要求 SOAP 本体にはには、次の要素が含まれています。
  
- [MarkAsJunk](markasjunk.md)
    
- [Itemid](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="successful-markasjunk-operation-response"></a>MarkAsJunk 操作の成功の応答

次の例では、受信拒否リストに送信者を追加し、電子メール メッセージを [迷惑メール フォルダーに移動する**MarkAsJunk**操作要求に正常な応答を示します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
    <s:Header>
        <h:ServerVersionInfo MajorVersion="15" 
                             MinorVersion="0" 
                             MajorBuildNumber="545" 
                             MinorBuildNumber="11" 
                             Version="Exchange2013" 
                             xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                             xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                             xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
    </s:Header>
    <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
            xmlns:xsd="http://www.w3.org/2001/XMLSchema">
        <m:MarkAsJunkResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                              xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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
    
## <a name="markasjunk-operation-request-example-remove-a-sender-from-the-blocked-sender-list"></a>MarkAsJunk 操作の要求の例: ブロックされた送信者の一覧から送信者を削除します。

**MarkAsJunk**操作要求の次の例では、電子メール メッセージの送信者を受信拒否リストから削除し、電子メール メッセージを受信トレイ フォルダーに移動する方法を示します。 禁止された送信者の一覧から送信者を削除するのには、ブロックされている送信者から送信された電子メール メッセージを保持する必要があります。 送信者の電子メール アドレスは、送信者によって送信された電子メール メッセージに関連付けられます。 禁止された送信者の一覧から送信者を削除することも、参照の電子メール メッセージがユーザーのメールボックスに存在しない場合は失敗します。 項目 id、送信者の電子メール メッセージを関連付けるために使用は、Exchange のメールボックスに存在する項目に関連付けられているである必要があります。 送信者がクライアント アプリケーションから受信できるようにするために、以前にブロックされた送信者によって送信されたアイテムを格納する非表示のフォルダーを作成することをお勧めします。 イベントで Exchange メールボックスから項目を削除すると、管理者は Exchange 管理コンソールのを使用して、一覧から送信者を削除するのにはブロックされている送信者リストにアクセスするには。 Exchange 管理コンソールのを使用してユーザーのブロックを解除する方法の詳細については、 [[差出人セーフ リストおよび受信拒否の設定で Office 365 を構成する方法](http://support.microsoft.com/kb/2545137)を参照してください。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
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

禁止された送信者の一覧から送信者を削除するための正常な応答は、受信拒否リストに送信者を追加するための反応と同じです。
  
要求 SOAP 本体にはには、次の要素が含まれています。
  
- [MarkAsJunk](markasjunk.md)
    
- [Itemid](itemids.md)
    
- [ItemId](itemid.md)
    
## <a name="markasjunk-operation-error-response"></a>MarkAsJunk 操作のエラー応答

**MarkAsJunk**操作の要求に対してエラー応答の例を次に示します。 これは、追加または項目の識別子で指定された電子メール メッセージがメールボックスに存在しない場合、ブロックする送信者の一覧から送信者を削除する要求に応答します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="545" 
                         MinorBuildNumber="11" 
                         Version="Exchange2013" 
                         xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                          xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

エラー応答 SOAP 本体にはには、次の要素が含まれています。
  
- [MarkAsJunkResponse](markasjunkresponse.md)
    
- [ResponseMessages](responsemessages.md)
    
- [MarkAsJunkResponseMessage](markasjunkresponsemessage.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
## <a name="see-also"></a>関連項目

- [Exchange での EWS の操作](ews-operations-in-exchange.md)
    
- [GetItem 操作](getitem-operation.md)GetItem 操作 
    
- 
  [FindItem 操作](finditem-operation.md)
    

