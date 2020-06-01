---
title: RemoveDistributionGroupFromImList 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 252bddf2-98b6-4824-b548-2fba2bda5384
description: RemoveDistributionGroupFromImList EWS 操作についての情報を検索します。
ms.openlocfilehash: 66220f0cab99f404e17136bbb7836ca13d569b53
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459603"
---
# <a name="removedistributiongroupfromimlist-operation"></a><span data-ttu-id="2849f-103">RemoveDistributionGroupFromImList 操作</span><span class="sxs-lookup"><span data-stu-id="2849f-103">RemoveDistributionGroupFromImList operation</span></span>

<span data-ttu-id="2849f-104">**RemoveDistributionGroupFromImList** EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="2849f-104">Find information about the **RemoveDistributionGroupFromImList** EWS operation.</span></span> 
  
<span data-ttu-id="2849f-105">**RemoveDistributionGroupFromImList**操作では、lync が連絡先ストアに対して Exchange を使用している場合に、lync インスタントメッセージング (IM) リストから配布グループを削除します。</span><span class="sxs-lookup"><span data-stu-id="2849f-105">The **RemoveDistributionGroupFromImList** operation removes a distribution group from the Lync instant messaging (IM) list when Lync uses Exchange for the contact store.</span></span> 
  
<span data-ttu-id="2849f-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="2849f-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removedistributiongroupfromimlist-operation"></a><span data-ttu-id="2849f-107">RemoveDistributionGroupFromImList 操作の使用</span><span class="sxs-lookup"><span data-stu-id="2849f-107">Using the RemoveDistributionGroupFromImList operation</span></span>

<span data-ttu-id="2849f-108">**RemoveDistributionGroupFromImList**操作は、Exchange サーバーに格納されている Lync IM リストから削除する配布グループを識別する1つの引数を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="2849f-108">The **RemoveDistributionGroupFromImList** operation accepts a single argument that identifies a distribution group to remove from the Lync IM list stored on an Exchange server.</span></span> 
  
### <a name="removedistributiongroupfromimlist-operation-soap-headers"></a><span data-ttu-id="2849f-109">RemoveDistributionGroupFromImList 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="2849f-109">RemoveDistributionGroupFromImList operation SOAP headers</span></span>

<span data-ttu-id="2849f-110">**RemoveDistributionGroupFromImList**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="2849f-110">The **RemoveDistributionGroupFromImList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="2849f-111">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="2849f-111">**Header name**</span></span>|<span data-ttu-id="2849f-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="2849f-112">**Element**</span></span>|<span data-ttu-id="2849f-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="2849f-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="2849f-114">**偽装**</span><span class="sxs-lookup"><span data-stu-id="2849f-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="2849f-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="2849f-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="2849f-116">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="2849f-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="2849f-117">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="2849f-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="2849f-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="2849f-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="2849f-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="2849f-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="2849f-120">RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。</span><span class="sxs-lookup"><span data-stu-id="2849f-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="2849f-121">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="2849f-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="2849f-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="2849f-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="2849f-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="2849f-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="2849f-124">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="2849f-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="2849f-125">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="2849f-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="2849f-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="2849f-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="2849f-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="2849f-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="2849f-128">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="2849f-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="2849f-129">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="2849f-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removedistributiongroupfromimlist-operation-request-example-remove-a-distribution-group-from-an-im-list"></a><span data-ttu-id="2849f-130">RemoveDistributionGroupFromImList 操作要求の例: IM リストから配布グループを削除する</span><span class="sxs-lookup"><span data-stu-id="2849f-130">RemoveDistributionGroupFromImList operation request example: Remove a distribution group from an IM list</span></span>

<span data-ttu-id="2849f-131">次の**RemoveDistributionGroupFromImList**操作要求の例は、IM グループから配布グループを削除する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="2849f-131">The following example of a **RemoveDistributionGroupFromImList** operation request shows how to remove a distribution group from an IM group.</span></span> <span data-ttu-id="2849f-132">**RemoveDistributionGroupFromImList**操作は、IM リストから削除する配布グループを識別する一意のグループ識別子を受け入れます。</span><span class="sxs-lookup"><span data-stu-id="2849f-132">The **RemoveDistributionGroupFromImList** operation accepts the unique group identifier to identify the distribution group to remove from the IM list.</span></span> <span data-ttu-id="2849f-133">[Getimitemlist 操作](getimitemlist-operation.md)と[Adddistribution grouptoimlist 操作](adddistributiongrouptoimlist-operation.md)の応答で返される[ExchangeStoreId](exchangestoreid.md)要素は、IM リストから削除できる配布グループを識別します。</span><span class="sxs-lookup"><span data-stu-id="2849f-133">The [ExchangeStoreId](exchangestoreid.md) element that is returned in the response for the [GetImItemList operation](getimitemlist-operation.md) and the [AddDistributionGroupToImList operation](adddistributiongrouptoimlist-operation.md) identifies distribution groups that can be removed from the IM list.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="2849f-134">この記事のすべてのアイテム識別子と変更キーは、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="2849f-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:RemoveDistributionGroupFromImList>
         <m:GroupId Id="AAMkADEzO4QrAABmEh5oAAA="/>
      </m:RemoveDistributionGroupFromImList>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="2849f-135">要求 SOAP 本文では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="2849f-135">The following elements are used in the request SOAP body:</span></span>
  
