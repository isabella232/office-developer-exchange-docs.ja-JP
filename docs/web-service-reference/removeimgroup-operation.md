---
title: RemoveImGroup 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 5e788016-68e0-4a3f-9243-03f6b6c6b389
description: 操作 RemoveImGroup EWS についての情報を検索します。
ms.openlocfilehash: 85b312f0b156125a2d5395658ccea06d831abdde
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833097"
---
# <a name="removeimgroup-operation"></a><span data-ttu-id="47214-103">RemoveImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="47214-103">RemoveImGroup operation</span></span>

<span data-ttu-id="47214-104">**RemoveImGroup** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="47214-104">Find information about the **RemoveImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="47214-105">**RemoveImGroup**操作は、メールボックスからのインスタント メッセージング (IM) のグループは、1 つを削除します。</span><span class="sxs-lookup"><span data-stu-id="47214-105">The **RemoveImGroup** operation removes a single instant messaging (IM) group from a mailbox.</span></span> 
  
<span data-ttu-id="47214-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="47214-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-removeimgroup-operation"></a><span data-ttu-id="47214-107">RemoveImGroup 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="47214-107">Using the RemoveImGroup operation</span></span>

<span data-ttu-id="47214-108">のみ、 **RemoveImGroup**操作は、1 つのグループ識別子の引数を取る。</span><span class="sxs-lookup"><span data-stu-id="47214-108">The **RemoveImGroup** operation only takes a single group identifier argument.</span></span> 
  
### <a name="removeimgroup-operation-soap-headers"></a><span data-ttu-id="47214-109">RemoveImGroup 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="47214-109">RemoveImGroup operation SOAP headers</span></span>

<span data-ttu-id="47214-110">**RemoveImGroup**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="47214-110">The **RemoveImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="47214-111">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="47214-111">**Header name**</span></span>|<span data-ttu-id="47214-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="47214-112">**Element**</span></span>|<span data-ttu-id="47214-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="47214-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="47214-114">**偽装**</span><span class="sxs-lookup"><span data-stu-id="47214-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="47214-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="47214-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="47214-116">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="47214-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="47214-117">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="47214-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="47214-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="47214-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="47214-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="47214-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="47214-120">RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="47214-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="47214-121">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="47214-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="47214-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="47214-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="47214-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="47214-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="47214-124">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="47214-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="47214-125">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="47214-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="47214-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="47214-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="47214-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="47214-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="47214-128">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="47214-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="47214-129">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="47214-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="removeimgroup-operation-request-example"></a><span data-ttu-id="47214-130">RemoveImGroup 操作の要求の例</span><span class="sxs-lookup"><span data-stu-id="47214-130">RemoveImGroup operation request example</span></span>

<span data-ttu-id="47214-131">**RemoveImGroup**操作要求の次の例では、IM グループを削除する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="47214-131">The following example of a **RemoveImGroup** operation request shows how to remove an IM group.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="47214-132">グループ ID が小さすぎると読みやすさを保持します。</span><span class="sxs-lookup"><span data-stu-id="47214-132">The group ID has been shortened to preserve readability.</span></span> 
  
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
      <m:RemoveImGroup>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5hQoTbWAAAAAAQRAAA="
                    ChangeKey="EgAAAA=="/>
      </m:RemoveImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="47214-133">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="47214-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="47214-134">RemoveImGroup</span><span class="sxs-lookup"><span data-stu-id="47214-134">RemoveImGroup</span></span>](removeimgroup.md)
    
- [<span data-ttu-id="47214-135">グループ Id</span><span class="sxs-lookup"><span data-stu-id="47214-135">GroupId</span></span>](groupid.md)
    
## <a name="successful-removeimgroup-operation-response"></a><span data-ttu-id="47214-136">RemoveImGroup 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="47214-136">Successful RemoveImGroup operation response</span></span>

<span data-ttu-id="47214-137">成功した要求への応答、 **RemoveImGroup**操作の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="47214-137">The following example shows a successful response to a **RemoveImGroup** operation request.</span></span> 
  
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
      <RemoveImGroupResponse ResponseClass="Success" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="47214-138">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="47214-138">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="47214-139">RemoveImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="47214-139">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="47214-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="47214-140">ResponseCode</span></span>](responsecode.md)
    
## <a name="removeimgroup-operation-errorinvalidimgroupid-error-response"></a><span data-ttu-id="47214-141">RemoveImGroup 操作エラー応答の ErrorInvalidImGroupId</span><span class="sxs-lookup"><span data-stu-id="47214-141">RemoveImGroup operation ErrorInvalidImGroupId error response</span></span>

<span data-ttu-id="47214-142">**RemoveImGroup**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="47214-142">The following example shows an error response to a **RemoveImGroup** operation request.</span></span> <span data-ttu-id="47214-143">次のエラー応答は、メールボックス内に存在しないグループを削除しようとしましたがときに発生します。</span><span class="sxs-lookup"><span data-stu-id="47214-143">The following error response occurs when an attempt is made to remove a group that does not exist in the mailbox.</span></span> 
  
```XML
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
      <RemoveImGroupResponse ResponseClass="Error" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified Im Group Id is invalid.</MessageText>
         <ResponseCode>ErrorInvalidImGroupId</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="47214-144">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="47214-144">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="47214-145">RemoveImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="47214-145">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="47214-146">MessageText</span><span class="sxs-lookup"><span data-stu-id="47214-146">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="47214-147">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="47214-147">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="47214-148">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="47214-148">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="47214-149">EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="47214-149">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="removeimgroup-operation-errorinvalididmalformed-error-response"></a><span data-ttu-id="47214-150">RemoveImGroup 操作エラー応答の ErrorInvalidIdMalformed</span><span class="sxs-lookup"><span data-stu-id="47214-150">RemoveImGroup operation ErrorInvalidIdMalformed error response</span></span>

<span data-ttu-id="47214-151">**RemoveImGroup**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="47214-151">The following example shows an error response to a **RemoveImGroup** operation request.</span></span> <span data-ttu-id="47214-152">次のエラー応答は、誤った形式のグループ識別子を持つグループを削除しようとしましたがときに発生します。</span><span class="sxs-lookup"><span data-stu-id="47214-152">The following error response occurs when an attempt is made to remove a group with an incorrectly formatted group identifier.</span></span> 
  
```XML
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
      <RemoveImGroupResponse ResponseClass="Error" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Id is malformed.</MessageText>
         <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </RemoveImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="47214-153">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="47214-153">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="47214-154">RemoveImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="47214-154">RemoveImGroupResponse</span></span>](removeimgroupresponse.md)
    
- [<span data-ttu-id="47214-155">MessageText</span><span class="sxs-lookup"><span data-stu-id="47214-155">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="47214-156">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="47214-156">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="47214-157">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="47214-157">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="47214-158">関連項目</span><span class="sxs-lookup"><span data-stu-id="47214-158">See also</span></span>

- [<span data-ttu-id="47214-159">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="47214-159">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="47214-160">AddImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="47214-160">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="47214-161">SetImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="47214-161">SetImGroup operation</span></span>](setimgroup-operation.md)
    

