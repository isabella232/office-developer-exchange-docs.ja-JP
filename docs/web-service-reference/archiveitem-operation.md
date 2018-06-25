---
title: ArchiveItem 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1af216b3-13ea-498e-b4fc-23513755d731
description: 操作 ArchiveItem EWS についての情報を検索します。
ms.openlocfilehash: 954943acefef8da61e92de5f8857ca023ca4fc9f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759433"
---
# <a name="archiveitem-operation"></a><span data-ttu-id="d36c0-103">ArchiveItem 操作</span><span class="sxs-lookup"><span data-stu-id="d36c0-103">ArchiveItem operation</span></span>

<span data-ttu-id="d36c0-104">**ArchiveItem** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="d36c0-104">Find information about the **ArchiveItem** EWS operation.</span></span> 
  
<span data-ttu-id="d36c0-105">**ArchiveItem**操作は、メールボックス ユーザーのアーカイブ メールボックスにアイテムを移動します。</span><span class="sxs-lookup"><span data-stu-id="d36c0-105">The **ArchiveItem** operation moves an item into the mailbox user's archive mailbox.</span></span> 
  
<span data-ttu-id="d36c0-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="d36c0-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-archiveitem-operation"></a><span data-ttu-id="d36c0-107">ArchiveItem 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="d36c0-107">Using the ArchiveItem operation</span></span>

<span data-ttu-id="d36c0-108">**ArchiveItem**操作では、要求でそのアイテムのアーカイブ先のメールボックスと移動先フォルダーに移動する項目を識別する 2 つの引数を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="d36c0-108">The **ArchiveItem** operation takes two arguments in the request that identify the items to move to the archive mailbox and the destination folder for those items.</span></span> <span data-ttu-id="d36c0-109">この操作を行うためには、アーカイブ メールボックスを有効にする必要があります。</span><span class="sxs-lookup"><span data-stu-id="d36c0-109">An archive mailbox must be enabled in order for this operation to work.</span></span> <span data-ttu-id="d36c0-110">アーカイブ メールボックスを有効にする方法については、[インプレース アーカイブの管理](http://technet.microsoft.com/en-us/library/jj651146.aspx)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d36c0-110">For information about how to enable an archive mailbox, see [Manage In-Place Archives](http://technet.microsoft.com/en-us/library/jj651146.aspx).</span></span>
  
### <a name="archiveitem-operation-soap-headers"></a><span data-ttu-id="d36c0-111">ArchiveItem 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d36c0-111">ArchiveItem operation SOAP headers</span></span>

<span data-ttu-id="d36c0-112">**ArchiveItem**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="d36c0-112">The **ArchiveItem** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="d36c0-113">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="d36c0-113">**Header name**</span></span>|<span data-ttu-id="d36c0-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="d36c0-114">**Element**</span></span>|<span data-ttu-id="d36c0-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="d36c0-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="d36c0-116">**偽装**</span><span class="sxs-lookup"><span data-stu-id="d36c0-116">**Impersonation**</span></span> <br/> |[<span data-ttu-id="d36c0-117">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="d36c0-117">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="d36c0-118">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="d36c0-118">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="d36c0-119">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d36c0-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d36c0-120">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="d36c0-120">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="d36c0-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="d36c0-121">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="d36c0-122">RFC 3066、**言語の識別用のタグ**を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="d36c0-122">Identifies the culture, as defined in RFC 3066, **Tags for the Identification of Languages**, to be used to access the mailbox.</span></span> <span data-ttu-id="d36c0-123">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d36c0-123">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d36c0-124">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="d36c0-124">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="d36c0-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="d36c0-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="d36c0-126">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="d36c0-126">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="d36c0-127">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d36c0-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="d36c0-128">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="d36c0-128">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="d36c0-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="d36c0-129">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="d36c0-130">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="d36c0-130">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="d36c0-131">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="d36c0-131">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="archiveitem-operation-request-example-move-an-item-to-the-archive-inbox-folder"></a><span data-ttu-id="d36c0-132">ArchiveItem 操作の要求の例: 保存 [受信トレイ] フォルダーにアイテムを移動</span><span class="sxs-lookup"><span data-stu-id="d36c0-132">ArchiveItem operation request example: Move an item to the archive inbox folder</span></span>

<span data-ttu-id="d36c0-133">**ArchiveItem**操作要求の次の例では、アーカイブの受信トレイ フォルダーにアイテムを移動する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="d36c0-133">The following example of an **ArchiveItem** operation request shows how to move an item to the archive Inbox folder.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="d36c0-134">すべての項目の識別子と変更キーをこの資料では、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="d36c0-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8" ?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="d36c0-135">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d36c0-135">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d36c0-136">ArchiveItem</span><span class="sxs-lookup"><span data-stu-id="d36c0-136">ArchiveItem</span></span>](archiveitem.md)    
- [<span data-ttu-id="d36c0-137">ArchiveSourceFolderId</span><span class="sxs-lookup"><span data-stu-id="d36c0-137">ArchiveSourceFolderId</span></span>](archivesourcefolderid.md)    
- [<span data-ttu-id="d36c0-138">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="d36c0-138">DistinguishedFolderId</span></span>](distinguishedfolderid.md)    
- [<span data-ttu-id="d36c0-139">Itemid</span><span class="sxs-lookup"><span data-stu-id="d36c0-139">ItemIds</span></span>](itemids.md)   
- [<span data-ttu-id="d36c0-140">ItemId</span><span class="sxs-lookup"><span data-stu-id="d36c0-140">ItemId</span></span>](itemid.md)
    
