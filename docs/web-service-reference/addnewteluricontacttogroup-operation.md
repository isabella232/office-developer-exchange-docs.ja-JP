---
title: AddNewTelUriContactToGroup 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9688ce8-2465-45bb-8bd2-94b32ed4885c
description: EWS の AddNewTelUriContactToGroup 操作を使用する方法に関する情報を検索します。
ms.openlocfilehash: 34450171776b4215d9c0a39700a309e2e2d755dd
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19759294"
---
# <a name="addnewteluricontacttogroup-operation"></a><span data-ttu-id="0ba09-103">AddNewTelUriContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="0ba09-103">AddNewTelUriContactToGroup operation</span></span>

<span data-ttu-id="0ba09-104">**AddNewTelUriContactToGroup** EWS の操作を使用する方法に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="0ba09-104">Find information about how to use the **AddNewTelUriContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="0ba09-105">**AddNewTelUriContactToGroup**操作は、連絡先の電話番号に基づいたグループに新しい連絡先を追加します。</span><span class="sxs-lookup"><span data-stu-id="0ba09-105">The **AddNewTelUriContactToGroup** operation adds a new contact to a group based on a contact's phone number.</span></span> 
  
<span data-ttu-id="0ba09-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="0ba09-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addnewteluricontacttogroup-operation"></a><span data-ttu-id="0ba09-107">AddNewTelUriContactToGroup 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="0ba09-107">Using the AddNewTelUriContactToGroup operation</span></span>

<span data-ttu-id="0ba09-108">**AddNewTelUriContactToGroup**操作要求では、連絡先を追加する連絡先の電話の URI、SIP URI、電話番号、およびグループを送信します。</span><span class="sxs-lookup"><span data-stu-id="0ba09-108">An **AddNewTelUriContactToGroup** operation request submits a contact's TEL URI, SIP URI, phone number, and the group to add the contact to.</span></span> <span data-ttu-id="0ba09-109">**AddNewTelUriContactToGroup**の操作の応答は、新しい連絡先のペルソナを作成します。</span><span class="sxs-lookup"><span data-stu-id="0ba09-109">An **AddNewTelUriContactToGroup** operation response creates a persona for the new contact.</span></span> <span data-ttu-id="0ba09-110">この操作では、取引先担当者が名前を持っていない場合でも、新しい連絡先を追加するのにはクライアントを許可します。</span><span class="sxs-lookup"><span data-stu-id="0ba09-110">This operation allows clients to add a new contact even if the contact does not have a name.</span></span> 
  
### <a name="addnewteluricontacttogroup-operation-soap-headers"></a><span data-ttu-id="0ba09-111">AddNewTelUriContactToGroup 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0ba09-111">AddNewTelUriContactToGroup operation SOAP headers</span></span>

<span data-ttu-id="0ba09-112">**AddNewTelUriContactToGroup**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="0ba09-112">The **AddNewTelUriContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="0ba09-113">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="0ba09-113">**Header name**</span></span>|<span data-ttu-id="0ba09-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="0ba09-114">**Element**</span></span>|<span data-ttu-id="0ba09-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="0ba09-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0ba09-116">**偽装**</span><span class="sxs-lookup"><span data-stu-id="0ba09-116">**Impersonation**</span></span> <br/> |[<span data-ttu-id="0ba09-117">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="0ba09-117">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="0ba09-118">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="0ba09-118">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="0ba09-119">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0ba09-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0ba09-120">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="0ba09-120">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="0ba09-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="0ba09-121">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="0ba09-122">RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="0ba09-122">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="0ba09-123">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0ba09-123">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0ba09-124">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="0ba09-124">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="0ba09-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="0ba09-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="0ba09-126">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="0ba09-126">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="0ba09-127">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0ba09-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="0ba09-128">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="0ba09-128">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="0ba09-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0ba09-129">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="0ba09-130">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="0ba09-130">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="0ba09-131">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="0ba09-131">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addnewteluricontacttogroup-operation-request-example-add-a-new-contact-to-a-group"></a><span data-ttu-id="0ba09-132">AddNewTelUriContactToGroup 操作の要求の例: 新しい連絡先をグループに追加します。</span><span class="sxs-lookup"><span data-stu-id="0ba09-132">AddNewTelUriContactToGroup operation request example: Add a new contact to a group</span></span>

<span data-ttu-id="0ba09-133">**AddNewTelUriContactToGroup**操作要求の次の例では、新しい連絡先を作成し、インスタント メッセージング (IM) グループに連絡先の電話と SIP Uri を使用して新しい連絡先を追加する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="0ba09-133">The following example of an **AddNewTelUriContactToGroup** operation request shows how to create a new contact and add the new contact to an instant messaging (IM) group by using the contact's TEL and SIP URIs.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="0ba09-134">すべての項目の識別子と変更キーをこの資料では、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="0ba09-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
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
      <m:AddNewTelUriContactToGroup>
         <m:TelUriAddress>tel:5625550100</m:TelUriAddress>
         <m:ImContactSipUriAddress>sip:john@contoso.com</m:ImContactSipUriAddress>
         <m:ImTelephoneNumber>5625550100</m:ImTelephoneNumber>
         <m:GroupId Id="AAMkADEzOTm4QrAABY7+0GAAA="/>
      </m:AddNewTelUriContactToGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="0ba09-135">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0ba09-135">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0ba09-136">AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="0ba09-136">AddNewTelUriContactToGroup</span></span>](addnewteluricontacttogroup.md)
    
