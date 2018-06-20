---
title: AddDistributionGroupToImList 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5aa9bec8-71cf-4a6e-8ec8-b4965b40fd4a
description: 操作 AddDistributionGroupToImList EWS についての情報を検索します。
ms.openlocfilehash: 7c562c317890a4cffb9e5844ea41c1096a8595b4
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759277"
---
# <a name="adddistributiongrouptoimlist-operation"></a><span data-ttu-id="66cbd-103">AddDistributionGroupToImList 操作</span><span class="sxs-lookup"><span data-stu-id="66cbd-103">AddDistributionGroupToImList operation</span></span>

<span data-ttu-id="66cbd-104">**AddDistributionGroupToImList** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="66cbd-104">Find information about the **AddDistributionGroupToImList** EWS operation.</span></span> 
  
<span data-ttu-id="66cbd-105">**AddDistributionGroupToImList** Exchange Web サービス (EWS) 操作では、インスタント メッセージング (IM)] ボックスの一覧では、統合連絡先ストアに配布グループを追加します。</span><span class="sxs-lookup"><span data-stu-id="66cbd-105">The **AddDistributionGroupToImList** Exchange Web Services (EWS) operation adds a distribution group to the instant messaging (IM) list in the Unified Contact Store.</span></span> 
  
<span data-ttu-id="66cbd-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="66cbd-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-adddistributiongrouptoimlist-operation"></a><span data-ttu-id="66cbd-107">AddDistributionGroupToImList 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="66cbd-107">Using the AddDistributionGroupToImList operation</span></span>

<span data-ttu-id="66cbd-108">**AddDistributionGroupToImList**操作では、IM のリストに追加する配布グループを識別する 1 つの引数を受け取ります。</span><span class="sxs-lookup"><span data-stu-id="66cbd-108">The **AddDistributionGroupToImList** operation takes a single argument that identifies a distribution group to add to the IM list.</span></span> <span data-ttu-id="66cbd-109">この操作は、配布グループを作成できません。配布グループを作成することが既に必要があります。</span><span class="sxs-lookup"><span data-stu-id="66cbd-109">This operation does not create a distribution group; the distribution group must already be created.</span></span> 
  
<span data-ttu-id="66cbd-110">この操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="66cbd-110">This operation can use the SOAP headers that are listed in the following table.</span></span>
  
<span data-ttu-id="66cbd-111">**表 1 です。AddDistributionGroupToImList 操作の SOAP ヘッダー**</span><span class="sxs-lookup"><span data-stu-id="66cbd-111">**Table 1. AddDistributionGroupToImList operation SOAP headers**</span></span>

|<span data-ttu-id="66cbd-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="66cbd-112">**Header name**</span></span>|<span data-ttu-id="66cbd-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="66cbd-113">**Element**</span></span>|<span data-ttu-id="66cbd-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="66cbd-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="66cbd-115">**偽装**</span><span class="sxs-lookup"><span data-stu-id="66cbd-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="66cbd-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="66cbd-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="66cbd-117">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="66cbd-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="66cbd-118">これは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="66cbd-118">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="66cbd-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="66cbd-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="66cbd-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="66cbd-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="66cbd-121">RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="66cbd-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="66cbd-122">これは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="66cbd-122">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="66cbd-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="66cbd-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="66cbd-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="66cbd-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="66cbd-125">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="66cbd-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="66cbd-126">これは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="66cbd-126">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="66cbd-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="66cbd-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="66cbd-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="66cbd-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="66cbd-129">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="66cbd-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="66cbd-130">これは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="66cbd-130">This is applicable to a response.</span></span>  <br/> |
   
## <a name="adddistributiongrouptoimlist-operation-request-example"></a><span data-ttu-id="66cbd-131">AddDistributionGroupToImList 操作の要求の例</span><span class="sxs-lookup"><span data-stu-id="66cbd-131">AddDistributionGroupToImList operation request example</span></span>