- [<span data-ttu-id="2849f-136">RemoveDistributionGroupFromImList</span><span class="sxs-lookup"><span data-stu-id="2849f-136">RemoveDistributionGroupFromImList</span></span>](removedistributiongroupfromimlist.md)
    
- [<span data-ttu-id="2849f-137">GroupId</span><span class="sxs-lookup"><span data-stu-id="2849f-137">GroupId</span></span>](groupid.md)
    
## <a name="successful-removedistributiongroupfromimlist-operation-response"></a><span data-ttu-id="2849f-138">成功した RemoveDistributionGroupFromImList 操作の応答</span><span class="sxs-lookup"><span data-stu-id="2849f-138">Successful RemoveDistributionGroupFromImList operation response</span></span>

<span data-ttu-id="2849f-139">次の例は、IM グループから配布グループを削除するための**RemoveDistributionGroupFromImList**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="2849f-139">The following example shows a successful response to a **RemoveDistributionGroupFromImList** operation request to a remove a distribution group from an IM group.</span></span> 
  
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
      <RemoveDistributionGroupFromImListResponse ResponseClass="Success" 
                                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveDistributionGroupFromImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="2849f-140">応答 SOAP 本文では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="2849f-140">The following elements are used in the response SOAP body:</span></span>
  
- [<span data-ttu-id="2849f-141">RemoveDistributionGroupFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="2849f-141">RemoveDistributionGroupFromImListResponse</span></span>](removedistributiongroupfromimlistresponse.md)
    
- [<span data-ttu-id="2849f-142">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2849f-142">ResponseCode</span></span>](responsecode.md)
    
## <a name="removedistributiongroupfromimlist-operation-error-response-example"></a><span data-ttu-id="2849f-143">RemoveDistributionGroupFromImList 操作エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="2849f-143">RemoveDistributionGroupFromImList operation error response example</span></span>

<span data-ttu-id="2849f-144">次の例は、 **RemoveDistributionGroupFromImList**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="2849f-144">The following example shows an error response to a **RemoveDistributionGroupFromImList** operation request.</span></span> <span data-ttu-id="2849f-145">これは、既にメールボックスから削除されている配布グループを削除する要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="2849f-145">This is a response to a request to remove a distribution group that has already been removed from the mailbox.</span></span> 
  
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
      <RemoveDistributionGroupFromImListResponse ResponseClass="Error" 
                                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveDistributionGroupFromImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="2849f-146">エラー応答 SOAP 本文では、次の要素が使用されます。</span><span class="sxs-lookup"><span data-stu-id="2849f-146">The following elements are used in the error response SOAP body:</span></span>
  
- [<span data-ttu-id="2849f-147">RemoveDistributionGroupFromImListResponse</span><span class="sxs-lookup"><span data-stu-id="2849f-147">RemoveDistributionGroupFromImListResponse</span></span>](removedistributiongroupfromimlistresponse.md)
    
- [<span data-ttu-id="2849f-148">MessageText</span><span class="sxs-lookup"><span data-stu-id="2849f-148">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="2849f-149">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="2849f-149">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="2849f-150">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="2849f-150">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="2849f-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="2849f-151">See also</span></span>

- [<span data-ttu-id="2849f-152">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="2849f-152">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="2849f-153">GetImItemList 操作</span><span class="sxs-lookup"><span data-stu-id="2849f-153">GetImItemList operation</span></span>](getimitemlist-operation.md)
    
- [<span data-ttu-id="2849f-154">Adddeploy Grouptoimlist 操作</span><span class="sxs-lookup"><span data-stu-id="2849f-154">AddDistributionGroupToImList operation</span></span>](adddistributiongrouptoimlist-operation.md)
    
- [<span data-ttu-id="2849f-155">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="2849f-155">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx#What)
    

