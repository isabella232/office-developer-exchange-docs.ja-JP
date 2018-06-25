---
title: RemoveContactFromImList 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 28ec96c3-45af-48ff-9f17-718a527dc0ad
description: 操作 RemoveContactFromImList EWS についての情報を検索します。
ms.openlocfilehash: 036b295a84e86ad74c467572cc52fdf6bbae5191
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833080"
---
# <a name="removecontactfromimlist-operation"></a><span data-ttu-id="098ca-103">RemoveContactFromImList 操作</span><span class="sxs-lookup"><span data-stu-id="098ca-103">RemoveContactFromImList operation</span></span>

<span data-ttu-id="098ca-104">**RemoveContactFromImList** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="098ca-104">Find information about the **RemoveContactFromImList** EWS operation.</span></span> 
  
<span data-ttu-id="098ca-105">**RemoveContactFromImList**操作は、Lync は、連絡先ストアの Exchange を使用すると、Lync のインスタント メッセージング (IM) の一覧から連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="098ca-105">The **RemoveContactFromImList** operation removes contacts from the Lync instant messaging (IM) list when Lync uses Exchange for the contact store.</span></span> 
  
<span data-ttu-id="098ca-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="098ca-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removecontactfromimlist-operation"></a><span data-ttu-id="098ca-107">RemoveContactFromImList 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="098ca-107">Using the RemoveContactFromImList operation</span></span>

<span data-ttu-id="098ca-108">**RemoveContactFromImList**操作は、Exchange サーバーに格納されている Lync 連絡先リストから削除するメンバーを識別する 1 つの引数を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="098ca-108">The **RemoveContactFromImList** operation accepts a single argument that identifies a contact to remove from the Lync contact list stored on an Exchange server.</span></span> <span data-ttu-id="098ca-109">この操作のターゲットがという名前の**Lync 連絡先**Outlook 2013 で連絡先の一覧です。</span><span class="sxs-lookup"><span data-stu-id="098ca-109">The list of contacts that this operation targets is called **Lync Contacts** in Outlook 2013.</span></span> 
  
> [!CAUTION]
> <span data-ttu-id="098ca-110">連絡先リストから連絡先を削除するのには、 [DeleteItem の操作](deleteitem-operation.md)を使用しません。</span><span class="sxs-lookup"><span data-stu-id="098ca-110">Do not use the [DeleteItem operation](deleteitem-operation.md) to remove contacts from a contact list.</span></span> <span data-ttu-id="098ca-111">追加のサーバー側の処理では、 **Lync の連絡先**リストから連絡先を削除することをサポートするために発生する必要があります。</span><span class="sxs-lookup"><span data-stu-id="098ca-111">Additional server-side processing might have to occur to support removing a contact from the **Lync Contacts** list.</span></span> <span data-ttu-id="098ca-112">**Lync の連絡先**の一覧は、既定の**Lync の連絡先**のメールボックス フォルダーの概念と同じであることを注意してください。</span><span class="sxs-lookup"><span data-stu-id="098ca-112">Note that the **Lync Contacts** list is the conceptual equivalent of the default **Lync Contacts** mailbox folder.</span></span> 
  
### <a name="removecontactfromimlist-operation-soap-headers"></a><span data-ttu-id="098ca-113">RemoveContactFromImList 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="098ca-113">RemoveContactFromImList operation SOAP headers</span></span>

<span data-ttu-id="098ca-114">**RemoveContactFromImList**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="098ca-114">The **RemoveContactFromImList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="098ca-115">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="098ca-115">**Header name**</span></span>|<span data-ttu-id="098ca-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="098ca-116">**Element**</span></span>|<span data-ttu-id="098ca-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="098ca-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="098ca-118">**偽装**</span><span class="sxs-lookup"><span data-stu-id="098ca-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="098ca-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="098ca-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="098ca-120">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="098ca-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="098ca-121">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="098ca-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="098ca-122">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="098ca-122">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="098ca-123">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="098ca-123">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="098ca-124">RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="098ca-124">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="098ca-125">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="098ca-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="098ca-126">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="098ca-126">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="098ca-127">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="098ca-127">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="098ca-128">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="098ca-128">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="098ca-129">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="098ca-129">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="098ca-130">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="098ca-130">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="098ca-131">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="098ca-131">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="098ca-132">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="098ca-132">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="098ca-133">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="098ca-133">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removecontactfromimlist-operation-request-example-remove-a-contact-from-the-lync-contacts-list"></a><span data-ttu-id="098ca-134">RemoveContactFromImList 操作の要求の例: Lync の連絡先リストから連絡先を削除します。</span><span class="sxs-lookup"><span data-stu-id="098ca-134">RemoveContactFromImList operation request example: Remove a contact from the Lync Contacts list</span></span>