## <a name="successful-archiveitem-operation-response"></a><span data-ttu-id="d36c0-141">ArchiveItem 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="d36c0-141">Successful ArchiveItem operation response</span></span>

<span data-ttu-id="d36c0-142">次の例では、アーカイブ メールボックスにアイテムを移動するのには、 **ArchiveItem**操作の要求に正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="d36c0-142">The following example shows a successful response to an **ArchiveItem** operation request to move an item to an archive mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="526" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <m:ArchiveItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="d36c0-143">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d36c0-143">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d36c0-144">ArchiveItemResponse</span><span class="sxs-lookup"><span data-stu-id="d36c0-144">ArchiveItemResponse</span></span>](archiveitemresponse.md)    
- [<span data-ttu-id="d36c0-145">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d36c0-145">ResponseMessages</span></span>](responsemessages.md)   
- [<span data-ttu-id="d36c0-146">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d36c0-146">ArchiveItemResponseMessage</span></span>](archiveitemresponsemessage.md)    
- [<span data-ttu-id="d36c0-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d36c0-147">ResponseCode</span></span>](responsecode.md)    
- [<span data-ttu-id="d36c0-148">Items</span><span class="sxs-lookup"><span data-stu-id="d36c0-148">Items</span></span>](items.md)
    
## <a name="archiveitem-operation-error-response"></a><span data-ttu-id="d36c0-149">ArchiveItem 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="d36c0-149">ArchiveItem operation error response</span></span>

<span data-ttu-id="d36c0-150">**ArchiveItem**操作要求に対するエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="d36c0-150">The following example shows an error response to an **ArchiveItem** operation request.</span></span> <span data-ttu-id="d36c0-151">これは、ユーザーにアーカイブ メールボックスが有効になっていない場合は、アイテムをアーカイブするのには有効な要求への応答です。</span><span class="sxs-lookup"><span data-stu-id="d36c0-151">This is a response to a valid request to archive an item when an archive mailbox is not enabled for a user.</span></span> 
  
```xml
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
      <m:ArchiveItemResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                             xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="d36c0-152">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="d36c0-152">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="d36c0-153">ArchiveItemResponse</span><span class="sxs-lookup"><span data-stu-id="d36c0-153">ArchiveItemResponse</span></span>](archiveitemresponse.md)    
- [<span data-ttu-id="d36c0-154">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="d36c0-154">ResponseMessages</span></span>](responsemessages.md)    
- [<span data-ttu-id="d36c0-155">ArchiveItemResponseMessage</span><span class="sxs-lookup"><span data-stu-id="d36c0-155">ArchiveItemResponseMessage</span></span>](archiveitemresponsemessage.md)    
- [<span data-ttu-id="d36c0-156">MessageText</span><span class="sxs-lookup"><span data-stu-id="d36c0-156">MessageText</span></span>](messagetext.md)    
- [<span data-ttu-id="d36c0-157">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="d36c0-157">ResponseCode</span></span>](responsecode.md)    
- [<span data-ttu-id="d36c0-158">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="d36c0-158">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)    
- [<span data-ttu-id="d36c0-159">Items</span><span class="sxs-lookup"><span data-stu-id="d36c0-159">Items</span></span>](items.md)
    
<span data-ttu-id="d36c0-160">EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d36c0-160">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="d36c0-161">関連項目</span><span class="sxs-lookup"><span data-stu-id="d36c0-161">See also</span></span>

- [<span data-ttu-id="d36c0-162">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="d36c0-162">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md) 
- [<span data-ttu-id="d36c0-163">Exchange での EWS のアーカイブ</span><span class="sxs-lookup"><span data-stu-id="d36c0-163">Archiving in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/78ae179b-ae4f-4f64-911a-e0c70e0fa314%28Office.15%29.aspx)
    

