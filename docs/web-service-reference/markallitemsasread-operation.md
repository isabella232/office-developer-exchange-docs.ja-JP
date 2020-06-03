---
title: MarkAllItemsAsRead 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ea5b1cb6-6998-46fb-a99c-a6d3da77591f
description: MarkAllItemsAsRead EWS 操作に関する情報を検索します。
ms.openlocfilehash: aeeacea1cd5eed723f93027dd1ef75b34605fdfd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530531"
---
# <a name="markallitemsasread-operation"></a><span data-ttu-id="cbfe2-103">MarkAllItemsAsRead 操作</span><span class="sxs-lookup"><span data-stu-id="cbfe2-103">MarkAllItemsAsRead operation</span></span>

<span data-ttu-id="cbfe2-104">**Markallitemsasread** EWS 操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-104">Find information about the **MarkAllItemsAsRead** EWS operation.</span></span> 
  
<span data-ttu-id="cbfe2-105">**Markallitemsasread**操作は、すべてのアイテムが開封済みまたは未読であることを示すために、1つまたは複数のフォルダー内のすべてのアイテムに対する[isread](isread.md)プロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-105">The **MarkAllItemsAsRead** operation sets the [IsRead](isread.md) property on all items, in one or more folders, to indicate that all items are either read or unread.</span></span> 
  
<span data-ttu-id="cbfe2-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-markallitemsasread-operation"></a><span data-ttu-id="cbfe2-107">MarkAllItemsAsRead 操作の使用</span><span class="sxs-lookup"><span data-stu-id="cbfe2-107">Using the MarkAllItemsAsRead operation</span></span>

<span data-ttu-id="cbfe2-108">**Markallitemsasread**操作は、Exchange Web サービス (EWS) フォルダー識別子または既定の exchange フォルダー名のいずれかによって識別されるフォルダー内のすべてのアイテムに対して[isread](isread.md)プロパティを設定できます。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-108">The **MarkAllItemsAsRead** operation can set the [IsRead](isread.md) property on all items in folders identified by either the Exchange Web Services (EWS) folder identifier or the default Exchange folder name.</span></span> <span data-ttu-id="cbfe2-109">**Markallitemsasread**操作によって、開封済みとしてマークされたアイテムの開封確認メッセージの送信を抑制することもできます。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-109">The **MarkAllItemsAsRead** operation can also suppress the sending of read receipts for items marked as read.</span></span> 
  
### <a name="markallitemsasread-operation-soap-headers"></a><span data-ttu-id="cbfe2-110">MarkAllItemsAsRead operation SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="cbfe2-110">MarkAllItemsAsRead operation SOAP headers</span></span>

<span data-ttu-id="cbfe2-111">**Markallitemsasread**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-111">The **MarkAllItemsAsRead** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="cbfe2-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="cbfe2-112">**Header name**</span></span>|<span data-ttu-id="cbfe2-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="cbfe2-113">**Element**</span></span>|<span data-ttu-id="cbfe2-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="cbfe2-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="cbfe2-115">**偽装**</span><span class="sxs-lookup"><span data-stu-id="cbfe2-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="cbfe2-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="cbfe2-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="cbfe2-117">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="cbfe2-118">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cbfe2-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="cbfe2-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="cbfe2-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="cbfe2-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="cbfe2-121">RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="cbfe2-122">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cbfe2-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="cbfe2-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="cbfe2-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="cbfe2-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="cbfe2-125">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="cbfe2-126">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="cbfe2-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="cbfe2-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="cbfe2-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="cbfe2-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="cbfe2-129">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="cbfe2-130">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-read"></a><span data-ttu-id="cbfe2-131">MarkAllItemsAsRead operation 要求の例: フォルダー内のすべてのアイテムを既読にします。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-131">MarkAllItemsAsRead operation request example: Mark all items in a folder as read</span></span>

