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
# <a name="markasjunk-operation"></a><span data-ttu-id="221fe-103">MarkAsJunk の操作</span><span class="sxs-lookup"><span data-stu-id="221fe-103">MarkAsJunk operation</span></span>

<span data-ttu-id="221fe-104">**MarkAsJunk** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="221fe-104">Find information about the **MarkAsJunk** EWS operation.</span></span> 
  
<span data-ttu-id="221fe-105">**MarkAsJunk**操作は、追加しブロックされた電子メール] ボックスの一覧からユーザーを削除し、電子メール メッセージを [迷惑メール フォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="221fe-105">The **MarkAsJunk** operation adds and removes users from the blocked email list and moves email messages to the Junk Email folder.</span></span> 
  
<span data-ttu-id="221fe-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="221fe-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-markasjunk-operation"></a><span data-ttu-id="221fe-107">MarkAsJunk 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="221fe-107">Using the MarkAsJunk operation</span></span>

<span data-ttu-id="221fe-108">**MarkAsJunk**操作には、受信拒否リストに、電子メールの送信者を追加するか、移行先の電子メール メッセージを既定の [迷惑メール] フォルダーまたは [受信トレイ] フォルダーに移動するかどうかを示すために 2 つのブール型のオプションが含まれています。</span><span class="sxs-lookup"><span data-stu-id="221fe-108">The **MarkAsJunk** operation contains two Boolean options to indicate whether an email sender should be added to the blocked sender list and whether the target email message should be moved to the default Junk Email folder or the Inbox folder.</span></span> <span data-ttu-id="221fe-109">アクションは、**引数 IsJunk**と**MoveItem**属性の値によって決まります。</span><span class="sxs-lookup"><span data-stu-id="221fe-109">The actions are determined by the values of the **IsJunk** and **MoveItem** attributes.</span></span> <span data-ttu-id="221fe-110">**引数 IsJunk**と**MoveItem**属性の値の組み合わせに基づいて使用可能なアクションは、次のように。</span><span class="sxs-lookup"><span data-stu-id="221fe-110">The following are the possible actions based on the value combinations for the **IsJunk** and **MoveItem** attributes:</span></span> 
  
- <span data-ttu-id="221fe-111">**引数 IsJunk**属性が**true**に設定すると、 **MoveItem**属性が**true**に設定、ターゲットの電子メール メッセージの送信者がブロックされる送信者の一覧に追加し、Dmail を迷惑メール フォルダーに電子メール メッセージを移動します。</span><span class="sxs-lookup"><span data-stu-id="221fe-111">If the **IsJunk** attribute is set to **true**, and the **MoveItem** attribute is set to **true**, the sender of the target email message is added to the blocked sender list and the email message is moved to the Junk Dmail folder.</span></span>
    
- <span data-ttu-id="221fe-112">**引数 IsJunk**属性が**true**に設定すると、 **MoveItem**属性が**false**に設定、ターゲットの電子メール メッセージの送信者がブロックされる送信者の一覧に追加し、フォルダーから電子メール メッセージが移動しません。</span><span class="sxs-lookup"><span data-stu-id="221fe-112">If the **IsJunk** attribute is set to **true**, and the **MoveItem** attribute is set to **false**, the sender of the target email message is added to the blocked sender list and the email message is not moved from the folder.</span></span>
    
- <span data-ttu-id="221fe-113">**引数 IsJunk**属性が設定されている場合**は true**、ブロックする送信者の一覧から削除対象の電子メール ティーの送信者に**false を指定**し、 **MoveItem**属性が設定されてし、電子メール メッセージは [受信トレイ] フォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="221fe-113">If the **IsJunk** attribute is set to **false**, and the **MoveItem** attribute is set to **true**, the sender of the target email messageis removed from the blocked sender list and the email message is moved to the Inbox folder.</span></span>
    
- <span data-ttu-id="221fe-114">**引数 IsJunk**属性が**false**に設定されて場合は、 **MoveItem**属性が**false**に設定対象の電子メール メッセージの送信者がブロックされる送信者の一覧から削除し、フォルダーから電子メール メッセージが移動しません。</span><span class="sxs-lookup"><span data-stu-id="221fe-114">If the **IsJunk** attribute is set to **false**, and the **MoveItem** attribute is set to **false**, the sender of the target email message is removed from the blocked sender list and the email message is not moved from the folder.</span></span>
    
> [!IMPORTANT]
> <span data-ttu-id="221fe-115">受信拒否リストの内容は、EWS から検出可能ではありません。</span><span class="sxs-lookup"><span data-stu-id="221fe-115">The contents of the blocked sender list are not discoverable from EWS.</span></span> <span data-ttu-id="221fe-116">受信拒否リストに送信者を追加する場合、将来的に、送信者のブロックを解除するのには、ブロックされている送信者から送信された電子メール メッセージのコピーを保持する必要があります。</span><span class="sxs-lookup"><span data-stu-id="221fe-116">If a sender is added to the blocked sender list, you need to keep a copy of an email message sent by the blocked sender to unblock the sender in the future.</span></span> 
  
### <a name="markasjunk-operation-soap-headers"></a><span data-ttu-id="221fe-117">MarkAsJunk 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="221fe-117">MarkAsJunk operation SOAP headers</span></span>

<span data-ttu-id="221fe-118">**MarkAsJunk**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="221fe-118">The **MarkAsJunk** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="221fe-119">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="221fe-119">**Header name**</span></span>|<span data-ttu-id="221fe-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="221fe-120">**Element**</span></span>|<span data-ttu-id="221fe-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="221fe-121">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="221fe-122">**偽装**</span><span class="sxs-lookup"><span data-stu-id="221fe-122">**Impersonation**</span></span> <br/> |[<span data-ttu-id="221fe-123">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="221fe-123">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="221fe-124">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="221fe-124">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="221fe-125">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="221fe-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="221fe-126">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="221fe-126">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="221fe-127">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="221fe-127">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="221fe-128">RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="221fe-128">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="221fe-129">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="221fe-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="221fe-130">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="221fe-130">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="221fe-131">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="221fe-131">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="221fe-132">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="221fe-132">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="221fe-133">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="221fe-133">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="221fe-134">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="221fe-134">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="221fe-135">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="221fe-135">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="221fe-136">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="221fe-136">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="221fe-137">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="221fe-137">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="markasjunk-operation-request-example-add-a-sender-to-the-blocked-sender-list"></a><span data-ttu-id="221fe-138">MarkAsJunk 操作の要求の使用例: 受信拒否リストに送信者を追加</span><span class="sxs-lookup"><span data-stu-id="221fe-138">MarkAsJunk operation request example: Add a sender to the blocked sender list</span></span>

<span data-ttu-id="221fe-139">**MarkAsJunk**操作要求の次の例では、電子メールの送信者を受信拒否リストに追加し、[迷惑メール] フォルダーに電子メールを移動する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="221fe-139">The following example of a **MarkAsJunk** operation request shows how to add the sender of an email to the blocked sender list and move the email to the junk mail folder.</span></span> <span data-ttu-id="221fe-140">**MarkAsJunk**操作では、送信者が受信拒否リストに追加するを参照するために使用される電子メールを識別する一意の電子メール メッセージの id を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="221fe-140">The **MarkAsJunk** operation accepts the unique email message identifier to identify the email that is used to reference the sender that is added to the blocked sender list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="221fe-141">すべての項目の識別子と変更キーをこの資料では、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="221fe-141">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
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

<span data-ttu-id="221fe-142">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="221fe-142">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="221fe-143">MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="221fe-143">MarkAsJunk</span></span>](markasjunk.md)
    
- [<span data-ttu-id="221fe-144">Itemid</span><span class="sxs-lookup"><span data-stu-id="221fe-144">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="221fe-145">ItemId</span><span class="sxs-lookup"><span data-stu-id="221fe-145">ItemId</span></span>](itemid.md)
    
## <a name="successful-markasjunk-operation-response"></a><span data-ttu-id="221fe-146">MarkAsJunk 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="221fe-146">Successful MarkAsJunk operation response</span></span>

<span data-ttu-id="221fe-147">次の例では、受信拒否リストに送信者を追加し、電子メール メッセージを [迷惑メール フォルダーに移動する**MarkAsJunk**操作要求に正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="221fe-147">The following example shows a successful response to a **MarkAsJunk** operation request to add a sender to the blocked sender list and move the email message to the Junk Email folder.</span></span> 
  
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

<span data-ttu-id="221fe-148">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="221fe-148">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="221fe-149">MarkAsJunkResponse</span><span class="sxs-lookup"><span data-stu-id="221fe-149">MarkAsJunkResponse</span></span>](markasjunkresponse.md)
    
- [<span data-ttu-id="221fe-150">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="221fe-150">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="221fe-151">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="221fe-151">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
    
- [<span data-ttu-id="221fe-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="221fe-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="221fe-153">MovedItemId</span><span class="sxs-lookup"><span data-stu-id="221fe-153">MovedItemId</span></span>](moveditemid.md)
    
## <a name="markasjunk-operation-request-example-remove-a-sender-from-the-blocked-sender-list"></a><span data-ttu-id="221fe-154">MarkAsJunk 操作の要求の例: ブロックされた送信者の一覧から送信者を削除します。</span><span class="sxs-lookup"><span data-stu-id="221fe-154">MarkAsJunk operation request example: Remove a sender from the blocked sender list</span></span>

<span data-ttu-id="221fe-155">**MarkAsJunk**操作要求の次の例では、電子メール メッセージの送信者を受信拒否リストから削除し、電子メール メッセージを受信トレイ フォルダーに移動する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="221fe-155">The following example of a **MarkAsJunk** operation request shows how to remove the sender of an email message from the blocked sender list and move the email message to the Inbox folder.</span></span> <span data-ttu-id="221fe-156">禁止された送信者の一覧から送信者を削除するのには、ブロックされている送信者から送信された電子メール メッセージを保持する必要があります。</span><span class="sxs-lookup"><span data-stu-id="221fe-156">You need to keep an email message sent by the blocked sender to remove the sender from the blocked sender list.</span></span> <span data-ttu-id="221fe-157">送信者の電子メール アドレスは、送信者によって送信された電子メール メッセージに関連付けられます。</span><span class="sxs-lookup"><span data-stu-id="221fe-157">The sender's email address is associated with email messages that have been sent by the sender.</span></span> <span data-ttu-id="221fe-158">禁止された送信者の一覧から送信者を削除することも、参照の電子メール メッセージがユーザーのメールボックスに存在しない場合は失敗します。</span><span class="sxs-lookup"><span data-stu-id="221fe-158">Removing a sender from the blocked sender list will not succeed if the reference email message no longer exists in the user's mailbox.</span></span> <span data-ttu-id="221fe-159">項目 id、送信者の電子メール メッセージを関連付けるために使用は、Exchange のメールボックスに存在する項目に関連付けられているである必要があります。</span><span class="sxs-lookup"><span data-stu-id="221fe-159">The item identifier used to associate an email message with its sender must be associated with an item that exists in the Exchange mailbox.</span></span> <span data-ttu-id="221fe-160">送信者がクライアント アプリケーションから受信できるようにするために、以前にブロックされた送信者によって送信されたアイテムを格納する非表示のフォルダーを作成することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="221fe-160">We recommend that you create a hidden folder to store items sent by previously blocked senders so that the senders can be unblocked from the client application.</span></span> <span data-ttu-id="221fe-161">イベントで Exchange メールボックスから項目を削除すると、管理者は Exchange 管理コンソールのを使用して、一覧から送信者を削除するのにはブロックされている送信者リストにアクセスするには。</span><span class="sxs-lookup"><span data-stu-id="221fe-161">In the event that an item has been removed from the Exchange mailbox, an administrator has to use the Exchange Management Console to access the blocked sender list to remove a sender from the list.</span></span> <span data-ttu-id="221fe-162">Exchange 管理コンソールのを使用してユーザーのブロックを解除する方法の詳細については、 [[差出人セーフ リストおよび受信拒否の設定で Office 365 を構成する方法](http://support.microsoft.com/kb/2545137)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="221fe-162">For information about how to unblock a user by using the Exchange Management Console, see [How to configure the safe senders and blocked senders settings in Office 365](http://support.microsoft.com/kb/2545137).</span></span>
  
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

<span data-ttu-id="221fe-163">禁止された送信者の一覧から送信者を削除するための正常な応答は、受信拒否リストに送信者を追加するための反応と同じです。</span><span class="sxs-lookup"><span data-stu-id="221fe-163">A successful response for removing a sender from the blocked sender list is the same as the response for adding a sender to the blocked sender list.</span></span>
  
<span data-ttu-id="221fe-164">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="221fe-164">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="221fe-165">MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="221fe-165">MarkAsJunk</span></span>](markasjunk.md)
    
- [<span data-ttu-id="221fe-166">Itemid</span><span class="sxs-lookup"><span data-stu-id="221fe-166">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="221fe-167">ItemId</span><span class="sxs-lookup"><span data-stu-id="221fe-167">ItemId</span></span>](itemid.md)
    
## <a name="markasjunk-operation-error-response"></a><span data-ttu-id="221fe-168">MarkAsJunk 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="221fe-168">MarkAsJunk operation error response</span></span>

<span data-ttu-id="221fe-169">**MarkAsJunk**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="221fe-169">The following example shows an error response to a **MarkAsJunk** operation request.</span></span> <span data-ttu-id="221fe-170">これは、追加または項目の識別子で指定された電子メール メッセージがメールボックスに存在しない場合、ブロックする送信者の一覧から送信者を削除する要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="221fe-170">This is a response to a request to add or remove a sender from the blocked sender list when the email message specified by the item identifier no longer exists in the mailbox.</span></span> 
  
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

<span data-ttu-id="221fe-171">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="221fe-171">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="221fe-172">MarkAsJunkResponse</span><span class="sxs-lookup"><span data-stu-id="221fe-172">MarkAsJunkResponse</span></span>](markasjunkresponse.md)
    
- [<span data-ttu-id="221fe-173">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="221fe-173">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="221fe-174">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="221fe-174">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
    
- [<span data-ttu-id="221fe-175">MessageText</span><span class="sxs-lookup"><span data-stu-id="221fe-175">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="221fe-176">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="221fe-176">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="221fe-177">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="221fe-177">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="221fe-178">関連項目</span><span class="sxs-lookup"><span data-stu-id="221fe-178">See also</span></span>

- [<span data-ttu-id="221fe-179">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="221fe-179">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- <span data-ttu-id="221fe-180">[GetItem 操作](getitem-operation.md)GetItem 操作</span><span class="sxs-lookup"><span data-stu-id="221fe-180">[GetItem operation](getitem-operation.md) GetItem operation</span></span> 
    
- <span data-ttu-id="221fe-181">
  [FindItem 操作](finditem-operation.md)</span><span class="sxs-lookup"><span data-stu-id="221fe-181">[FindItem operation](finditem-operation.md)</span></span>
    

