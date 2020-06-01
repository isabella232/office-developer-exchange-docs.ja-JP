---
title: RemoveContactFromImList 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: RemoveContactFromImList EWS 操作についての情報を検索します。
ms.openlocfilehash: 8b3d83a0b53bad169d9f3478540e5087901f3a12
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458468"
---
# <a name="removecontactfromimlist-operation"></a><span data-ttu-id="70fa1-103">RemoveContactFromImList 操作</span><span class="sxs-lookup"><span data-stu-id="70fa1-103">RemoveContactFromImList operation</span></span>

<span data-ttu-id="70fa1-104">**RemoveContactFromImList** EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="70fa1-104">Find information about the **RemoveContactFromImList** EWS operation.</span></span> 
  
<span data-ttu-id="70fa1-105">**RemoveContactFromImList**操作は、lync が連絡先ストアに対して Exchange を使用している場合に、lync インスタントメッセージング (IM) リストから連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="70fa1-105">The **RemoveContactFromImList** operation removes contacts from the Lync instant messaging (IM) list when Lync uses Exchange for the contact store.</span></span> 
  
<span data-ttu-id="70fa1-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="70fa1-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removecontactfromimlist-operation"></a><span data-ttu-id="70fa1-107">RemoveContactFromImList 操作の使用</span><span class="sxs-lookup"><span data-stu-id="70fa1-107">Using the RemoveContactFromImList operation</span></span>

<span data-ttu-id="70fa1-108">**RemoveContactFromImList**操作は、Exchange サーバーに格納されている Lync 連絡先リストから削除する連絡先を識別する1つの引数を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="70fa1-108">The **RemoveContactFromImList** operation accepts a single argument that identifies a contact to remove from the Lync contact list stored on an Exchange server.</span></span> <span data-ttu-id="70fa1-109">この操作対象の連絡先の一覧は、Outlook 2013 では**Lync 連絡先**と呼ばれます。</span><span class="sxs-lookup"><span data-stu-id="70fa1-109">The list of contacts that this operation targets is called **Lync Contacts** in Outlook 2013.</span></span> 
  
> [!CAUTION]
> <span data-ttu-id="70fa1-110">連絡先リストから連絡先を削除する場合は、 [DeleteItem 操作](deleteitem-operation.md)を使用しないでください。</span><span class="sxs-lookup"><span data-stu-id="70fa1-110">Do not use the [DeleteItem operation](deleteitem-operation.md) to remove contacts from a contact list.</span></span> <span data-ttu-id="70fa1-111">**Lync 連絡先**リストから連絡先を削除できるようにするには、追加のサーバー側処理が必要になることがあります。</span><span class="sxs-lookup"><span data-stu-id="70fa1-111">Additional server-side processing might have to occur to support removing a contact from the **Lync Contacts** list.</span></span> <span data-ttu-id="70fa1-112">**Lync 連絡先**リストは、既定の**lync 連絡先**メールボックスフォルダーに相当する概念であることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="70fa1-112">Note that the **Lync Contacts** list is the conceptual equivalent of the default **Lync Contacts** mailbox folder.</span></span> 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a><span data-ttu-id="70fa1-113">RemoveContactFromImList 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="70fa1-113">RemoveContactFromImList operation SOAP headers</span></span>

<span data-ttu-id="70fa1-114">**RemoveContactFromImList**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="70fa1-114">The **RemoveContactFromImList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="70fa1-115">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="70fa1-115">**Header name**</span></span>|<span data-ttu-id="70fa1-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="70fa1-116">**Element**</span></span>|<span data-ttu-id="70fa1-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="70fa1-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="70fa1-118">**偽装**</span><span class="sxs-lookup"><span data-stu-id="70fa1-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="70fa1-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="70fa1-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="70fa1-120">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="70fa1-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="70fa1-121">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="70fa1-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="70fa1-122">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="70fa1-122">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="70fa1-123">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="70fa1-123">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="70fa1-124">RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。</span><span class="sxs-lookup"><span data-stu-id="70fa1-124">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="70fa1-125">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="70fa1-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="70fa1-126">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="70fa1-126">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="70fa1-127">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="70fa1-127">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="70fa1-128">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="70fa1-128">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="70fa1-129">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="70fa1-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="70fa1-130">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="70fa1-130">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="70fa1-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="70fa1-131">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="70fa1-132">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="70fa1-132">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="70fa1-133">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="70fa1-133">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a><span data-ttu-id="70fa1-134">RemoveContactFromImList 操作要求の例: Lync 連絡先リストから連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="70fa1-134">RemoveContactFromImList operation request example: Remove a contact from the Lync Contacts list</span></span>

