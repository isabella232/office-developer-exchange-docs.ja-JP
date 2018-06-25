---
title: SetImGroup 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2d48aa07-8152-4c3d-a519-061253e80174
description: 操作 SetImGroup EWS についての情報を検索します。
ms.openlocfilehash: 80980c25888ab3fcae0a761e115c3ac3d578a013
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833421"
---
# <a name="setimgroup-operation"></a><span data-ttu-id="40d68-103">SetImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="40d68-103">SetImGroup operation</span></span>

<span data-ttu-id="40d68-104">**SetImGroup** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="40d68-104">Find information about the **SetImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="40d68-105">**SetImGroup**操作では、インスタント メッセージング (IM) のグループの表示名を変更します。</span><span class="sxs-lookup"><span data-stu-id="40d68-105">The **SetImGroup** operation changes the display name of an instant messaging (IM) group.</span></span> 
  
<span data-ttu-id="40d68-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="40d68-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-setimgroup-operation"></a><span data-ttu-id="40d68-107">SetImGroup 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="40d68-107">Using the SetImGroup operation</span></span>

<span data-ttu-id="40d68-108">**SetImGroup**操作には、単一の表示名の引数はわずかです。</span><span class="sxs-lookup"><span data-stu-id="40d68-108">The **SetImGroup** operation only takes a single display name argument.</span></span> 
  
### <a name="setimgroup-operation-soap-headers"></a><span data-ttu-id="40d68-109">SetImGroup 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="40d68-109">SetImGroup operation SOAP headers</span></span>

<span data-ttu-id="40d68-110">**SetImGroup**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="40d68-110">The **SetImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="40d68-111">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="40d68-111">**Header name**</span></span>|<span data-ttu-id="40d68-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="40d68-112">**Element**</span></span>|<span data-ttu-id="40d68-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="40d68-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="40d68-114">**偽装**</span><span class="sxs-lookup"><span data-stu-id="40d68-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="40d68-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="40d68-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="40d68-116">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="40d68-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="40d68-117">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="40d68-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="40d68-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="40d68-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="40d68-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="40d68-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="40d68-120">RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="40d68-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="40d68-121">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="40d68-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="40d68-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="40d68-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="40d68-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="40d68-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="40d68-124">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="40d68-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="40d68-125">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="40d68-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="40d68-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="40d68-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="40d68-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="40d68-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="40d68-128">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="40d68-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="40d68-129">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="40d68-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="setimgroup-operation-request-example"></a><span data-ttu-id="40d68-130">SetImGroup 操作の要求の例</span><span class="sxs-lookup"><span data-stu-id="40d68-130">SetImGroup operation request example</span></span>

<span data-ttu-id="40d68-131">**SetImGroup**操作要求の次の例では、IM グループの表示名を"MyNewGroupName"に変更する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="40d68-131">The following example of a **SetImGroup** operation request shows how to change an IM group display name to "MyNewGroupName".</span></span> 
  
> [!NOTE]
> <span data-ttu-id="40d68-132">読みやすさを保持するために Exchange ストア id が小さすぎます。</span><span class="sxs-lookup"><span data-stu-id="40d68-132">The Exchange store identifier has been shortened to preserve readability.</span></span> 
  
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
      <m:SetImGroup>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkQoTbWAAAAAAQRAAA="
                    ChangeKey="EgAAAA=="/>
         <m:NewDisplayName>MyNewGroupName</m:NewDisplayName>
      </m:SetImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="40d68-133">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="40d68-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="40d68-134">SetImGroup</span><span class="sxs-lookup"><span data-stu-id="40d68-134">SetImGroup</span></span>](setimgroup.md)
    
- [<span data-ttu-id="40d68-135">グループ Id</span><span class="sxs-lookup"><span data-stu-id="40d68-135">GroupId</span></span>](groupid.md)
    
- [<span data-ttu-id="40d68-136">NewDisplayName</span><span class="sxs-lookup"><span data-stu-id="40d68-136">NewDisplayName</span></span>](newdisplayname.md)
    
## <a name="successful-setimgroup-operation-response"></a><span data-ttu-id="40d68-137">SetImGroup 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="40d68-137">Successful SetImGroup operation response</span></span>

<span data-ttu-id="40d68-138">成功した要求への応答、 **SetImGroup**操作の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="40d68-138">The following example shows a successful response to a **SetImGroup** operation request.</span></span> 
  
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
      <SetImGroupResponse ResponseClass="Success" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         </SetImGroupResponse>
      </s:Body>
</s:Envelope>
```

<span data-ttu-id="40d68-139">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="40d68-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="40d68-140">SetImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="40d68-140">SetImGroupResponse</span></span>](setimgroupresponse.md)
    
- [<span data-ttu-id="40d68-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="40d68-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="setimgroup-operation-error-response"></a><span data-ttu-id="40d68-142">SetImGroup 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="40d68-142">SetImGroup operation error response</span></span>

<span data-ttu-id="40d68-143">**SetImGroup**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="40d68-143">The following example shows an error response to a **SetImGroup** operation request.</span></span> <span data-ttu-id="40d68-144">次のエラー応答は、既存のグループの表示名とグループの表示名を変更しようとしましたがときに発生します。</span><span class="sxs-lookup"><span data-stu-id="40d68-144">The following error response occurs when an attempt is made to change the group display name to the existing group display name.</span></span> 
  
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
      <SetImGroupResponse ResponseClass="Error" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>An IM group with the specified display name already exists.</MessageText>
         <ResponseCode>ErrorImGroupDisplayNameAlreadyExists</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="40d68-145">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="40d68-145">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="40d68-146">SetImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="40d68-146">SetImGroupResponse</span></span>](setimgroupresponse.md)
    
- [<span data-ttu-id="40d68-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="40d68-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="40d68-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="40d68-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="40d68-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="40d68-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="40d68-150">EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="40d68-150">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="40d68-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="40d68-151">See also</span></span>

- [<span data-ttu-id="40d68-152">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="40d68-152">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="40d68-153">AddImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="40d68-153">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="40d68-154">RemoveImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="40d68-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    

