---
title: SetImGroup 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 2d48aa07-8152-4c3d-a519-061253e80174
description: SetImGroup EWS 操作に関する情報を検索します。
ms.openlocfilehash: 37b290559fff0b2de57669741547ba4b1b56c28c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44438076"
---
# <a name="setimgroup-operation"></a><span data-ttu-id="de429-103">SetImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="de429-103">SetImGroup operation</span></span>

<span data-ttu-id="de429-104">**Setimgroup** EWS 操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="de429-104">Find information about the **SetImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="de429-105">**Setimgroup**操作は、インスタントメッセージング (IM) グループの表示名を変更します。</span><span class="sxs-lookup"><span data-stu-id="de429-105">The **SetImGroup** operation changes the display name of an instant messaging (IM) group.</span></span> 
  
<span data-ttu-id="de429-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="de429-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-setimgroup-operation"></a><span data-ttu-id="de429-107">SetImGroup 操作の使用</span><span class="sxs-lookup"><span data-stu-id="de429-107">Using the SetImGroup operation</span></span>

<span data-ttu-id="de429-108">**Setimgroup**操作は、1つの表示名の引数のみを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="de429-108">The **SetImGroup** operation only takes a single display name argument.</span></span> 
  
### <a name="setimgroup-operation-soap-headers"></a><span data-ttu-id="de429-109">SetImGroup 操作 SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="de429-109">SetImGroup operation SOAP headers</span></span>

<span data-ttu-id="de429-110">**Setimgroup**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="de429-110">The **SetImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="de429-111">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="de429-111">**Header name**</span></span>|<span data-ttu-id="de429-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="de429-112">**Element**</span></span>|<span data-ttu-id="de429-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="de429-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="de429-114">**偽装**</span><span class="sxs-lookup"><span data-stu-id="de429-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="de429-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="de429-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="de429-116">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="de429-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="de429-117">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="de429-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="de429-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="de429-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="de429-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="de429-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="de429-120">RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。</span><span class="sxs-lookup"><span data-stu-id="de429-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="de429-121">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="de429-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="de429-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="de429-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="de429-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="de429-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="de429-124">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="de429-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="de429-125">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="de429-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="de429-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="de429-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="de429-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="de429-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="de429-128">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="de429-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="de429-129">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="de429-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="setimgroup-operation-request-example"></a><span data-ttu-id="de429-130">SetImGroup 操作要求の例</span><span class="sxs-lookup"><span data-stu-id="de429-130">SetImGroup operation request example</span></span>

<span data-ttu-id="de429-131">**Setimgroup**操作要求の次の例は、IM グループの表示名を "MyNewGroupName" に変更する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="de429-131">The following example of a **SetImGroup** operation request shows how to change an IM group display name to "MyNewGroupName".</span></span> 
  
> [!NOTE]
> <span data-ttu-id="de429-132">読みやすくするために、Exchange ストア識別子が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="de429-132">The Exchange store identifier has been shortened to preserve readability.</span></span> 
  
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
      <m:SetImGroup>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkQoTbWAAAAAAQRAAA="
                    ChangeKey="EgAAAA=="/>
         <m:NewDisplayName>MyNewGroupName</m:NewDisplayName>
      </m:SetImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="de429-133">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de429-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="de429-134">SetImGroup</span><span class="sxs-lookup"><span data-stu-id="de429-134">SetImGroup</span></span>](setimgroup.md)
    
- [<span data-ttu-id="de429-135">GroupId</span><span class="sxs-lookup"><span data-stu-id="de429-135">GroupId</span></span>](groupid.md)
    
- [<span data-ttu-id="de429-136">NewDisplayName</span><span class="sxs-lookup"><span data-stu-id="de429-136">NewDisplayName</span></span>](newdisplayname.md)
    
## <a name="successful-setimgroup-operation-response"></a><span data-ttu-id="de429-137">SetImGroup 操作応答の成功</span><span class="sxs-lookup"><span data-stu-id="de429-137">Successful SetImGroup operation response</span></span>

<span data-ttu-id="de429-138">次の例は、 **Setimgroup**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="de429-138">The following example shows a successful response to a **SetImGroup** operation request.</span></span> 
  
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
      <SetImGroupResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         </SetImGroupResponse>
      </s:Body>
</s:Envelope>
```

<span data-ttu-id="de429-139">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de429-139">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="de429-140">SetImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="de429-140">SetImGroupResponse</span></span>](setimgroupresponse.md)
    
- [<span data-ttu-id="de429-141">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="de429-141">ResponseCode</span></span>](responsecode.md)
    
## <a name="setimgroup-operation-error-response"></a><span data-ttu-id="de429-142">SetImGroup 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="de429-142">SetImGroup operation error response</span></span>

<span data-ttu-id="de429-143">次の例は、 **Setimgroup**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="de429-143">The following example shows an error response to a **SetImGroup** operation request.</span></span> <span data-ttu-id="de429-144">グループの表示名を既存のグループの表示名に変更しようとすると、次のエラーが返されます。</span><span class="sxs-lookup"><span data-stu-id="de429-144">The following error response occurs when an attempt is made to change the group display name to the existing group display name.</span></span> 
  
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
      <SetImGroupResponse ResponseClass="Error" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>An IM group with the specified display name already exists.</MessageText>
         <ResponseCode>ErrorImGroupDisplayNameAlreadyExists</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </SetImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="de429-145">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="de429-145">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="de429-146">SetImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="de429-146">SetImGroupResponse</span></span>](setimgroupresponse.md)
    
- [<span data-ttu-id="de429-147">MessageText</span><span class="sxs-lookup"><span data-stu-id="de429-147">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="de429-148">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="de429-148">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="de429-149">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="de429-149">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="de429-150">EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)</span><span class="sxs-lookup"><span data-stu-id="de429-150">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="de429-151">関連項目</span><span class="sxs-lookup"><span data-stu-id="de429-151">See also</span></span>

- [<span data-ttu-id="de429-152">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="de429-152">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="de429-153">AddImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="de429-153">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="de429-154">RemoveImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="de429-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    

