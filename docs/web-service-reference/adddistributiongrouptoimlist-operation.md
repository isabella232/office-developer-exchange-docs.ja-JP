---
title: Adddeploy Grouptoimlist 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a
description: Adddeploy Grouptoimlist EWS 操作についての情報を検索します。
ms.openlocfilehash: e68e21b6994af5773f5cf991d55129e1db3367ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44463693"
---
# <a name="adddistributiongrouptoimlist-operation"></a><span data-ttu-id="7a125-103">Adddeploy Grouptoimlist 操作</span><span class="sxs-lookup"><span data-stu-id="7a125-103">AddDistributionGroupToImList operation</span></span>

<span data-ttu-id="7a125-104">**Adddeploy Grouptoimlist** EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="7a125-104">Find information about the **AddDistributionGroupToImList** EWS operation.</span></span> 
  
<span data-ttu-id="7a125-105">**Adddistribution Grouptoimlist** Exchange Web SERVICES (EWS) 操作は、統合連絡先ストアのインスタントメッセージング (IM) リストに配布グループを追加します。</span><span class="sxs-lookup"><span data-stu-id="7a125-105">The **AddDistributionGroupToImList** Exchange Web Services (EWS) operation adds a distribution group to the instant messaging (IM) list in the Unified Contact Store.</span></span> 
  
<span data-ttu-id="7a125-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7a125-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-adddistributiongrouptoimlist-operation"></a><span data-ttu-id="7a125-107">Adddeploy Grouptoimlist 操作の使用</span><span class="sxs-lookup"><span data-stu-id="7a125-107">Using the AddDistributionGroupToImList operation</span></span>

<span data-ttu-id="7a125-108">**Adddistribution Grouptoimlist**操作は、IM リストに追加する配布グループを識別する1つの引数を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="7a125-108">The **AddDistributionGroupToImList** operation takes a single argument that identifies a distribution group to add to the IM list.</span></span> <span data-ttu-id="7a125-109">この操作では、配布グループは作成されません。配布グループは既に作成されている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7a125-109">This operation does not create a distribution group; the distribution group must already be created.</span></span> 
  
<span data-ttu-id="7a125-110">この操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="7a125-110">This operation can use the SOAP headers that are listed in the following table.</span></span>
  
<span data-ttu-id="7a125-111">**表1Adddeploy Grouptoimlist 操作 SOAP ヘッダー**</span><span class="sxs-lookup"><span data-stu-id="7a125-111">**Table 1. AddDistributionGroupToImList operation SOAP headers**</span></span>

|<span data-ttu-id="7a125-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="7a125-112">**Header name**</span></span>|<span data-ttu-id="7a125-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="7a125-113">**Element**</span></span>|<span data-ttu-id="7a125-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="7a125-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7a125-115">**偽装**</span><span class="sxs-lookup"><span data-stu-id="7a125-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="7a125-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="7a125-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="7a125-117">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="7a125-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="7a125-118">これは要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="7a125-118">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7a125-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="7a125-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="7a125-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="7a125-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="7a125-121">RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。</span><span class="sxs-lookup"><span data-stu-id="7a125-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="7a125-122">これは要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="7a125-122">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7a125-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="7a125-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="7a125-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="7a125-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="7a125-125">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="7a125-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="7a125-126">これは要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="7a125-126">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7a125-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="7a125-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="7a125-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7a125-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="7a125-129">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="7a125-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="7a125-130">これは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="7a125-130">This is applicable to a response.</span></span>  <br/> |
   
## <a name="adddistributiongrouptoimlist-operation-request-example"></a><span data-ttu-id="7a125-131">Adddeploy Grouptoimlist 操作要求の例</span><span class="sxs-lookup"><span data-stu-id="7a125-131">AddDistributionGroupToImList operation request example</span></span>

<span data-ttu-id="7a125-132">次の**Adddistribution Grouptoimlist**操作要求の例は、配布グループを IM リストに追加する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="7a125-132">The following example of an **AddDistributionGroupToImList** operation request shows how to add a distribution group to the IM list.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
   </soap:Header>
   <soap:Body >
      <m:AddDistributionGroupToImList>
         <m:SmtpAddress>distributionlist1@example.com</m:SmtpAddress>
      </m:AddDistributionGroupToImList>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="7a125-133">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7a125-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7a125-134">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="7a125-134">AddDistributionGroupToImList</span></span>](adddistributiongrouptoimlist.md)   
