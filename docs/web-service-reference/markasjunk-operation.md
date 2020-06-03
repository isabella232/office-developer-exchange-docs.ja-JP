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
ms.lasthandoff: 06/03/2020
ms.locfileid: "44468573"
---
# <a name="markasjunk-operation"></a><span data-ttu-id="e3bb0-103">MarkAsJunk 操作</span><span class="sxs-lookup"><span data-stu-id="e3bb0-103">MarkAsJunk operation</span></span>

<span data-ttu-id="e3bb0-104">**Markasjunk** EWS 操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-104">Find information about the **MarkAsJunk** EWS operation.</span></span> 
  
<span data-ttu-id="e3bb0-105">**Markasjunk**操作は、ブロックされた電子メールリストに対してユーザーを追加および削除し、電子メールメッセージを [迷惑メール] フォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-105">The **MarkAsJunk** operation adds and removes users from the blocked email list and moves email messages to the Junk Email folder.</span></span> 
  
<span data-ttu-id="e3bb0-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-markasjunk-operation"></a><span data-ttu-id="e3bb0-107">MarkAsJunk 操作の使用</span><span class="sxs-lookup"><span data-stu-id="e3bb0-107">Using the MarkAsJunk operation</span></span>

<span data-ttu-id="e3bb0-108">**Markasjunk**操作には、電子メール送信者を受信拒否リストに追加する必要があるかどうか、および対象の電子メールメッセージを既定の迷惑メールフォルダーまたは受信トレイフォルダーに移動する必要があるかどうかを示す2つのブールオプションがあります。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-108">The **MarkAsJunk** operation contains two Boolean options to indicate whether an email sender should be added to the blocked sender list and whether the target email message should be moved to the default Junk Email folder or the Inbox folder.</span></span> <span data-ttu-id="e3bb0-109">アクションは、 **Isjunk メール**属性と**moveitem**属性の値によって決まります。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-109">The actions are determined by the values of the **IsJunk** and **MoveItem** attributes.</span></span> <span data-ttu-id="e3bb0-110">**Isjunk メール**属性と**moveitem**属性の値の組み合わせに基づいて、次の操作を実行できます。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-110">The following are the possible actions based on the value combinations for the **IsJunk** and **MoveItem** attributes:</span></span> 
  
- <span data-ttu-id="e3bb0-111">**Isjunk**属性が**true**に設定されていて、 **moveitem**属性が**true**に設定されている場合、対象の電子メールメッセージの送信者は、受信拒否リストに追加され、電子メールメッセージは迷惑メールフォルダーに移動されます。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-111">If the **IsJunk** attribute is set to **true**, and the **MoveItem** attribute is set to **true**, the sender of the target email message is added to the blocked sender list and the email message is moved to the Junk Dmail folder.</span></span>
    
- <span data-ttu-id="e3bb0-112">**Isjunk**属性が**true**に設定されていて、 **moveitem**属性が**false**に設定されている場合、移動先の電子メールメッセージの送信者は、受信拒否リストに追加され、電子メールメッセージはフォルダーから移動されません。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-112">If the **IsJunk** attribute is set to **true**, and the **MoveItem** attribute is set to **false**, the sender of the target email message is added to the blocked sender list and the email message is not moved from the folder.</span></span>
    
- <span data-ttu-id="e3bb0-113">**Isjunk**属性が**false**に設定されていて、 **moveitem**属性が**true**に設定されている場合、移動先の電子メールメッセージの送信者は、受信拒否リストから削除され、電子メールメッセージは受信トレイフォルダーに移動されます。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-113">If the **IsJunk** attribute is set to **false**, and the **MoveItem** attribute is set to **true**, the sender of the target email messageis removed from the blocked sender list and the email message is moved to the Inbox folder.</span></span>
    
- <span data-ttu-id="e3bb0-114">**Isjunk**属性が**false**に設定されていて、 **moveitem**属性が**false**に設定されている場合、移動先の電子メールメッセージの送信者は、受信拒否リストから削除され、電子メールメッセージはフォルダーから移動されません。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-114">If the **IsJunk** attribute is set to **false**, and the **MoveItem** attribute is set to **false**, the sender of the target email message is removed from the blocked sender list and the email message is not moved from the folder.</span></span>
    
> [!IMPORTANT]
> <span data-ttu-id="e3bb0-115">受信拒否リストの内容は、EWS からは検出できません。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-115">The contents of the blocked sender list are not discoverable from EWS.</span></span> <span data-ttu-id="e3bb0-116">送信者が受信拒否リストに追加されている場合は、ブロックする送信者によって送信された電子メールメッセージのコピーを保持して、送信元のブロックを解除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-116">If a sender is added to the blocked sender list, you need to keep a copy of an email message sent by the blocked sender to unblock the sender in the future.</span></span> 
  
### <a name="markasjunk-operation-soap-headers"></a><span data-ttu-id="e3bb0-117">MarkAsJunk 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3bb0-117">MarkAsJunk operation SOAP headers</span></span>

