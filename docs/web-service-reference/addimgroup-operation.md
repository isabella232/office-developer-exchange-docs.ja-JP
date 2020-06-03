---
title: AddImGroup 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 6df6e504-b7c8-4773-b10f-ffa5defac229
description: AddImGroup EWS 操作についての情報を検索します。
ms.openlocfilehash: 38ed12a741d46fe998dc0079ed13973ce9edf5ac
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462816"
---
# <a name="addimgroup-operation"></a><span data-ttu-id="3fc2c-103">AddImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="3fc2c-103">AddImGroup operation</span></span>

<span data-ttu-id="3fc2c-104">**Addimgroup** EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-104">Find information about the **AddImGroup** EWS operation.</span></span> 
  
<span data-ttu-id="3fc2c-105">**Addimgroup** Exchange Web サービス (EWS) の操作によって、新しいインスタントメッセージング (IM) グループがメールボックスに追加されます。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-105">The **AddImGroup** Exchange Web Services (EWS) operation adds a new instant messaging (IM) group to a mailbox.</span></span> 
  
<span data-ttu-id="3fc2c-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addimgroup-operation"></a><span data-ttu-id="3fc2c-107">AddImGroup 操作の使用</span><span class="sxs-lookup"><span data-stu-id="3fc2c-107">Using the AddImGroup operation</span></span>

<span data-ttu-id="3fc2c-108">**Addimgroup**操作は、1つの表示名の引数のみを受け取ります。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-108">The **AddImGroup** operation only takes a single display name argument.</span></span> 
  
<span data-ttu-id="3fc2c-109">この操作は、新しいグループの表示名、グループの種類、および Exchange ストア識別子を返します。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-109">This operation returns the display name, group type, and Exchange store identifier of the new group.</span></span>
  
<span data-ttu-id="3fc2c-110">**Addimgroup**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-110">The **AddImGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
<span data-ttu-id="3fc2c-111">**表1AddImGroup 操作 SOAP ヘッダー**</span><span class="sxs-lookup"><span data-stu-id="3fc2c-111">**Table 1. AddImGroup operation SOAP headers**</span></span>

|<span data-ttu-id="3fc2c-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="3fc2c-112">**Header name**</span></span>|<span data-ttu-id="3fc2c-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="3fc2c-113">**Element**</span></span>|<span data-ttu-id="3fc2c-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="3fc2c-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="3fc2c-115">**偽装**</span><span class="sxs-lookup"><span data-stu-id="3fc2c-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="3fc2c-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="3fc2c-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="3fc2c-117">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="3fc2c-118">これは要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-118">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3fc2c-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="3fc2c-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="3fc2c-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="3fc2c-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="3fc2c-121">RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="3fc2c-122">これは要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-122">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3fc2c-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="3fc2c-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="3fc2c-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="3fc2c-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="3fc2c-125">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="3fc2c-126">これは要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-126">This is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="3fc2c-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="3fc2c-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="3fc2c-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="3fc2c-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="3fc2c-129">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="3fc2c-130">これは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-130">This is applicable to a response.</span></span>  <br/> |
   
## <a name="addimgroup-operation-request-example-create-a-new-im-group"></a><span data-ttu-id="3fc2c-131">AddImGroup 操作要求の例: 新しい IM グループを作成します。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-131">AddImGroup operation request example: Create a new IM group</span></span>

<span data-ttu-id="3fc2c-132">次に示す**Addimgroup**操作要求の例は、My顧客グループという名前の IM グループを作成する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-132">The following example of an **AddImGroup** operation request shows how to create an IM group named MyCustomerGroup.</span></span> 
  
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
      <m:AddImGroup>
         <m:DisplayName>MyCustomGroup</m:DisplayName>
      </m:AddImGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="3fc2c-133">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-133">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3fc2c-134">AddImGroup</span><span class="sxs-lookup"><span data-stu-id="3fc2c-134">AddImGroup</span></span>](addimgroup.md)
    
- [<span data-ttu-id="3fc2c-135">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="3fc2c-135">DisplayName (string)</span></span>](displayname-string.md)
    
