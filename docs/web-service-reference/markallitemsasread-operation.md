---
title: MarkAllItemsAsRead 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: ea5b1cb6-6998-46fb-a99c-a6d3da77591f
description: 操作 MarkAllItemsAsRead EWS についての情報を検索します。
ms.openlocfilehash: 995a6219f0a3b41bddb0d65c875d981322e1ce78
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832354"
---
# <a name="markallitemsasread-operation"></a><span data-ttu-id="e0b78-103">MarkAllItemsAsRead 操作</span><span class="sxs-lookup"><span data-stu-id="e0b78-103">MarkAllItemsAsRead operation</span></span>

<span data-ttu-id="e0b78-104">**MarkAllItemsAsRead** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="e0b78-104">Find information about the **MarkAllItemsAsRead** EWS operation.</span></span> 
  
<span data-ttu-id="e0b78-105">**MarkAllItemsAsRead**操作では、すべてのアイテムは、開封済みまたは未読のいずれかを示すために、1 つまたは複数のフォルダー内のすべてのアイテムの[IsRead](isread.md)プロパティを設定します。</span><span class="sxs-lookup"><span data-stu-id="e0b78-105">The **MarkAllItemsAsRead** operation sets the [IsRead](isread.md) property on all items, in one or more folders, to indicate that all items are either read or unread.</span></span> 
  
<span data-ttu-id="e0b78-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="e0b78-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-markallitemsasread-operation"></a><span data-ttu-id="e0b78-107">MarkAllItemsAsRead 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="e0b78-107">Using the MarkAllItemsAsRead operation</span></span>

<span data-ttu-id="e0b78-108">**MarkAllItemsAsRead**操作は、Exchange Web サービス (EWS) フォルダーの識別子または Exchange の既定のフォルダー名のいずれかによって識別されたフォルダー内のすべてのアイテムで、 [IsRead](isread.md)プロパティを設定できます。</span><span class="sxs-lookup"><span data-stu-id="e0b78-108">The **MarkAllItemsAsRead** operation can set the [IsRead](isread.md) property on all items in folders identified by either the Exchange Web Services (EWS) folder identifier or the default Exchange folder name.</span></span> <span data-ttu-id="e0b78-109">**MarkAllItemsAsRead**操作は、読み取りとしてマークされたアイテムを開封済みメッセージの送信を抑制してもできます。</span><span class="sxs-lookup"><span data-stu-id="e0b78-109">The **MarkAllItemsAsRead** operation can also suppress the sending of read receipts for items marked as read.</span></span> 
  
### <a name="markallitemsasread-operation-soap-headers"></a><span data-ttu-id="e0b78-110">MarkAllItemsAsRead 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e0b78-110">MarkAllItemsAsRead operation SOAP headers</span></span>

<span data-ttu-id="e0b78-111">**MarkAllItemsAsRead**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="e0b78-111">The **MarkAllItemsAsRead** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="e0b78-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="e0b78-112">**Header name**</span></span>|<span data-ttu-id="e0b78-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="e0b78-113">**Element**</span></span>|<span data-ttu-id="e0b78-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="e0b78-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="e0b78-115">**偽装**</span><span class="sxs-lookup"><span data-stu-id="e0b78-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="e0b78-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="e0b78-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="e0b78-117">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="e0b78-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="e0b78-118">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="e0b78-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e0b78-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="e0b78-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="e0b78-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="e0b78-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="e0b78-121">RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="e0b78-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="e0b78-122">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="e0b78-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e0b78-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="e0b78-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="e0b78-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="e0b78-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="e0b78-125">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="e0b78-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="e0b78-126">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="e0b78-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="e0b78-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="e0b78-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="e0b78-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="e0b78-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="e0b78-129">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="e0b78-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="e0b78-130">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="e0b78-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-read"></a><span data-ttu-id="e0b78-131">MarkAllItemsAsRead 操作の要求の例: 読み取りとフォルダーのすべてのアイテムをマークします。</span><span class="sxs-lookup"><span data-stu-id="e0b78-131">MarkAllItemsAsRead operation request example: Mark all items in a folder as read</span></span>