<span data-ttu-id="e3bb0-118">**Markasjunk**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-118">The **MarkAsJunk** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="e3bb0-119">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="e3bb0-119">**Header name**</span></span>|<span data-ttu-id="e3bb0-120">**要素**</span><span class="sxs-lookup"><span data-stu-id="e3bb0-120">**Element**</span></span>|<span data-ttu-id="e3bb0-121">**説明**</span><span class="sxs-lookup"><span data-stu-id="e3bb0-121">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e3bb0-122">**偽装**</span><span class="sxs-lookup"><span data-stu-id="e3bb0-122">**Impersonation**</span></span> <br/> |[<span data-ttu-id="e3bb0-123">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="e3bb0-123">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="e3bb0-124">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-124">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="e3bb0-125">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e3bb0-126">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="e3bb0-126">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="e3bb0-127">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="e3bb0-127">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="e3bb0-128">RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-128">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="e3bb0-129">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e3bb0-130">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="e3bb0-130">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="e3bb0-131">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="e3bb0-131">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="e3bb0-132">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-132">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="e3bb0-133">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-133">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e3bb0-134">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="e3bb0-134">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="e3bb0-135">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e3bb0-135">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="e3bb0-136">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-136">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="e3bb0-137">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-137">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="markasjunk-operation-request-example-add-a-sender-to-the-blocked-sender-list"></a><span data-ttu-id="e3bb0-138">MarkAsJunk 操作要求の例: 送信者を受信拒否リストに追加します。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-138">MarkAsJunk operation request example: Add a sender to the blocked sender list</span></span>

<span data-ttu-id="e3bb0-139">次の例は、 **Markasjunk**操作要求の例で、電子メールの送信者を受信拒否リストに追加し、その電子メールを迷惑メールフォルダーに移動する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-139">The following example of a **MarkAsJunk** operation request shows how to add the sender of an email to the blocked sender list and move the email to the junk mail folder.</span></span> <span data-ttu-id="e3bb0-140">**Markasjunk**操作は、受信拒否リストに追加された送信者を参照するために使用される電子メールを識別する一意の電子メールメッセージ識別子を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-140">The **MarkAsJunk** operation accepts the unique email message identifier to identify the email that is used to reference the sender that is added to the blocked sender list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e3bb0-141">この記事のすべてのアイテム識別子と変更キーは、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-141">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
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

<span data-ttu-id="e3bb0-142">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-142">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e3bb0-143">MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="e3bb0-143">MarkAsJunk</span></span>](markasjunk.md)
    
- [<span data-ttu-id="e3bb0-144">ItemIds</span><span class="sxs-lookup"><span data-stu-id="e3bb0-144">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="e3bb0-145">ItemId</span><span class="sxs-lookup"><span data-stu-id="e3bb0-145">ItemId</span></span>](itemid.md)
    
## <a name="successful-markasjunk-operation-response"></a><span data-ttu-id="e3bb0-146">正常な MarkAsJunk 操作の応答</span><span class="sxs-lookup"><span data-stu-id="e3bb0-146">Successful MarkAsJunk operation response</span></span>

<span data-ttu-id="e3bb0-147">次の例は、[ブロックする差出人のリスト] に送信者を追加し、その電子メールメッセージを迷惑メールフォルダーに移動するための、 **Markasjunk**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-147">The following example shows a successful response to a **MarkAsJunk** operation request to add a sender to the blocked sender list and move the email message to the Junk Email folder.</span></span> 
  
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

<span data-ttu-id="e3bb0-148">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-148">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e3bb0-149">MarkAsJunkResponse</span><span class="sxs-lookup"><span data-stu-id="e3bb0-149">MarkAsJunkResponse</span></span>](markasjunkresponse.md)
    