## <a name="successful-addimgroup-operation-response"></a><span data-ttu-id="3fc2c-136">正常な AddImGroup 操作の応答</span><span class="sxs-lookup"><span data-stu-id="3fc2c-136">Successful AddImGroup operation response</span></span>

<span data-ttu-id="3fc2c-137">次の例は、 **Addimgroup**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-137">The following example shows a successful response to an **AddImGroup** operation request.</span></span> 
  
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
      <AddImGroupResponse ResponseClass="Success"
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImGroup>
            <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">MyCustomGroup</DisplayName>
            <GroupType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">IPM.DistList.MOC.UserGroup</GroupType>
            <ExchangeStoreId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MAAA="
                             ChangeKey="EgAAAA=="
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/types"/>
         </ImGroup>
      </AddImGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="3fc2c-138">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-138">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="3fc2c-139">AddImGroupResponse</span><span class="sxs-lookup"><span data-stu-id="3fc2c-139">AddImGroupResponse</span></span>](addimgroupresponse.md)
    
- [<span data-ttu-id="3fc2c-140">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="3fc2c-140">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="3fc2c-141">ImGroup</span><span class="sxs-lookup"><span data-stu-id="3fc2c-141">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="3fc2c-142">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="3fc2c-142">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="3fc2c-143">GroupType</span><span class="sxs-lookup"><span data-stu-id="3fc2c-143">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="3fc2c-144">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="3fc2c-144">ExchangeStoreId</span></span>](exchangestoreid.md)
    
## <a name="addimgroup-operation-error-response"></a><span data-ttu-id="3fc2c-145">AddImGroup 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="3fc2c-145">AddImGroup operation error response</span></span>

<span data-ttu-id="3fc2c-146">次の例は、 **Addimgroup**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-146">The following example shows an error response to an **AddImGroup** operation request.</span></span> <span data-ttu-id="3fc2c-147">これは、表示名に使用できない文字を含む要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-147">This is a response to a request that contains a character that cannot be used in a display name.</span></span> <span data-ttu-id="3fc2c-148">これは SOAP フォールトであり、スキーマベースのエラーメッセージではないことに注意してください。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-148">Note that this is a SOAP fault and not a schema-based error message.</span></span> <span data-ttu-id="3fc2c-149">要求で送信された表示名は ~! @ # $% ^ &amp; で、文字にエラーが発生し &amp; ます。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-149">The display name submitted in the request is ~!@#$%^&amp;, and the error occurs on the &amp; character.</span></span> <span data-ttu-id="3fc2c-150">&amp;11 行目と要求ペイロードの3番目の文字の文字が発生しました。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-150">The &amp; character occurred on the 11th line and 33rd character in the request payload.</span></span> <span data-ttu-id="3fc2c-151">HTTP 500 コードを使用して応答が返されました。</span><span class="sxs-lookup"><span data-stu-id="3fc2c-151">The response was returned with an HTTP 500 code.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="https://schemas.microsoft.com/exchange/services/2006/types">a:ErrorSchemaValidation</faultcode>
         <faultstring xml:lang="en-US">The request failed schema validation: An error occurred while parsing EntityName. Line 11, position 33.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorSchemaValidation</e:ResponseCode>
            <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The request failed schema validation.</e:Message>
            <t:MessageXml xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
               <t:LineNumber>11</t:LineNumber>
               <t:LinePosition>33</t:LinePosition>
               <t:Violation>An error occurred while parsing EntityName. Line 11, position 33.</t:Violation>
            </t:MessageXml>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="3fc2c-152">関連項目</span><span class="sxs-lookup"><span data-stu-id="3fc2c-152">See also</span></span>

- [<span data-ttu-id="3fc2c-153">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="3fc2c-153">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="3fc2c-154">RemoveImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="3fc2c-154">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
    
- [<span data-ttu-id="3fc2c-155">SetImGroup</span><span class="sxs-lookup"><span data-stu-id="3fc2c-155">SetImGroup</span></span>](setimgroup.md)
    

