---
title: AddImGroup 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6df6e504-b7c8-4773-b10f-ffa5defac229
description: 操作 AddImGroup EWS についての情報を検索します。
ms.openlocfilehash: 91236f9ad2236b3f6bee600b9d57bcf736090ed7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759283"
---
# <a name="addimgroup-operation"></a><span data-ttu-id="1c128-103">AddImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="1c128-103">AddImGroup operation</span></span>

<span data-ttu-id="1c128-104">**AddImGroup** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="1c128-104">Find information about the **AddImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="1c128-105">**AddImGroup** Exchange Web サービス (EWS) の操作は、メールボックスに、新しいインスタント メッセージング (IM) グループを追加します。</span><span class="sxs-lookup"><span data-stu-id="1c128-105">The **AddImGroup** Exchange Web Services (EWS) operation adds a new instant messaging (IM) group to a mailbox.</span></span> 
  
<span data-ttu-id="1c128-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="1c128-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addimgroup-operation"></a><span data-ttu-id="1c128-107">AddImGroup 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="1c128-107">Using the AddImGroup operation</span></span>

<span data-ttu-id="1c128-108">**AddImGroup**操作には、単一の表示名の引数はわずかです。</span><span class="sxs-lookup"><span data-stu-id="1c128-108">The **AddImGroup** operation only takes a single display name argument.</span></span> 
  
<span data-ttu-id="1c128-109">この操作は、表示名、グループの種類、および新しいグループの Exchange ストアの識別子を返します。</span><span class="sxs-lookup"><span data-stu-id="1c128-109">This operation returns the display name, group type, and Exchange store identifier of the new group.</span></span>
  
<span data-ttu-id="1c128-110">**AddImGroup**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="1c128-110">The **AddImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="1c128-111">**表 1 です。AddImGroup 操作の SOAP ヘッダー**</span><span class="sxs-lookup"><span data-stu-id="1c128-111">**Table 1. AddImGroup operation SOAP headers**</span></span>

|<span data-ttu-id="1c128-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="1c128-112">**Header name**</span></span>|<span data-ttu-id="1c128-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="1c128-113">**Element**</span></span>|<span data-ttu-id="1c128-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="1c128-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="1c128-115">**偽装**</span><span class="sxs-lookup"><span data-stu-id="1c128-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="1c128-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="1c128-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="1c128-117">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="1c128-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="1c128-118">これは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="1c128-118">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1c128-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="1c128-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="1c128-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="1c128-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="1c128-121">RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="1c128-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="1c128-122">これは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="1c128-122">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1c128-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="1c128-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="1c128-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="1c128-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="1c128-125">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="1c128-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="1c128-126">これは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="1c128-126">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="1c128-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="1c128-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="1c128-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="1c128-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="1c128-129">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="1c128-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="1c128-130">これは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="1c128-130">This is applicable to a response.</span></span>  <br/> |
   
## <a name="addimgroup-operation-request-example-create-a-new-im-group"></a><span data-ttu-id="1c128-131">AddImGroup 操作の要求の例: IM グループの新規作成</span><span class="sxs-lookup"><span data-stu-id="1c128-131">AddImGroup operation request example: Create a new IM group</span></span>

<span data-ttu-id="1c128-132">**AddImGroup**操作要求の次の例では、MyCustomerGroup という名前の IM グループを作成する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="1c128-132">The following example of an **AddImGroup** operation request shows how to create an IM group named MyCustomerGroup.</span></span> 
  
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
      <m:AddImGroup>
         <m:DisplayName>MyCustomGroup</m:DisplayName>
      </m:AddImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="1c128-133">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1c128-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1c128-134">AddImGroup</span><span class="sxs-lookup"><span data-stu-id="1c128-134">AddImGroup</span></span>](addimgroup.md)
    
- [<span data-ttu-id="1c128-135">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="1c128-135">DisplayName (string)</span></span>](displayname-string.md)
    
## <a name="successful-addimgroup-operation-response"></a><span data-ttu-id="1c128-136">AddImGroup 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="1c128-136">Successful AddImGroup operation response</span></span>

<span data-ttu-id="1c128-137">**AddImGroup**操作の要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1c128-137">The following example shows a successful response to an **AddImGroup** operation request.</span></span> 
  
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
      <AddImGroupResponse ResponseClass="Success"
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImGroup>
            <DisplayName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">MyCustomGroup</DisplayName>
            <GroupType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">IPM.DistList.MOC.UserGroup</GroupType>
            <ExchangeStoreId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MAAA="
                             ChangeKey="EgAAAA=="
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/types"/>
         </ImGroup>
      </AddImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="1c128-138">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="1c128-138">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="1c128-139">AddImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="1c128-139">AddImGroupResponse</span></span>](addimgroupresponse.md)
    
- [<span data-ttu-id="1c128-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="1c128-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="1c128-141">ImGroup</span><span class="sxs-lookup"><span data-stu-id="1c128-141">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="1c128-142">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="1c128-142">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="1c128-143">GroupType</span><span class="sxs-lookup"><span data-stu-id="1c128-143">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="1c128-144">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="1c128-144">ExchangeStoreId</span></span>](exchangestoreid.md)
    
## <a name="addimgroup-operation-error-response"></a><span data-ttu-id="1c128-145">AddImGroup 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="1c128-145">AddImGroup operation error response</span></span>

<span data-ttu-id="1c128-146">**AddImGroup**操作要求に対するエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="1c128-146">The following example shows an error response to an **AddImGroup** operation request.</span></span> <span data-ttu-id="1c128-147">これは、表示名に使用できない文字が含まれる要求への応答です。</span><span class="sxs-lookup"><span data-stu-id="1c128-147">This is a response to a request that contains a character that cannot be used in a display name.</span></span> <span data-ttu-id="1c128-148">これが SOAP フォールトとスキーマ ・ ベースのエラー メッセージではないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="1c128-148">Note that this is a SOAP fault and not a schema-based error message.</span></span> <span data-ttu-id="1c128-149">要求で送信される表示名は、~! @# $% ^&amp;でエラーが発生し、&amp;の文字。</span><span class="sxs-lookup"><span data-stu-id="1c128-149">The display name submitted in the request is ~!@#$%^&amp;, and the error occurs on the &amp; character.</span></span> <span data-ttu-id="1c128-150">&amp;要求ペイロードの 11 行と 33rd の文字の文字が発生しました。</span><span class="sxs-lookup"><span data-stu-id="1c128-150">The &amp; character occurred on the 11th line and 33rd character in the request payload.</span></span> <span data-ttu-id="1c128-151">HTTP 500 コードで応答が返されました。</span><span class="sxs-lookup"><span data-stu-id="1c128-151">The response was returned with an HTTP 500 code.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="http://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
         <faultstring xml:lang="en-US">The request failed schema validation: An error occurred while parsing EntityName. Line 11, position 33.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
            <e:Message xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
            <t:MessageXml xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
               <t:LineNumber>11</t:LineNumber>
               <t:LinePosition>33</t:LinePosition>
               <t:Violation>An error occurred while parsing EntityName. Line 11, position 33.</t:Violation>
            </t:MessageXml>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="1c128-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="1c128-152">See also</span></span>

- [<span data-ttu-id="1c128-153">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="1c128-153">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="1c128-154">RemoveImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="1c128-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="1c128-155">SetImGroup</span><span class="sxs-lookup"><span data-stu-id="1c128-155">SetImGroup</span></span>](setimgroup.md)
    

