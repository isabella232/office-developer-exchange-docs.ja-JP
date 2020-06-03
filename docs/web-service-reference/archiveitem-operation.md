---
title: アーカイブアイテムの操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1af216b3-13ea-498e-b4fc-23513755d731
description: アーカイブアイテム EWS 操作に関する情報を検索します。
ms.openlocfilehash: d1e18122e67c36babbc8bf01d305309e2b17b568
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44463434"
---
# <a name="archiveitem-operation"></a><span data-ttu-id="c0e89-103">アーカイブアイテムの操作</span><span class="sxs-lookup"><span data-stu-id="c0e89-103">ArchiveItem operation</span></span>

<span data-ttu-id="c0e89-104">**アーカイブアイテム**EWS 操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="c0e89-104">Find information about the **ArchiveItem** EWS operation.</span></span> 
  
<span data-ttu-id="c0e89-105">**アーカイブアイテム**の操作によって、アイテムがメールボックスユーザーのアーカイブメールボックスに移動されます。</span><span class="sxs-lookup"><span data-stu-id="c0e89-105">The **ArchiveItem** operation moves an item into the mailbox user's archive mailbox.</span></span> 
  
<span data-ttu-id="c0e89-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="c0e89-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-archiveitem-operation"></a><span data-ttu-id="c0e89-107">アーカイブアイテム操作の使用</span><span class="sxs-lookup"><span data-stu-id="c0e89-107">Using the ArchiveItem operation</span></span>

<span data-ttu-id="c0e89-108">アーカイブ**アイテム**操作は、アーカイブメールボックスに移動するアイテムとそれらのアイテムの宛先フォルダーに移動するアイテムを識別する2つの引数を要求で受け取ります。</span><span class="sxs-lookup"><span data-stu-id="c0e89-108">The **ArchiveItem** operation takes two arguments in the request that identify the items to move to the archive mailbox and the destination folder for those items.</span></span> <span data-ttu-id="c0e89-109">この操作を動作させるには、アーカイブメールボックスを有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="c0e89-109">An archive mailbox must be enabled in order for this operation to work.</span></span> <span data-ttu-id="c0e89-110">アーカイブメールボックスを有効にする方法については、「[インプレースアーカイブを管理](https://technet.microsoft.com/library/jj651146.aspx)する」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="c0e89-110">For information about how to enable an archive mailbox, see [Manage In-Place Archives](https://technet.microsoft.com/library/jj651146.aspx).</span></span>
  
### <a name="archiveitem-operation-soap-headers"></a><span data-ttu-id="c0e89-111">アーカイブアイテム操作 SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="c0e89-111">ArchiveItem operation SOAP headers</span></span>

<span data-ttu-id="c0e89-112">**アーカイブアイテム**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="c0e89-112">The **ArchiveItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="c0e89-113">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="c0e89-113">**Header name**</span></span>|<span data-ttu-id="c0e89-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="c0e89-114">**Element**</span></span>|<span data-ttu-id="c0e89-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="c0e89-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="c0e89-116">**偽装**</span><span class="sxs-lookup"><span data-stu-id="c0e89-116">**Impersonation**</span></span> <br/> |[<span data-ttu-id="c0e89-117">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="c0e89-117">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="c0e89-118">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="c0e89-118">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="c0e89-119">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="c0e89-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c0e89-120">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="c0e89-120">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="c0e89-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="c0e89-121">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="c0e89-122">RFC 3066 で定義されているように、メールボックスへのアクセスに使用される**言語の識別用のタグ**を識別します。</span><span class="sxs-lookup"><span data-stu-id="c0e89-122">Identifies the culture, as defined in RFC 3066, **Tags for the Identification of Languages**, to be used to access the mailbox.</span></span> <span data-ttu-id="c0e89-123">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="c0e89-123">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c0e89-124">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="c0e89-124">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="c0e89-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="c0e89-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="c0e89-126">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="c0e89-126">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="c0e89-127">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="c0e89-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="c0e89-128">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="c0e89-128">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="c0e89-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="c0e89-129">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="c0e89-130">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="c0e89-130">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="c0e89-131">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="c0e89-131">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="archiveitem-operation-request-example-move-an-item-to-the-archive-inbox-folder"></a><span data-ttu-id="c0e89-132">アーカイブアイテム操作の要求例: アイテムをアーカイブ受信トレイフォルダーに移動します。</span><span class="sxs-lookup"><span data-stu-id="c0e89-132">ArchiveItem operation request example: Move an item to the archive inbox folder</span></span>

<span data-ttu-id="c0e89-133">次のアーカイブ**アイテム**操作要求の例は、アイテムをアーカイブ受信トレイフォルダーに移動する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="c0e89-133">The following example of an **ArchiveItem** operation request shows how to move an item to the archive Inbox folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="c0e89-134">この記事のすべてのアイテム識別子と変更キーは、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="c0e89-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body>
      <m:ArchiveItem>
         <m:ArchiveSourceFolderId>
            <t:DistinguishedFolderId Id="inbox"/>
         </m:ArchiveSourceFolderId>
         <m:ItemIds>
            <t:ItemId Id="AQMkG5BBwrQAAAxoAAAA=" ChangeKey="CQAAAHCtAAAAAAB7"/>
         </m:ItemIds>
      </m:ArchiveItem>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="c0e89-135">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0e89-135">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c0e89-136">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="c0e89-136">ArchiveItem</span></span>](archiveitem.md)    