<span data-ttu-id="098ca-135">**RemoveContactFromImList**操作要求の次の例では、 **Lync の連絡先**リストから連絡先を削除する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="098ca-135">The following example of a **RemoveContactFromImList** operation request shows how to remove a contact from the **Lync Contacts** list.</span></span> <span data-ttu-id="098ca-136">**RemoveContactFromImList**操作では、 **Lync の連絡先**の一覧から削除された連絡先を識別する 1 つ固有連絡先 id を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="098ca-136">The **RemoveContactFromImList** operation accepts a single unique contact identifier to identify the contact that is removed from the **Lync Contacts** list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="098ca-137">すべての項目の識別子と変更キーをこの資料では、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="098ca-137">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
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
      <m:RemoveContactFromImList>
         <m:ContactId Id=""/>
      </m:RemoveContactFromImList>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="098ca-138">次の要素は、SOAP 本文の要求で使用されます。</span><span class="sxs-lookup"><span data-stu-id="098ca-138">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="098ca-139">RemoveContactFromImList</span><span class="sxs-lookup"><span data-stu-id="098ca-139">RemoveContactFromImList</span></span>](removecontactfromimlist.md)
    
- [<span data-ttu-id="098ca-140">ContactId</span><span class="sxs-lookup"><span data-stu-id="098ca-140">ContactId</span></span>](contactid.md)
    
## <a name="successful-removecontactfromimlist-operation-response"></a><span data-ttu-id="098ca-141">RemoveContactFromImList 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="098ca-141">Successful RemoveContactFromImList operation response</span></span>

<span data-ttu-id="098ca-142">次の例では、 **Lync の連絡先**リストから連絡先を削除するのには、 **RemoveContactFromImList**操作の要求に正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="098ca-142">The following example shows a successful response to a **RemoveContactFromImList** operation request to remove a contact from the **Lync Contacts** list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Success" 
                                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="098ca-143">応答 SOAP 本文では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="098ca-143">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="098ca-144">RemoveContactFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="098ca-144">RemoveContactFromImListResponse</span></span>](removecontactfromimlistresponse.md)
    
- [<span data-ttu-id="098ca-145">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="098ca-145">ResponseCode</span></span>](responsecode.md)
    
## <a name="removecontactfromimlist-operation-error-response"></a><span data-ttu-id="098ca-146">RemoveContactFromImList 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="098ca-146">RemoveContactFromImList operation error response</span></span>

<span data-ttu-id="098ca-147">**RemoveContactFromImList**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="098ca-147">The following example shows an error response to a **RemoveContactFromImList** operation request.</span></span> <span data-ttu-id="098ca-148">これは、連絡先が一覧に存在しない場合は、 **Lync の連絡先**リストから連絡先を削除する要求に応答します。</span><span class="sxs-lookup"><span data-stu-id="098ca-148">This is a response to a request to remove a contact from the **Lync Contacts** list when the contact no longer exists in the list.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <RemoveContactFromImListResponse ResponseClass="Error" 
                                       xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveContactFromImListResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="098ca-149">エラー応答 SOAP 本文では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="098ca-149">The following elements are used in the error response SOAP body:</span></span>
  
- [<span data-ttu-id="098ca-150">RemoveContactFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="098ca-150">RemoveContactFromImListResponse</span></span>](removecontactfromimlistresponse.md)
    
- [<span data-ttu-id="098ca-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="098ca-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="098ca-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="098ca-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="098ca-153">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="098ca-153">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="098ca-154">関連項目</span><span class="sxs-lookup"><span data-stu-id="098ca-154">See also</span></span>

- [<span data-ttu-id="098ca-155">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="098ca-155">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="098ca-156">GetImItemList 操作</span><span class="sxs-lookup"><span data-stu-id="098ca-156">GetImItemList operation</span></span>](getimitemlist-operation.md)
    