- [<span data-ttu-id="0ba09-137">TelUriAddress</span><span class="sxs-lookup"><span data-stu-id="0ba09-137">TelUriAddress</span></span>](teluriaddress.md)
    
- [<span data-ttu-id="0ba09-138">ImContactSipUriAddress</span><span class="sxs-lookup"><span data-stu-id="0ba09-138">ImContactSipUriAddress</span></span>](imcontactsipuriaddress.md)
    
- [<span data-ttu-id="0ba09-139">ImTelephoneNumber</span><span class="sxs-lookup"><span data-stu-id="0ba09-139">ImTelephoneNumber</span></span>](imtelephonenumber.md)
    
- [<span data-ttu-id="0ba09-140">グループ Id</span><span class="sxs-lookup"><span data-stu-id="0ba09-140">GroupId</span></span>](groupid.md)
    
## <a name="successful-addnewteluricontacttogroup-operation-response"></a><span data-ttu-id="0ba09-141">AddNewTelUriContactToGroup 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="0ba09-141">Successful AddNewTelUriContactToGroup operation response</span></span>

<span data-ttu-id="0ba09-142">次の例では、連絡先を作成するのには、 **AddNewTelUriContactToGroup**操作の要求に正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="0ba09-142">The following example shows a successful response to an **AddNewTelUriContactToGroup** operation request to create a contact.</span></span> <span data-ttu-id="0ba09-143">応答には、連絡先の関連付けられているペルソナの識別子、連絡先の電話番号に基づく場合、ペルソナ、およびソースの識別子の属性の一部として表示される連絡先の項目の識別子の表示名が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0ba09-143">The response contains the associated persona identifier for the contact, the display name of the persona, which in this case is based on the contact's phone number, and the contact's item identifier, which is displayed as part of the source identifier attribution.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"                           
            xmlns:xsd="http://www.w3.org/2001/XMLSchema"
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
            xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" />
   </s:Header>
   <s:Body>
      <AddNewTelUriContactToGroupResponse ResponseClass="Success" 
                                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <Persona>
            <t:PersonaId Id="AAQkADE686dX3s="/>
            <t:PersonaType>Person</t:PersonaType>
            <t:CreationTime>2012-10-29T23:10:13Z</t:CreationTime>
            <t:DisplayName/>
            <t:DisplayNameFirstLast>5625550100</t:DisplayNameFirstLast>
            <t:DisplayNameLastFirst>5625550100</t:DisplayNameLastFirst>
            <t:FileAs/>
            <t:FileAsId >None</t:FileAsId>
            <t:RelevanceScore >2147483647</t:RelevanceScore>
            <t:Attributions>
               <t:Attribution>
                  <t:Id>0</t:Id>
                  <t:SourceId Id="ABhHuhCAAA=" ChangeKey="EQAAABxFU"/>
                  <t:DisplayName>Lync Contacts</t:DisplayName>
                  <t:IsWritable>false</t:IsWritable>
                  <t:IsQuickContact>true</t:IsQuickContact>
                  <t:IsHidden>false</t:IsHidden>
               </t:Attribution>
            </t:Attributions>
            <t:FileAsIds>
               <t:StringAttributedValue>
                  <t:Value>None</t:Value>
                  <t:Attributions>
                     <t:Attribution>0</t:Attribution>
                  </t:Attributions>
               </t:StringAttributedValue>
            </t:FileAsIds>
            <t:OtherTelephones>
               <t:PhoneNumberAttributedValue>
                  <t:Value>
                     <t:Number>5625550100</t:Number>
                     <t:Type>Other</t:Type>
                  </t:Value>
                  <t:Attributions>
                     <t:Attribution>0</t:Attribution>
                  </t:Attributions>
               </t:PhoneNumberAttributedValue>
            </t:OtherTelephones>
         </Persona>
      </AddNewTelUriContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="0ba09-144">応答 SOAP 本文は、次の要素含まれています。</span><span class="sxs-lookup"><span data-stu-id="0ba09-144">The response SOAP body contains following elements:</span></span>
  