<span data-ttu-id="70fa1-135">次の**RemoveContactFromImList**操作要求の例は、 **Lync 連絡先**リストから連絡先を削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="70fa1-135">The following example of a **RemoveContactFromImList** operation request shows how to remove a contact from the **Lync Contacts** list.</span></span> <span data-ttu-id="70fa1-136">**RemoveContactFromImList**操作は、 **Lync の連絡先**リストから削除された連絡先を識別するための一意の連絡先識別子を1つだけ受け入れます。</span><span class="sxs-lookup"><span data-stu-id="70fa1-136">The **RemoveContactFromImList** operation accepts a single unique contact identifier to identify the contact that is removed from the **Lync Contacts** list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="70fa1-137">この記事のすべてのアイテム識別子と変更キーは、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="70fa1-137">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
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
      <m:RemoveContactFromImList>
         <m:ContactId Id=""/>
      </m:RemoveContactFromImList>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="70fa1-138">要求 SOAP 本文では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="70fa1-138">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="70fa1-139">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="70fa1-139">RemoveContactFromImList</span></span>](removecontactfromimlist.md)
    
- [<span data-ttu-id="70fa1-140">ContactId</span><span class="sxs-lookup"><span data-stu-id="70fa1-140">ContactId</span></span>](contactid.md)
    
## <a name="successful-removecontactfromimlist-operation-response"></a><span data-ttu-id="70fa1-141">成功した RemoveContactFromImList 操作の応答</span><span class="sxs-lookup"><span data-stu-id="70fa1-141">Successful RemoveContactFromImList operation response</span></span>

<span data-ttu-id="70fa1-142">次の例は、 **RemoveContactFromImList**操作要求に対する正常な応答を示しています。これは、 **Lync 連絡先**リストから連絡先を削除することです。</span><span class="sxs-lookup"><span data-stu-id="70fa1-142">The following example shows a successful response to a **RemoveContactFromImList** operation request to remove a contact from the **Lync Contacts** list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Success" 
                                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="70fa1-143">応答 SOAP 本文では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="70fa1-143">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="70fa1-144">RemoveContactFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="70fa1-144">RemoveContactFromImListResponse</span></span>](removecontactfromimlistresponse.md)
    
- [<span data-ttu-id="70fa1-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="70fa1-145">ResponseCode</span></span>](responsecode.md)
    
## <a name="removecontactfromimlist-operation-error-response"></a><span data-ttu-id="70fa1-146">RemoveContactFromImList 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="70fa1-146">RemoveContactFromImList operation error response</span></span>

<span data-ttu-id="70fa1-147">次の例は、 **RemoveContactFromImList**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="70fa1-147">The following example shows an error response to a **RemoveContactFromImList** operation request.</span></span> <span data-ttu-id="70fa1-148">これは、連絡先がリストに存在しなくなったときに、 **Lync の連絡先**リストから連絡先を削除する要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="70fa1-148">This is a response to a request to remove a contact from the **Lync Contacts** list when the contact no longer exists in the list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Error" 
                                       xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="70fa1-149">エラー応答 SOAP 本文では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="70fa1-149">The following elements are used in the error response SOAP body:</span></span>
  
- [<span data-ttu-id="70fa1-150">RemoveContactFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="70fa1-150">RemoveContactFromImListResponse</span></span>](removecontactfromimlistresponse.md)
    
- [<span data-ttu-id="70fa1-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="70fa1-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="70fa1-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="70fa1-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="70fa1-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="70fa1-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="70fa1-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="70fa1-154">See also</span></span>

- [<span data-ttu-id="70fa1-155">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="70fa1-155">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="70fa1-156">GetImItemList 操作</span><span class="sxs-lookup"><span data-stu-id="70fa1-156">GetImItemList operation</span></span>](getimitemlist-operation.md)
    