- [<span data-ttu-id="7a125-135">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="7a125-135">SmtpAddress</span></span>](smtpaddress.md)
    
## <a name="successful-adddistributiongrouptoimlist-operation-response"></a><span data-ttu-id="7a125-136">Adddeploy Grouptoimlist 操作応答の成功</span><span class="sxs-lookup"><span data-stu-id="7a125-136">Successful AddDistributionGroupToImList operation response</span></span>

<span data-ttu-id="7a125-137">次の例は、 **Adddeploy Grouptoimlist**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="7a125-137">The following example shows a successful response to an **AddDistributionGroupToImList** operation request.</span></span> 
  
<span data-ttu-id="7a125-138">成功した応答には、配布グループの表示名、配布グループの Exchange ストアクラス、および新しい配布グループの EWS 識別子が含まれます。</span><span class="sxs-lookup"><span data-stu-id="7a125-138">The successful response contains the distribution group display name, the Exchange store class for the distribution group, and the EWS identifier of the new distribution group.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"
            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
            xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <s:Header>
      <t:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013"/>
   </s:Header>
   <s:Body>
      <m:AddDistributionGroupToImListResponse ResponseClass="Success">
         <m:ResponseCode>NoError</m:ResponseCode>
         <m:ImGroup>
            <t:DisplayName>distributionlist1@example.com</t:DisplayName>
            <t:GroupType>IPM.DistList.MOC.DG</t:GroupType>
            <t:ExchangeStoreId Id="AAMkAGQ1MjJjAA=" 
                             ChangeKey="EgAAAA=="/>
      </m:ImGroup>
      </m:AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="7a125-139">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7a125-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7a125-140">Adddeploy Grouptoimlistresponse</span><span class="sxs-lookup"><span data-stu-id="7a125-140">AddDistributionGroupToImListResponse</span></span>](adddistributiongrouptoimlistresponse.md)
    
- [<span data-ttu-id="7a125-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7a125-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7a125-142">ImGroup</span><span class="sxs-lookup"><span data-stu-id="7a125-142">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="7a125-143">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="7a125-143">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="7a125-144">GroupType</span><span class="sxs-lookup"><span data-stu-id="7a125-144">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="7a125-145">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="7a125-145">ExchangeStoreId</span></span>](exchangestoreid.md)
    
## <a name="adddistributiongrouptoimlist-operation-errorinvalidimdistributiongroupsmtpaddress-error-response"></a><span data-ttu-id="7a125-146">Adddeploy Grouptoimlist 操作 ErrorInvalidImDistributionGroupSmtpAddress エラー応答</span><span class="sxs-lookup"><span data-stu-id="7a125-146">AddDistributionGroupToImList operation ErrorInvalidImDistributionGroupSmtpAddress error response</span></span>

<span data-ttu-id="7a125-147">次の例は、 **Adddeploy Grouptoimlist**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="7a125-147">The following example shows an error response to an **AddDistributionGroupToImList** operation request.</span></span> <span data-ttu-id="7a125-148">Exchange ストアに存在しない配布グループを追加しようとすると、次のエラー応答が発生します。</span><span class="sxs-lookup"><span data-stu-id="7a125-148">The following error response occurs when an attempt is made to add a distribution group that does not exist in the Exchange store.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddDistributionGroupToImListResponse ResponseClass="Error" 
                                            xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified IM distribution group SMTP address is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImDistributionGroupSmtpAddress</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="7a125-149">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7a125-149">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7a125-150">Adddeploy Grouptoimlistresponse</span><span class="sxs-lookup"><span data-stu-id="7a125-150">AddDistributionGroupToImListResponse</span></span>](adddistributiongrouptoimlistresponse.md)
    
- [<span data-ttu-id="7a125-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="7a125-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="7a125-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7a125-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="7a125-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="7a125-153">See also</span></span>

- [<span data-ttu-id="7a125-154">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="7a125-154">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)   
- [<span data-ttu-id="7a125-155">AddImGroup</span><span class="sxs-lookup"><span data-stu-id="7a125-155">AddImGroup</span></span>](addimgroup-operation.md)   
- [<span data-ttu-id="7a125-156">RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="7a125-156">RemoveImGroup</span></span>](removeimgroup-operation.md)
    