- [<span data-ttu-id="0ba09-145">AddNewTelUriContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="0ba09-145">AddNewTelUriContactToGroupResponse</span></span>](addnewteluricontacttogroupresponse.md)
    
- [<span data-ttu-id="0ba09-146">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0ba09-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0ba09-147">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="0ba09-147">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="0ba09-148">PersonaId</span><span class="sxs-lookup"><span data-stu-id="0ba09-148">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="0ba09-149">PersonaType</span><span class="sxs-lookup"><span data-stu-id="0ba09-149">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="0ba09-150">CreationTime</span><span class="sxs-lookup"><span data-stu-id="0ba09-150">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="0ba09-151">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="0ba09-151">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="0ba09-152">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="0ba09-152">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="0ba09-153">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="0ba09-153">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="0ba09-154">表題</span><span class="sxs-lookup"><span data-stu-id="0ba09-154">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="0ba09-155">FileAsId</span><span class="sxs-lookup"><span data-stu-id="0ba09-155">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="0ba09-156">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="0ba09-156">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="0ba09-157">帰属 (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="0ba09-157">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="0ba09-158">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="0ba09-158">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="0ba09-159">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="0ba09-159">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="0ba09-160">SourceId</span><span class="sxs-lookup"><span data-stu-id="0ba09-160">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="0ba09-161">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="0ba09-161">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="0ba09-162">IsWritable</span><span class="sxs-lookup"><span data-stu-id="0ba09-162">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="0ba09-163">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="0ba09-163">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="0ba09-164">IsHidden</span><span class="sxs-lookup"><span data-stu-id="0ba09-164">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="0ba09-165">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="0ba09-165">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="0ba09-166">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="0ba09-166">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="0ba09-167">値</span><span class="sxs-lookup"><span data-stu-id="0ba09-167">Value</span></span>](value.md)
    
- [<span data-ttu-id="0ba09-168">帰属 (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="0ba09-168">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="0ba09-169">属性 (文字列)</span><span class="sxs-lookup"><span data-stu-id="0ba09-169">Attribution (string)</span></span>](attribution-string.md)
    
- [<span data-ttu-id="0ba09-170">OtherTelephones</span><span class="sxs-lookup"><span data-stu-id="0ba09-170">OtherTelephones</span></span>](othertelephones.md)
    
- [<span data-ttu-id="0ba09-171">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="0ba09-171">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="0ba09-172">値</span><span class="sxs-lookup"><span data-stu-id="0ba09-172">Value</span></span>](value.md)
    
- [<span data-ttu-id="0ba09-173">Number</span><span class="sxs-lookup"><span data-stu-id="0ba09-173">Number</span></span>](number.md)
    
- [<span data-ttu-id="0ba09-174">型 (文字列)</span><span class="sxs-lookup"><span data-stu-id="0ba09-174">Type (string)</span></span>](type-string.md)
    
- [<span data-ttu-id="0ba09-175">帰属 (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="0ba09-175">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="0ba09-176">属性 (文字列)</span><span class="sxs-lookup"><span data-stu-id="0ba09-176">Attribution (string)</span></span>](attribution-string.md)
    
## <a name="addnewteluricontacttogroup-operation-error-response-example"></a><span data-ttu-id="0ba09-177">AddNewTelUriContactToGroup 操作のエラー応答の例</span><span class="sxs-lookup"><span data-stu-id="0ba09-177">AddNewTelUriContactToGroup operation error response example</span></span>

<span data-ttu-id="0ba09-178">グループ識別子には、メールボックス内のグループを示していない整形式の値が含まれている場合、次の使用例は**AddNewTelUriContactToGroup**操作要求に対するエラー応答を示します。</span><span class="sxs-lookup"><span data-stu-id="0ba09-178">The following example shows an error response to an **AddNewTelUriContactToGroup** operation request when the group identifier contains a well-formed value that does not identify a group in the mailbox.</span></span> 
  
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
      <AddNewTelUriContactToGroupResponse ResponseClass="Error" 
                                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddNewTelUriContactToGroupResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="0ba09-179">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0ba09-179">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="0ba09-180">AddNewTelUriContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="0ba09-180">AddNewTelUriContactToGroupResponse</span></span>](addnewteluricontacttogroupresponse.md)
    
- [<span data-ttu-id="0ba09-181">MessageText</span><span class="sxs-lookup"><span data-stu-id="0ba09-181">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="0ba09-182">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="0ba09-182">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="0ba09-183">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="0ba09-183">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="0ba09-184">関連項目</span><span class="sxs-lookup"><span data-stu-id="0ba09-184">See also</span></span>

- [<span data-ttu-id="0ba09-185">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="0ba09-185">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="0ba09-186">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="0ba09-186">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