<span data-ttu-id="e0b78-132">**MarkAllItemsAsRead**操作要求の次の例にに**true を指定**フォルダー内のすべてのアイテムとも呼ばれる読み取りフラグ、 [IsRead](isread.md)プロパティを設定する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="e0b78-132">The following example of a **MarkAllItemsAsRead** operation request shows how to set the [IsRead](isread.md) property, which is also called the read flag, to **true** on all items in a folder.</span></span> <span data-ttu-id="e0b78-133">この例では、すべて開封済みメッセージ要求に対する応答で開封確認を送信しない読み取りも示します。</span><span class="sxs-lookup"><span data-stu-id="e0b78-133">This example also shows that read receipts are not sent in response to any read receipt requests.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="e0b78-134">すべての項目の識別子と変更キーをこの資料では、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="e0b78-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> <span data-ttu-id="e0b78-135">変更キーは、この操作に必要ではありません。</span><span class="sxs-lookup"><span data-stu-id="e0b78-135">Change keys are not required for this operation.</span></span> 
  
```XML
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
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

<span data-ttu-id="e0b78-136">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e0b78-136">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e0b78-137">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="e0b78-137">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
    
- [<span data-ttu-id="e0b78-138">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="e0b78-138">ReadFlag</span></span>](readflag.md)
    
- [<span data-ttu-id="e0b78-139">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="e0b78-139">SuppressReadReceipts</span></span>](suppressreadreceipts.md)
    
- [<span data-ttu-id="e0b78-140">FolderIds</span><span class="sxs-lookup"><span data-stu-id="e0b78-140">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="e0b78-141">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="e0b78-141">FolderId</span></span>](folderid.md)
    
## <a name="successful-markallitemsasread-operation-response"></a><span data-ttu-id="e0b78-142">MarkAllItemsAsRead 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="e0b78-142">Successful MarkAllItemsAsRead operation response</span></span>

<span data-ttu-id="e0b78-143">**MarkAllItemsAsRead**操作要求をフォルダー内のすべてのアイテムをマークするために正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e0b78-143">The following example shows a successful response to a **MarkAllItemsAsRead** operation request to mark all items in a folder as read.</span></span> 
  
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
      <m:MarkAllItemsAsReadResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
         <m:ResponseMessages>
            <m:MarkAllItemsAsReadResponseMessage ResponseClass="Success">
               <m:ResponseCode>NoError</m:ResponseCode>
            </m:MarkAllItemsAsReadResponseMessage>
         </m:ResponseMessages>
      </m:MarkAllItemsAsReadResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="e0b78-144">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e0b78-144">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e0b78-145">MarkAllItemsAsReadResponse</span><span class="sxs-lookup"><span data-stu-id="e0b78-145">MarkAllItemsAsReadResponse</span></span>](markallitemsasreadresponse.md)
    
- [<span data-ttu-id="e0b78-146">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e0b78-146">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e0b78-147">MarkAllItemsAsReadResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e0b78-147">MarkAllItemsAsReadResponseMessage</span></span>](markallitemsasreadresponsemessage.md)
    
- [<span data-ttu-id="e0b78-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e0b78-148">ResponseCode</span></span>](responsecode.md)
    
## <a name="markallitemsasread-operation-request-example-mark-all-items-in-a-folder-as-unread"></a><span data-ttu-id="e0b78-149">MarkAllItemsAsRead 操作の要求の例: 未読フォルダー内のすべてのアイテムをマークします。</span><span class="sxs-lookup"><span data-stu-id="e0b78-149">MarkAllItemsAsRead operation request example: Mark all items in a folder as unread</span></span>

<span data-ttu-id="e0b78-150">[IsRead](isread.md)プロパティを**false**に設定フォルダー内のすべての項目に対して**MarkAllItemsAsRead**操作要求の次の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="e0b78-150">The following example of a **MarkAllItemsAsRead** operation request shows how to set the [IsRead](isread.md) property to **false** on all items in a folder.</span></span> <span data-ttu-id="e0b78-151">この例では、すべて開封済みメッセージ要求に対する応答で開封確認を送信しない読み取りも示します。</span><span class="sxs-lookup"><span data-stu-id="e0b78-151">This example also shows that read receipts are not sent in response to any read receipt requests.</span></span> 
  
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

<span data-ttu-id="e0b78-152">すべてのアイテムを既読としてマークするための要求に正常な応答は、未読のすべてのアイテムをマークするための要求への応答と同じです。</span><span class="sxs-lookup"><span data-stu-id="e0b78-152">A successful response to a request to mark all items as read is the same as the response to a request to mark all items as unread.</span></span>
  
<span data-ttu-id="e0b78-153">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e0b78-153">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e0b78-154">MarkAllItemsAsRead</span><span class="sxs-lookup"><span data-stu-id="e0b78-154">MarkAllItemsAsRead</span></span>](markallitemsasread.md)
    
- [<span data-ttu-id="e0b78-155">ReadFlag</span><span class="sxs-lookup"><span data-stu-id="e0b78-155">ReadFlag</span></span>](readflag.md)
    
- [<span data-ttu-id="e0b78-156">SuppressReadReceipts</span><span class="sxs-lookup"><span data-stu-id="e0b78-156">SuppressReadReceipts</span></span>](suppressreadreceipts.md)
    
- [<span data-ttu-id="e0b78-157">FolderIds</span><span class="sxs-lookup"><span data-stu-id="e0b78-157">FolderIds</span></span>](folderids.md)
    
- [<span data-ttu-id="e0b78-158">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="e0b78-158">FolderId</span></span>](folderid.md)
    
## <a name="markallitemsasread-operation-error-response"></a><span data-ttu-id="e0b78-159">MarkAllItemsAsRead 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="e0b78-159">MarkAllItemsAsRead operation error response</span></span>

<span data-ttu-id="e0b78-160">次の使用例は、メールボックスのフォルダーが存在しない場合フォルダー内のすべてのアイテムを開封済みまたは未読としてマークするのには**MarkAllItemsAsRead**の操作要求に対するエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="e0b78-160">The following example shows an error response to a **MarkAllItemsAsRead** operation request to mark all items in a folder as read or unread when the folder does not exist in the mailbox.</span></span> 
  
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
      <m:MarkAllItemsAsReadResponse xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
                                    xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="e0b78-161">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="e0b78-161">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="e0b78-162">MarkAllItemsAsReadResponse</span><span class="sxs-lookup"><span data-stu-id="e0b78-162">MarkAllItemsAsReadResponse</span></span>](markallitemsasreadresponse.md)
    
- [<span data-ttu-id="e0b78-163">ResponseMessages</span><span class="sxs-lookup"><span data-stu-id="e0b78-163">ResponseMessages</span></span>](responsemessages.md)
    
- [<span data-ttu-id="e0b78-164">MarkAllItemsAsReadResponseMessage</span><span class="sxs-lookup"><span data-stu-id="e0b78-164">MarkAllItemsAsReadResponseMessage</span></span>](markallitemsasreadresponsemessage.md)
    
- [<span data-ttu-id="e0b78-165">MessageText</span><span class="sxs-lookup"><span data-stu-id="e0b78-165">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="e0b78-166">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="e0b78-166">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="e0b78-167">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="e0b78-167">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="e0b78-168">関連項目</span><span class="sxs-lookup"><span data-stu-id="e0b78-168">See also</span></span>

- [<span data-ttu-id="e0b78-169">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="e0b78-169">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- <span data-ttu-id="e0b78-170">
  [FindFolder 操作](findfolder-operation.md)</span><span class="sxs-lookup"><span data-stu-id="e0b78-170">[FindFolder operation](findfolder-operation.md)</span></span>
    

