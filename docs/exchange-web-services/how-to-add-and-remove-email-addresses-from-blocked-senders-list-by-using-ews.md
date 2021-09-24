---
title: Exchange で EWS を使用して、受信拒否リストに対してメール アドレスを追加、削除する
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.localizationpriority: medium
ms.assetid: b88288ee-6af7-45b5-a55c-5929cd0c16f1
description: 受信拒否リストに対してメール アドレスを追加および削除するために EWS マネージ API または EWS を使用する方法を説明します。
ms.openlocfilehash: 4deacbfa6e146675e3248e3932734a1492645246
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512206"
---
# <a name="add-and-remove-email-addresses-from-the-blocked-senders-list-by-using-ews-in-exchange"></a>Exchange で EWS を使用して、受信拒否リストに対してメール アドレスを追加、削除する

受信拒否リストに対してメール アドレスを追加および削除するために EWS マネージ API または EWS を使用する方法を説明します。
  
ユーザーの [迷惑メール] オプションの [受信拒否リスト] によって、指定した送信者からのすべてのメール メッセージを迷惑メール フォルダーに移動する方法が提供されています。EWS マネージ API または EWS アプリケーションで、受信拒否リストに対してメール アドレスの追加と削除を行えるようにできます。
  
電子メール アドレスを [受信拒否リスト] に追加または削除する前に、電子メール アドレスからのメッセージがユーザーのメールボックスに存在している必要があります。 [ExchangeService.MarkAsJunk](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) EWS マネージ API メソッドと[MarkAsJunk](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) EWS 操作では、アイテム ID のコレクションを使用します。 コレクション内のアイテムの ID は、迷惑メールの状態を変更するメールボックス内のメッセージを示します。 
  
[Get-MailboxJunkEmailConfiguration](https://technet.microsoft.com/library/dd979784%28v=exchg.150%29.aspx)および[Set-MailboxJunkEmailConfiguration](https://technet.microsoft.com/library/dd979780%28v=exchg.150%29.aspx) Exchange Management Shell コマンドレットを使用して、ブロックされた送信者リストに直接アクセスできます。 
  
## <a name="add-an-email-address-to-or-remove-it-from-the-blocked-senders-list-by-using-the-ews-managed-api"></a>EWS マネージ API を使用して、受信拒否リストに対してメール アドレスを追加または削除します。
<a name="bk_AddRemoveEWSMA"> </a>

メール メッセージの送信者を受信拒否リストに追加するには、**MarkAsJunk** メソッドを使用し、**isJunk** パラメーターを **true** にセットします。メール メッセージの送信者を受信拒否リストから削除するには、**isJunk** パラメーターを **false** にセットします。
  
次の例では、メッセージの迷惑ステータスを変更するための **MarkAsJunk** メソッドの使用方法を示します。 
  
```cs
private static void MarkMessageAsJunk(ExchangeService service, ItemId messageId, bool isJunk, bool moveItem)
{
    List<ItemId> junkItemIds = new List<ItemId>();
    junkItemIds.Add(messageId);
    ServiceResponseCollection<MarkAsJunkResponse> responseCollection = null;
    try
    {
        // If isJunk is true, the sender of the email message is added to 
        // the Blocked Senders List. If isJunk is false, the sender is removed
        // from the list (if present).
        responseCollection = service.MarkAsJunk(junkItemIds, isJunk, moveItem);
    }
    catch (ServiceResponseException ex)
    {
        Console.WriteLine("Error marking item as junk: {0}", ex.ErrorCode);
        return;
    }
    foreach (MarkAsJunkResponse response in responseCollection)
    {
        if (response.Result == ServiceResult.Success)
        {
            Console.WriteLine("Successfully marked message as {0}junk.", isJunk ? "": "NOT ");
            if (moveItem)
            {
                Console.WriteLine("New item ID: {0}", response.MovedItemId.ToString());
            }
        }
        else
        {
            Console.WriteLine("[{0}]: {1}", response.Result.ToString(),
                response.ErrorCode.ToString());
        }
    }
}
```

## <a name="add-an-email-address-to-or-remove-it-from-the-blocked-senders-list-by-using-ews"></a>EWS を使用して、受信拒否リストに対してメール アドレスを追加または削除する
<a name="bk_AddRemoveEWS"> </a>

次の EWS の SOAP 要求は、[MarkAsJunk](https://msdn.microsoft.com/library/f06bafc6-7ee3-4b2b-9fd1-7c51328f4729%28Office.15%29.aspx) 要素の **IsJunk** 属性を **true** に設定して、アイテムを迷惑アイテムとしてマークします。また、**MarkAsJunk** 要素の **MoveItem** 属性を **true** に設定して、メッセージを迷惑メール フォルダーに移動します。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
    xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
    xmlns:soap="https://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:MarkAsJunk IsJunk="true" MoveItem="true">
      <m:ItemIds>
        <t:ItemId Id="AAMkADg1OWUwODcyLTg4M2MtNDAyMS05YjI0LTI5ZGM5OTU4Njk3YwBGAAAAAADPriAxh444TpHj2GoQxWQNBwAN+VjmVZl5Rq1ymCq5eFKOAAAAAAENAAAN+VjmVZl5Rq1ymCq5eFKOAAAAAAEuAAA=" 
            ChangeKey="CQAAABYAAAAN+VjmVZl5Rq1ymCq5eFKOAAAAAADi" />
      </m:ItemIds>
    </m:MarkAsJunk>
  </soap:Body>
</soap:Envelope>
```

次の EWS の SOAP 応答では、正常な応答を示しています。応答内の [MovedItemId](https://msdn.microsoft.com/library/7d5425ab-1e75-43d1-b801-802ff5139df6%28Office.15%29.aspx) 要素には、移動後のアイテムのアイテム ID が含まれます。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="https://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
      <m:ResponseMessages>
        <m:MarkAsJunkResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</m:ResponseCode>
          <m:MovedItemId Id="AAMkADg1OWUwODcyLTg4M2MtNDAyMS05YjI0LTI5ZGM5OTU4Njk3YwBGAAAAAADPriAxh444TpHj2GoQxWQNBwAN+VjmVZl5Rq1ymCq5eFKOAAAAAAEbAAAN+VjmVZl5Rq1ymCq5eFKOAAAE59DIAAA="
              ChangeKey="CQAAABYAAAAN+VjmVZl5Rq1ymCq5eFKOAAAE59E+" />
        </m:MarkAsJunkResponseMessage>
      </m:ResponseMessages>
    </m:MarkAsJunkResponse>
  </s:Body>
</s:Envelope>
```

## <a name="see-also"></a>関連項目

- [Exchange での受信トレイの管理と EWS](inbox-management-and-ews-in-exchange.md)   
- [ExchangeService.MarkAsJunk](https://msdn.microsoft.com/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx)   
- [MarkAsJunk 操作](https://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)   
- [Get-MailboxJunkEmailConfiguration](https://technet.microsoft.com/library/dd979784%28v=exchg.150%29.aspx)   
- [Set-MailboxJunkEmailConfiguration](https://technet.microsoft.com/library/dd979780%28v=exchg.150%29.aspx) 
- [Exchange Management Shell](../management/exchange-management-shell.md)
    

