---
title: 追加し、Exchange の EWS を使用して、[受信拒否リストから電子メール アドレスを削除
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
localization_priority: Normal
ms.assetid: b88288ee-6af7-45b5-a55c-5929cd0c16f1
description: 受信拒否リストに対してメール アドレスを追加および削除するために EWS マネージ API または EWS を使用する方法を説明します。
ms.openlocfilehash: c03ed585ebd62802000179d8c837786ba5f9aab4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19758899"
---
# <a name="add-and-remove-email-addresses-from-the-blocked-senders-list-by-using-ews-in-exchange"></a><span data-ttu-id="e1899-103">追加し、Exchange の EWS を使用して、[受信拒否リストから電子メール アドレスを削除</span><span class="sxs-lookup"><span data-stu-id="e1899-103">Add and remove email addresses from the Blocked Senders List by using EWS in Exchange</span></span>

<span data-ttu-id="e1899-104">受信拒否リストに対してメール アドレスを追加および削除するために EWS マネージ API または EWS を使用する方法を説明します。</span><span class="sxs-lookup"><span data-stu-id="e1899-104">Find out how to use the EWS Managed API or EWS to add email addresses to and remove them from the Blocked Senders List.</span></span>
  
<span data-ttu-id="e1899-p101">ユーザーの [迷惑メール] オプションの [受信拒否リスト] によって、指定した送信者からのすべてのメール メッセージを迷惑メール フォルダーに移動する方法が提供されています。EWS マネージ API または EWS アプリケーションで、受信拒否リストに対してメール アドレスの追加と削除を行えるようにできます。</span><span class="sxs-lookup"><span data-stu-id="e1899-p101">The Blocked Senders List in a user's Junk Email options provides a way to move all email messages from specified senders to the Junk Email folder. You can enable your EWS Managed API or EWS application to add email addresses to or remove them from the Blocked Senders List.</span></span>
  
<span data-ttu-id="e1899-107">電子メール アドレスからのメッセージに電子メール アドレスを追加したり、受信拒否リストから削除する前にユーザーのメールボックスに存在する必要があります注意してください。</span><span class="sxs-lookup"><span data-stu-id="e1899-107">Note that a message from the email address must exist in the user's mailbox before you can add the email address to or remove it from the Blocked Senders List.</span></span> <span data-ttu-id="e1899-108">[ExchangeService.MarkAsJunk](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) EWS のマネージ API のメソッドと[MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)の EWS の操作は、項目 Id のコレクションを使用します。</span><span class="sxs-lookup"><span data-stu-id="e1899-108">The [ExchangeService.MarkAsJunk](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx) EWS Managed API method and the [MarkAsJunk](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx) EWS operation use a collection of item IDs.</span></span> <span data-ttu-id="e1899-109">項目コレクション内の Id は、迷惑メールのステータスを変更する対象のメールボックス内のメッセージを示しています。</span><span class="sxs-lookup"><span data-stu-id="e1899-109">The item IDs in the collection indicate messages in the mailbox for which the junk mail status should be changed.</span></span> 
  
<span data-ttu-id="e1899-110">[Get MailboxJunkEmailConfiguration](http://technet.microsoft.com/en-us/library/dd979784%28v=exchg.150%29.aspx)と[セット MailboxJunkEmailConfiguration](http://technet.microsoft.com/en-us/library/dd979780%28v=exchg.150%29.aspx) Exchange 管理シェル コマンドレットを使用するには [受信拒否リストに直接アクセスします。</span><span class="sxs-lookup"><span data-stu-id="e1899-110">You can use the [Get-MailboxJunkEmailConfiguration](http://technet.microsoft.com/en-us/library/dd979784%28v=exchg.150%29.aspx) and [Set-MailboxJunkEmailConfiguration](http://technet.microsoft.com/en-us/library/dd979780%28v=exchg.150%29.aspx) Exchange Management Shell cmdlets to access the Blocked Senders List directly.</span></span> 
  
## <a name="add-an-email-address-to-or-remove-it-from-the-blocked-senders-list-by-using-the-ews-managed-api"></a><span data-ttu-id="e1899-111">EWS マネージ API を使用して、受信拒否リストに対してメール アドレスを追加または削除します。</span><span class="sxs-lookup"><span data-stu-id="e1899-111">Add an email address to or remove it from the Blocked Senders List by using the EWS Managed API</span></span>
<span data-ttu-id="e1899-112"><a name="bk_AddRemoveEWSMA"> </a></span><span class="sxs-lookup"><span data-stu-id="e1899-112"></span></span>

<span data-ttu-id="e1899-113">電子メール メッセージの送信者を [受信拒否リストに追加するに**MarkAsJunk**メソッドを使用し、**引数 isJunk**パラメーターを**true**に設定します。</span><span class="sxs-lookup"><span data-stu-id="e1899-113">To add the sender of an email message to the Blocked Senders List, use the **MarkAsJunk** method and set the **isJunk** parameter to **true**.</span></span> <span data-ttu-id="e1899-114">電子メール メッセージの送信者を [受信拒否リストから削除するには、 **false を指定**する**引数 isJunk**パラメーターを設定します。</span><span class="sxs-lookup"><span data-stu-id="e1899-114">To remove the sender of an email message from the Blocked Senders List, set the **isJunk** parameter to **false**.</span></span>
  
<span data-ttu-id="e1899-115">次の例では、迷惑メッセージのステータスを変更するのには、 **MarkAsJunk**メソッドを使用する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="e1899-115">The following example shows how to use the **MarkAsJunk** method to change the junk status of a message.</span></span> 
  
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

## <a name="add-an-email-address-to-or-remove-it-from-the-blocked-senders-list-by-using-ews"></a><span data-ttu-id="e1899-116">EWS を使用して、受信拒否リストに対してメール アドレスを追加または削除する</span><span class="sxs-lookup"><span data-stu-id="e1899-116">Add an email address to or remove it from the Blocked Senders List by using EWS</span></span>
<span data-ttu-id="e1899-117"><a name="bk_AddRemoveEWS"> </a></span><span class="sxs-lookup"><span data-stu-id="e1899-117"></span></span>

<span data-ttu-id="e1899-118">次の EWS の SOAP 要求では、 **true を指定**する[MarkAsJunk](http://msdn.microsoft.com/library/f06bafc6-7ee3-4b2b-9fd1-7c51328f4729%28Office.15%29.aspx)要素に**引数 IsJunk**属性を設定することにより迷惑メールとしてアイテムをマークします。</span><span class="sxs-lookup"><span data-stu-id="e1899-118">The following EWS SOAP request marks an item as junk by setting the **IsJunk** attribute on the [MarkAsJunk](http://msdn.microsoft.com/library/f06bafc6-7ee3-4b2b-9fd1-7c51328f4729%28Office.15%29.aspx) element to **true**.</span></span> <span data-ttu-id="e1899-119">移動メッセージ [迷惑メール] フォルダーに**MarkAsJunk**要素を**true**に、 **MoveItem**属性を設定することによってします。</span><span class="sxs-lookup"><span data-stu-id="e1899-119">It also moves the message to the Junk Email folder by setting the **MoveItem** attribute on the **MarkAsJunk** element to **true**.</span></span>
  
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
        <t:ItemId Id="AAMkADg1OWUwODcyLTg4M2MtNDAyMS05YjI0LTI5ZGM5OTU4Njk3YwBGAAAAAADPriAxh444TpHj2GoQxWQNBwAN+VjmVZl5Rq1ymCq5eFKOAAAAAAENAAAN+VjmVZl5Rq1ymCq5eFKOAAAAAAEuAAA=" 
            ChangeKey="CQAAABYAAAAN+VjmVZl5Rq1ymCq5eFKOAAAAAADi" />
      </m:ItemIds>
    </m:MarkAsJunk>
  </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="e1899-120">次の EWS の SOAP 応答には、正常な応答が表示されます。</span><span class="sxs-lookup"><span data-stu-id="e1899-120">The following EWS SOAP response shows the successful response.</span></span> <span data-ttu-id="e1899-121">応答内の[MovedItemId](http://msdn.microsoft.com/library/7d5425ab-1e75-43d1-b801-802ff5139df6%28Office.15%29.aspx)要素には、移動後の項目の項目 ID が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e1899-121">The [MovedItemId](http://msdn.microsoft.com/library/7d5425ab-1e75-43d1-b801-802ff5139df6%28Office.15%29.aspx) element in the response contains the item ID for the item after it was moved.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" MinorVersion="0" MajorBuildNumber="712" MinorBuildNumber="22" Version="V2_3" 
        xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
        xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
        xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <m:MarkAsJunkResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
        xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

## <a name="see-also"></a><span data-ttu-id="e1899-122">関連項目</span><span class="sxs-lookup"><span data-stu-id="e1899-122">See also</span></span>

- [<span data-ttu-id="e1899-123">Exchange での受信トレイの管理と EWS</span><span class="sxs-lookup"><span data-stu-id="e1899-123">Inbox management and EWS in Exchange</span></span>](inbox-management-and-ews-in-exchange.md)   
- [<span data-ttu-id="e1899-124">ExchangeService.MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="e1899-124">ExchangeService.MarkAsJunk</span></span>](http://msdn.microsoft.com/en-us/library/microsoft.exchange.webservices.data.exchangeservice.markasjunk%28v=exchg.80%29.aspx)   
- [<span data-ttu-id="e1899-125">MarkAsJunk の操作</span><span class="sxs-lookup"><span data-stu-id="e1899-125">MarkAsJunk operation</span></span>](http://msdn.microsoft.com/library/1f71f04d-56a9-4fee-a4e7-d1034438329e%28Office.15%29.aspx)   
- [<span data-ttu-id="e1899-126">Get MailboxJunkEmailConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1899-126">Get-MailboxJunkEmailConfiguration</span></span>](http://technet.microsoft.com/en-us/library/dd979784%28v=exchg.150%29.aspx)   
- [<span data-ttu-id="e1899-127">セット MailboxJunkEmailConfiguration</span><span class="sxs-lookup"><span data-stu-id="e1899-127">Set-MailboxJunkEmailConfiguration</span></span>](http://technet.microsoft.com/en-us/library/dd979780%28v=exchg.150%29.aspx) 
- [<span data-ttu-id="e1899-128">Exchange 管理シェル</span><span class="sxs-lookup"><span data-stu-id="e1899-128">Exchange Management Shell</span></span>](../management/exchange-management-shell.md)
    