<span data-ttu-id="66cbd-132">**AddDistributionGroupToImList**操作要求の次の例では、IM のリストに配布グループを追加する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="66cbd-132">The following example of an **AddDistributionGroupToImList** operation request shows how to add a distribution group to the IM list.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="66cbd-133">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="66cbd-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="66cbd-134">AddDistributionGroupToImList</span><span class="sxs-lookup"><span data-stu-id="66cbd-134">AddDistributionGroupToImList</span></span>](adddistributiongrouptoimlist.md)   
- [<span data-ttu-id="66cbd-135">SmtpAddress</span><span class="sxs-lookup"><span data-stu-id="66cbd-135">SmtpAddress</span></span>](smtpaddress.md)
    
## <a name="successful-adddistributiongrouptoimlist-operation-response"></a><span data-ttu-id="66cbd-136">AddDistributionGroupToImList 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="66cbd-136">Successful AddDistributionGroupToImList operation response</span></span>

<span data-ttu-id="66cbd-137">**AddDistributionGroupToImList**操作の要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="66cbd-137">The following example shows a successful response to an **AddDistributionGroupToImList** operation request.</span></span> 
  
<span data-ttu-id="66cbd-138">正常な応答には、配布グループの表示名、配布グループと、EWS 識別子の新しい配布グループの Exchange ストアのクラスが含まれています。</span><span class="sxs-lookup"><span data-stu-id="66cbd-138">The successful response contains the distribution group display name, the Exchange store class for the distribution group, and the EWS identifier of the new distribution group.</span></span>
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"
            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
            xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="66cbd-139">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="66cbd-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="66cbd-140">AddDistributionGroupToImListResponse</span><span class="sxs-lookup"><span data-stu-id="66cbd-140">AddDistributionGroupToImListResponse</span></span>](adddistributiongrouptoimlistresponse.md)
    
- [<span data-ttu-id="66cbd-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="66cbd-141">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="66cbd-142">ImGroup</span><span class="sxs-lookup"><span data-stu-id="66cbd-142">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="66cbd-143">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="66cbd-143">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="66cbd-144">GroupType</span><span class="sxs-lookup"><span data-stu-id="66cbd-144">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="66cbd-145">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="66cbd-145">ExchangeStoreId</span></span>](exchangestoreid.md)
    
## <a name="adddistributiongrouptoimlist-operation-errorinvalidimdistributiongroupsmtpaddress-error-response"></a><span data-ttu-id="66cbd-146">AddDistributionGroupToImList 操作エラー応答の ErrorInvalidImDistributionGroupSmtpAddress</span><span class="sxs-lookup"><span data-stu-id="66cbd-146">AddDistributionGroupToImList operation ErrorInvalidImDistributionGroupSmtpAddress error response</span></span>

<span data-ttu-id="66cbd-147">**AddDistributionGroupToImList**操作要求に対するエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="66cbd-147">The following example shows an error response to an **AddDistributionGroupToImList** operation request.</span></span> <span data-ttu-id="66cbd-148">次のエラー応答は、Exchange ストア内に存在しない配布グループを追加しようとしましたがときに発生します。</span><span class="sxs-lookup"><span data-stu-id="66cbd-148">The following error response occurs when an attempt is made to add a distribution group that does not exist in the Exchange store.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddDistributionGroupToImListResponse ResponseClass="Error" 
                                            xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified IM distribution group SMTP address is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImDistributionGroupSmtpAddress</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddDistributionGroupToImListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="66cbd-149">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="66cbd-149">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="66cbd-150">AddDistributionGroupToImListResponse</span><span class="sxs-lookup"><span data-stu-id="66cbd-150">AddDistributionGroupToImListResponse</span></span>](adddistributiongrouptoimlistresponse.md)
    
- [<span data-ttu-id="66cbd-151">MessageText</span><span class="sxs-lookup"><span data-stu-id="66cbd-151">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="66cbd-152">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="66cbd-152">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="66cbd-153">関連項目</span><span class="sxs-lookup"><span data-stu-id="66cbd-153">See also</span></span>

- [<span data-ttu-id="66cbd-154">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="66cbd-154">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)   
- [<span data-ttu-id="66cbd-155">AddImGroup</span><span class="sxs-lookup"><span data-stu-id="66cbd-155">AddImGroup</span></span>](addimgroup-operation.md)   
- [<span data-ttu-id="66cbd-156">RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="66cbd-156">RemoveImGroup</span></span>](removeimgroup-operation.md)
    