- [<span data-ttu-id="e3bb0-150">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e3bb0-150">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e3bb0-151">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e3bb0-151">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
    
- [<span data-ttu-id="e3bb0-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e3bb0-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e3bb0-153">MovedItemId</span><span class="sxs-lookup"><span data-stu-id="e3bb0-153">MovedItemId</span></span>](moveditemid.md)
    
## <a name="markasjunk-operation-request-example-remove-a-sender-from-the-blocked-sender-list"></a><span data-ttu-id="e3bb0-154">MarkAsJunk 操作要求の例: 受信拒否リストから送信者を削除します</span><span class="sxs-lookup"><span data-stu-id="e3bb0-154">MarkAsJunk operation request example: Remove a sender from the blocked sender list</span></span>

<span data-ttu-id="e3bb0-155">次の例は、 **Markasjunk**操作要求の例で、電子メールメッセージの送信者を受信拒否リストから削除し、その電子メールメッセージを受信トレイフォルダーに移動する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-155">The following example of a **MarkAsJunk** operation request shows how to remove the sender of an email message from the blocked sender list and move the email message to the Inbox folder.</span></span> <span data-ttu-id="e3bb0-156">受信拒否リストから送信者を削除するには、ブロックする送信者によって送信される電子メールメッセージを保持する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-156">You need to keep an email message sent by the blocked sender to remove the sender from the blocked sender list.</span></span> <span data-ttu-id="e3bb0-157">送信者の電子メールアドレスは、送信者によって送信された電子メールメッセージに関連付けられています。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-157">The sender's email address is associated with email messages that have been sent by the sender.</span></span> <span data-ttu-id="e3bb0-158">参照電子メールメッセージがユーザーのメールボックスに存在しなくなった場合、受信拒否リストからの送信者の削除は成功しません。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-158">Removing a sender from the blocked sender list will not succeed if the reference email message no longer exists in the user's mailbox.</span></span> <span data-ttu-id="e3bb0-159">送信者に電子メールメッセージを関連付けるために使用されるアイテム識別子は、Exchange メールボックス内に存在するアイテムに関連付けられている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-159">The item identifier used to associate an email message with its sender must be associated with an item that exists in the Exchange mailbox.</span></span> <span data-ttu-id="e3bb0-160">以前にブロックされた送信者が送信したアイテムを格納するための非表示のフォルダーを作成して、クライアントアプリケーションからの送信者のブロックを解除できるようにすることをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-160">We recommend that you create a hidden folder to store items sent by previously blocked senders so that the senders can be unblocked from the client application.</span></span> <span data-ttu-id="e3bb0-161">Exchange メールボックスからアイテムが削除された場合は、管理者が Exchange 管理コンソールを使用して、受信拒否リストにアクセスして送信者を一覧から削除する必要があります。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-161">In the event that an item has been removed from the Exchange mailbox, an administrator has to use the Exchange Management Console to access the blocked sender list to remove a sender from the list.</span></span> <span data-ttu-id="e3bb0-162">Exchange 管理コンソールを使用してユーザーのブロックを解除する方法については、「 [Office 365 で差出人セーフリストと受信拒否設定を構成する方法](https://support.microsoft.com/kb/2545137)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-162">For information about how to unblock a user by using the Exchange Management Console, see [How to configure the safe senders and blocked senders settings in Office 365](https://support.microsoft.com/kb/2545137).</span></span>
  
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

<span data-ttu-id="e3bb0-163">受信拒否リストから送信者を削除するための正常な応答は、受信拒否リストに送信者を追加する際の応答と同じです。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-163">A successful response for removing a sender from the blocked sender list is the same as the response for adding a sender to the blocked sender list.</span></span>
  
<span data-ttu-id="e3bb0-164">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-164">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e3bb0-165">MarkAsJunk</span><span class="sxs-lookup"><span data-stu-id="e3bb0-165">MarkAsJunk</span></span>](markasjunk.md)
    
- [<span data-ttu-id="e3bb0-166">ItemIds</span><span class="sxs-lookup"><span data-stu-id="e3bb0-166">ItemIds</span></span>](itemids.md)
    
- [<span data-ttu-id="e3bb0-167">ItemId</span><span class="sxs-lookup"><span data-stu-id="e3bb0-167">ItemId</span></span>](itemid.md)
    
## <a name="markasjunk-operation-error-response"></a><span data-ttu-id="e3bb0-168">MarkAsJunk 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="e3bb0-168">MarkAsJunk operation error response</span></span>

<span data-ttu-id="e3bb0-169">次の例は、 **Markasjunk**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-169">The following example shows an error response to a **MarkAsJunk** operation request.</span></span> <span data-ttu-id="e3bb0-170">これは、アイテム識別子によって指定された電子メールメッセージがメールボックスに存在しなくなったときに、受信拒否リストに送信者を追加または削除する要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-170">This is a response to a request to add or remove a sender from the blocked sender list when the email message specified by the item identifier no longer exists in the mailbox.</span></span> 
  
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

<span data-ttu-id="e3bb0-171">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e3bb0-171">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e3bb0-172">MarkAsJunkResponse</span><span class="sxs-lookup"><span data-stu-id="e3bb0-172">MarkAsJunkResponse</span></span>](markasjunkresponse.md)
    
- [<span data-ttu-id="e3bb0-173">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e3bb0-173">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e3bb0-174">MarkAsJunkResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e3bb0-174">MarkAsJunkResponseMessage</span></span>](markasjunkresponsemessage.md)
    
- [<span data-ttu-id="e3bb0-175">MessageText</span><span class="sxs-lookup"><span data-stu-id="e3bb0-175">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="e3bb0-176">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e3bb0-176">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e3bb0-177">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e3bb0-177">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="e3bb0-178">関連項目</span><span class="sxs-lookup"><span data-stu-id="e3bb0-178">See also</span></span>

- [<span data-ttu-id="e3bb0-179">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="e3bb0-179">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- <span data-ttu-id="e3bb0-180">[GetItem 操作](getitem-operation.md)GetItem 操作</span><span class="sxs-lookup"><span data-stu-id="e3bb0-180">[GetItem operation](getitem-operation.md) GetItem operation</span></span> 
    
- [<span data-ttu-id="e3bb0-181">FindItem 操作</span><span class="sxs-lookup"><span data-stu-id="e3bb0-181">FindItem operation</span></span>](finditem-operation.md)
    