<span data-ttu-id="cbfe2-132">**Markallitemsasread**操作要求の次の例は、フォルダー内のすべてのアイテムに対して、 [isread](isread.md)プロパティ (read フラグとも呼ばれます) を**true**に設定する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-132">The following example of a **MarkAllItemsAsRead** operation request shows how to set the [IsRead](isread.md) property, which is also called the read flag, to **true** on all items in a folder.</span></span> <span data-ttu-id="cbfe2-133">この例では、開封確認要求に対する応答で開封確認が送信されないことも示しています。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-133">This example also shows that read receipts are not sent in response to any read receipt requests.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="cbfe2-134">この記事のすべてのアイテム識別子と変更キーは、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> <span data-ttu-id="cbfe2-135">この操作では、キーを変更する必要はありません。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-135">Change keys are not required for this operation.</span></span> 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body>
      <m:MarkAllItemsAsRead>
         <m:ReadFlag>true</m:ReadFlag>
         <m:SuppressReadReceipts>true</m:SuppressReadReceipts>
         <m:FolderIds>
            <t:FolderId Id="AAMkADEzOTExYZRAAA=" 
                        ChangeKey="AQAAAAA3vA==" />
         </m:FolderIds>
      </m:MarkAllItemsAsRead>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="cbfe2-136">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-136">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cbfe2-137">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="cbfe2-137">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
    
- [<span data-ttu-id="cbfe2-138">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="cbfe2-138">ReadFlag</span></span>](readflag.md)
    
- [<span data-ttu-id="cbfe2-139">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="cbfe2-139">SuppressReadReceipts</span></span>](suppressreadreceipts.md)
    
- [<span data-ttu-id="cbfe2-140">FolderIds</span><span class="sxs-lookup"><span data-stu-id="cbfe2-140">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="cbfe2-141">FolderId</span><span class="sxs-lookup"><span data-stu-id="cbfe2-141">FolderId</span></span>](folderid.md)
    
## <a name="successful-markallitemsasread-operation-response"></a><span data-ttu-id="cbfe2-142">Successful MarkAllItemsAsRead operation 応答</span><span class="sxs-lookup"><span data-stu-id="cbfe2-142">Successful MarkAllItemsAsRead operation response</span></span>

<span data-ttu-id="cbfe2-143">次の例は、フォルダー内のすべてのアイテムを開封済みとしてマークするために、 **Markallitemsasread**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-143">The following example shows a successful response to a **MarkAllItemsAsRead** operation request to mark all items in a folder as read.</span></span> 
  
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
      <m:MarkAllItemsAsReadResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:MarkAllItemsAsReadResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
            </m:MarkAllItemsAsReadResponseMessage>
         </m:ResponseMessages>
      </m:MarkAllItemsAsReadResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="cbfe2-144">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-144">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cbfe2-145">MarkAllItemsAsReadResponse</span><span class="sxs-lookup"><span data-stu-id="cbfe2-145">MarkAllItemsAsReadResponse</span></span>](markallitemsasreadresponse.md)
    
- [<span data-ttu-id="cbfe2-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cbfe2-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="cbfe2-147">MarkAllItemsAsReadResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cbfe2-147">MarkAllItemsAsReadResponseMessage</span></span>](markallitemsasreadresponsemessage.md)
    
- [<span data-ttu-id="cbfe2-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cbfe2-148">ResponseCode</span></span>](responsecode.md)
    
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-unread"></a><span data-ttu-id="cbfe2-149">MarkAllItemsAsRead operation 要求の例: フォルダー内のすべてのアイテムを未読としてマークします</span><span class="sxs-lookup"><span data-stu-id="cbfe2-149">MarkAllItemsAsRead operation request example: Mark all items in a folder as unread</span></span>