- [<span data-ttu-id="c0e89-137">ArchiveSourceFolderId</span><span class="sxs-lookup"><span data-stu-id="c0e89-137">ArchiveSourceFolderId</span></span>](archivesourcefolderid.md)    
- [<span data-ttu-id="c0e89-138">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="c0e89-138">DistinguishedFolderId</span></span>](distinguishedfolderid.md)    
- [<span data-ttu-id="c0e89-139">ItemIds</span><span class="sxs-lookup"><span data-stu-id="c0e89-139">ItemIds</span></span>](itemids.md)   
- [<span data-ttu-id="c0e89-140">ItemId</span><span class="sxs-lookup"><span data-stu-id="c0e89-140">ItemId</span></span>](itemid.md)
    
## <a name="successful-archiveitem-operation-response"></a><span data-ttu-id="c0e89-141">アーカイブアイテム操作の応答が正常に行われる</span><span class="sxs-lookup"><span data-stu-id="c0e89-141">Successful ArchiveItem operation response</span></span>

<span data-ttu-id="c0e89-142">次の例は、アーカイブメールボックスにアイテムを移動するための、アーカイブ**アイテム**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="c0e89-142">The following example shows a successful response to an **ArchiveItem** operation request to move an item to an archive mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:ArchiveItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:ArchiveItemResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
               <m:Items/>
            </m:ArchiveItemResponseMessage>
         </m:ResponseMessages>
      </m:ArchiveItemResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="c0e89-143">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0e89-143">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c0e89-144">アーカイブ Itemresponse</span><span class="sxs-lookup"><span data-stu-id="c0e89-144">ArchiveItemResponse</span></span>](archiveitemresponse.md)    
- [<span data-ttu-id="c0e89-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c0e89-145">ResponseMessages</span></span>](responsemessages.md)   
- [<span data-ttu-id="c0e89-146">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c0e89-146">ArchiveItemResponseMessage</span></span>](archiveitemresponsemessage.md)    
- [<span data-ttu-id="c0e89-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c0e89-147">ResponseCode</span></span>](responsecode.md)    
- [<span data-ttu-id="c0e89-148">Items</span><span class="sxs-lookup"><span data-stu-id="c0e89-148">Items</span></span>](items.md)
    
## <a name="archiveitem-operation-error-response"></a><span data-ttu-id="c0e89-149">アーカイブアイテムの操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="c0e89-149">ArchiveItem operation error response</span></span>

<span data-ttu-id="c0e89-150">次の例は、**アーカイブアイテム**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="c0e89-150">The following example shows an error response to an **ArchiveItem** operation request.</span></span> <span data-ttu-id="c0e89-151">これは、アーカイブメールボックスがユーザーに対して有効になっていない場合にアイテムをアーカイブするための有効な要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="c0e89-151">This is a response to a valid request to archive an item when an archive mailbox is not enabled for a user.</span></span> 
  
```xml
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
      <m:ArchiveItemResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:ArchiveItemResponseMessage ResponseClass="Error">
               <m:MessageText>Archive mailbox is not enabled for this user.</m:MessageText>
               <m:ResponseCode>ErrorInvalidOperation</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
               <m:Items/>
            </m:ArchiveItemResponseMessage>
         </m:ResponseMessages>
      </m:ArchiveItemResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="c0e89-152">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="c0e89-152">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="c0e89-153">アーカイブ Itemresponse</span><span class="sxs-lookup"><span data-stu-id="c0e89-153">ArchiveItemResponse</span></span>](archiveitemresponse.md)    
- [<span data-ttu-id="c0e89-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="c0e89-154">ResponseMessages</span></span>](responsemessages.md)    
- [<span data-ttu-id="c0e89-155">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="c0e89-155">ArchiveItemResponseMessage</span></span>](archiveitemresponsemessage.md)    
- [<span data-ttu-id="c0e89-156">MessageText</span><span class="sxs-lookup"><span data-stu-id="c0e89-156">MessageText</span></span>](messagetext.md)    
- [<span data-ttu-id="c0e89-157">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="c0e89-157">ResponseCode</span></span>](responsecode.md)    
- [<span data-ttu-id="c0e89-158">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="c0e89-158">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)    
- [<span data-ttu-id="c0e89-159">Items</span><span class="sxs-lookup"><span data-stu-id="c0e89-159">Items</span></span>](items.md)
    
<span data-ttu-id="c0e89-160">EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)</span><span class="sxs-lookup"><span data-stu-id="c0e89-160">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="c0e89-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="c0e89-161">See also</span></span>

- [<span data-ttu-id="c0e89-162">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="c0e89-162">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md) 
- [<span data-ttu-id="c0e89-163">Exchange での EWS のアーカイブ</span><span class="sxs-lookup"><span data-stu-id="c0e89-163">Archiving in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/78ae179b-ae4f-4f64-911a-e0c70e0fa314%28Office.15%29.aspx)
    