<span data-ttu-id="cbfe2-150">次の**Markallitemsasread**操作要求の例は、フォルダー内のすべてのアイテムで[isread](isread.md)プロパティを**false**に設定する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-150">The following example of a **MarkAllItemsAsRead** operation request shows how to set the [IsRead](isread.md) property to **false** on all items in a folder.</span></span> <span data-ttu-id="cbfe2-151">この例では、開封確認要求に対する応答で開封確認が送信されないことも示しています。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-151">This example also shows that read receipts are not sent in response to any read receipt requests.</span></span> 
  
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
      <m:MarkAllItemsAsRead>
         <m:ReadFlag>false</m:ReadFlag>
         <m:SuppressReadReceipts>true</m:SuppressReadReceipts>
         <m:FolderIds>
            <t:FolderId Id="AAMkADEzOTExYZRAAA=" 
                        ChangeKey="AQAAAAA3vA==" />
         </m:FolderIds>
      </m:MarkAllItemsAsRead>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="cbfe2-152">すべてのアイテムを開封済みとしてマークする要求に対する正常な応答は、すべてのアイテムを未読としてマークする要求に対する応答と同じです。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-152">A successful response to a request to mark all items as read is the same as the response to a request to mark all items as unread.</span></span>
  
<span data-ttu-id="cbfe2-153">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-153">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cbfe2-154">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="cbfe2-154">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
    
- [<span data-ttu-id="cbfe2-155">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="cbfe2-155">ReadFlag</span></span>](readflag.md)
    
- [<span data-ttu-id="cbfe2-156">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="cbfe2-156">SuppressReadReceipts</span></span>](suppressreadreceipts.md)
    
- [<span data-ttu-id="cbfe2-157">FolderIds</span><span class="sxs-lookup"><span data-stu-id="cbfe2-157">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="cbfe2-158">FolderId</span><span class="sxs-lookup"><span data-stu-id="cbfe2-158">FolderId</span></span>](folderid.md)
    
## <a name="markallitemsasread-operation-error-response"></a><span data-ttu-id="cbfe2-159">MarkAllItemsAsRead 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="cbfe2-159">MarkAllItemsAsRead operation error response</span></span>

<span data-ttu-id="cbfe2-160">次の例は、フォルダーがメールボックス内に存在しない場合に、フォルダー内のすべてのアイテムに開封済みまたは未読マークを付けるための、 **Markallitemsasread**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-160">The following example shows an error response to a **MarkAllItemsAsRead** operation request to mark all items in a folder as read or unread when the folder does not exist in the mailbox.</span></span> 
  
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
      <m:MarkAllItemsAsReadResponse xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:MarkAllItemsAsReadResponseMessage ResponseClass="Error">
               <m:MessageText>The specified object was not found in the store.</m:MessageText>
               <m:ResponseCode>ErrorItemNotFound</m:ResponseCode>
               <m:DescriptiveLinkKey>0</m:DescriptiveLinkKey>
            </m:MarkAllItemsAsReadResponseMessage>
         </m:ResponseMessages>
      </m:MarkAllItemsAsReadResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="cbfe2-161">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="cbfe2-161">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="cbfe2-162">MarkAllItemsAsReadResponse</span><span class="sxs-lookup"><span data-stu-id="cbfe2-162">MarkAllItemsAsReadResponse</span></span>](markallitemsasreadresponse.md)
    
- [<span data-ttu-id="cbfe2-163">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="cbfe2-163">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="cbfe2-164">MarkAllItemsAsReadResponseMessage</span><span class="sxs-lookup"><span data-stu-id="cbfe2-164">MarkAllItemsAsReadResponseMessage</span></span>](markallitemsasreadresponsemessage.md)
    
- [<span data-ttu-id="cbfe2-165">MessageText</span><span class="sxs-lookup"><span data-stu-id="cbfe2-165">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="cbfe2-166">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="cbfe2-166">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="cbfe2-167">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="cbfe2-167">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="cbfe2-168">関連項目</span><span class="sxs-lookup"><span data-stu-id="cbfe2-168">See also</span></span>

- [<span data-ttu-id="cbfe2-169">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="cbfe2-169">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="cbfe2-170">FindFolder 操作</span><span class="sxs-lookup"><span data-stu-id="cbfe2-170">FindFolder operation</span></span>](findfolder-operation.md)
    

