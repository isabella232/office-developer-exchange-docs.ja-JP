---
title: AddNewTelUriContactToGroup 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c9688ce8-2465-45bb-8bd2-94b32ed4885c
description: AddNewTelUriContactToGroup EWS 操作の使用方法に関する情報を検索します。
ms.openlocfilehash: 91228ec627ad928d2f1837c135af24846f811b1c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44464946"
---
# <a name="addnewteluricontacttogroup-operation"></a><span data-ttu-id="f3d63-103">AddNewTelUriContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="f3d63-103">AddNewTelUriContactToGroup operation</span></span>

<span data-ttu-id="f3d63-104">**AddNewTelUriContactToGroup** EWS 操作の使用方法に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="f3d63-104">Find information about how to use the **AddNewTelUriContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="f3d63-105">**AddNewTelUriContactToGroup**操作は、連絡先の電話番号に基づいてグループに新しい連絡先を追加します。</span><span class="sxs-lookup"><span data-stu-id="f3d63-105">The **AddNewTelUriContactToGroup** operation adds a new contact to a group based on a contact's phone number.</span></span> 
  
<span data-ttu-id="f3d63-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="f3d63-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addnewteluricontacttogroup-operation"></a><span data-ttu-id="f3d63-107">AddNewTelUriContactToGroup 操作の使用</span><span class="sxs-lookup"><span data-stu-id="f3d63-107">Using the AddNewTelUriContactToGroup operation</span></span>

<span data-ttu-id="f3d63-108">**AddNewTelUriContactToGroup**操作要求は、連絡先の TEL URI、SIP uri、電話番号、連絡先を追加するグループを送信します。</span><span class="sxs-lookup"><span data-stu-id="f3d63-108">An **AddNewTelUriContactToGroup** operation request submits a contact's TEL URI, SIP URI, phone number, and the group to add the contact to.</span></span> <span data-ttu-id="f3d63-109">**AddNewTelUriContactToGroup**操作の応答では、新しい連絡先のペルソナが作成されます。</span><span class="sxs-lookup"><span data-stu-id="f3d63-109">An **AddNewTelUriContactToGroup** operation response creates a persona for the new contact.</span></span> <span data-ttu-id="f3d63-110">この操作により、連絡先が名前を持たない場合でも、クライアントは新しい連絡先を追加できます。</span><span class="sxs-lookup"><span data-stu-id="f3d63-110">This operation allows clients to add a new contact even if the contact does not have a name.</span></span> 
  
### <a name="addnewteluricontacttogroup-operation-soap-headers"></a><span data-ttu-id="f3d63-111">AddNewTelUriContactToGroup 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f3d63-111">AddNewTelUriContactToGroup operation SOAP headers</span></span>

<span data-ttu-id="f3d63-112">**AddNewTelUriContactToGroup**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="f3d63-112">The **AddNewTelUriContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="f3d63-113">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="f3d63-113">**Header name**</span></span>|<span data-ttu-id="f3d63-114">**要素**</span><span class="sxs-lookup"><span data-stu-id="f3d63-114">**Element**</span></span>|<span data-ttu-id="f3d63-115">**説明**</span><span class="sxs-lookup"><span data-stu-id="f3d63-115">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="f3d63-116">**偽装**</span><span class="sxs-lookup"><span data-stu-id="f3d63-116">**Impersonation**</span></span> <br/> |[<span data-ttu-id="f3d63-117">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="f3d63-117">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="f3d63-118">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="f3d63-118">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="f3d63-119">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="f3d63-119">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="f3d63-120">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="f3d63-120">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="f3d63-121">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="f3d63-121">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="f3d63-122">RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。</span><span class="sxs-lookup"><span data-stu-id="f3d63-122">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="f3d63-123">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="f3d63-123">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="f3d63-124">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="f3d63-124">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="f3d63-125">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="f3d63-125">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="f3d63-126">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="f3d63-126">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="f3d63-127">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="f3d63-127">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="f3d63-128">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="f3d63-128">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="f3d63-129">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="f3d63-129">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="f3d63-130">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="f3d63-130">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="f3d63-131">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="f3d63-131">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addnewteluricontacttogroup-operation-request-example-add-a-new-contact-to-a-group"></a><span data-ttu-id="f3d63-132">AddNewTelUriContactToGroup 操作要求の例: 新しい連絡先をグループに追加します。</span><span class="sxs-lookup"><span data-stu-id="f3d63-132">AddNewTelUriContactToGroup operation request example: Add a new contact to a group</span></span>

<span data-ttu-id="f3d63-133">次の**AddNewTelUriContactToGroup**操作要求の例は、連絡先の TEL および SIP uri を使用して、新しい連絡先を作成し、インスタントメッセージング (IM) グループに新しい連絡先を追加する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="f3d63-133">The following example of an **AddNewTelUriContactToGroup** operation request shows how to create a new contact and add the new contact to an instant messaging (IM) group by using the contact's TEL and SIP URIs.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="f3d63-134">この記事のすべてのアイテム識別子と変更キーは、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="f3d63-134">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
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
      <m:AddNewTelUriContactToGroup>
         <m:TelUriAddress>tel:5625550100</m:TelUriAddress>
         <m:ImContactSipUriAddress>sip:john@contoso.com</m:ImContactSipUriAddress>
         <m:ImTelephoneNumber>5625550100</m:ImTelephoneNumber>
         <m:GroupId Id="AAMkADEzOTm4QrAABY7+0GAAA="/>
      </m:AddNewTelUriContactToGroup>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="f3d63-135">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3d63-135">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="f3d63-136">AddNewTelUriContactToGroup</span><span class="sxs-lookup"><span data-stu-id="f3d63-136">AddNewTelUriContactToGroup</span></span>](addnewteluricontacttogroup.md)
    
- [<span data-ttu-id="f3d63-137">TelUriAddress</span><span class="sxs-lookup"><span data-stu-id="f3d63-137">TelUriAddress</span></span>](teluriaddress.md)
    
- [<span data-ttu-id="f3d63-138">Imcontactsi紫 Iaddress</span><span class="sxs-lookup"><span data-stu-id="f3d63-138">ImContactSipUriAddress</span></span>](imcontactsipuriaddress.md)
    
- [<span data-ttu-id="f3d63-139">ImTelephoneNumber</span><span class="sxs-lookup"><span data-stu-id="f3d63-139">ImTelephoneNumber</span></span>](imtelephonenumber.md)
    
- [<span data-ttu-id="f3d63-140">GroupId</span><span class="sxs-lookup"><span data-stu-id="f3d63-140">GroupId</span></span>](groupid.md)
    
## <a name="successful-addnewteluricontacttogroup-operation-response"></a><span data-ttu-id="f3d63-141">成功した AddNewTelUriContactToGroup 操作の応答</span><span class="sxs-lookup"><span data-stu-id="f3d63-141">Successful AddNewTelUriContactToGroup operation response</span></span>

<span data-ttu-id="f3d63-142">次の例は、連絡先を作成するための**AddNewTelUriContactToGroup**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="f3d63-142">The following example shows a successful response to an **AddNewTelUriContactToGroup** operation request to create a contact.</span></span> <span data-ttu-id="f3d63-143">応答には、連絡先の関連付けられたペルソナ識別子、この例では連絡先の電話番号に基づき、連絡先のアイテムの識別子が含まれています。これは、送信元識別子の一部として表示されます。</span><span class="sxs-lookup"><span data-stu-id="f3d63-143">The response contains the associated persona identifier for the contact, the display name of the persona, which in this case is based on the contact's phone number, and the contact's item identifier, which is displayed as part of the source identifier attribution.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/"                           
            xmlns:xsd="http://www.w3.org/2001/XMLSchema"
            xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
            xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
   </s:Header>
   <s:Body>
      <AddNewTelUriContactToGroupResponse ResponseClass="Success" 
                                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

<span data-ttu-id="f3d63-144">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3d63-144">The response SOAP body contains following elements:</span></span>
  
- [<span data-ttu-id="f3d63-145">AddNewTelUriContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="f3d63-145">AddNewTelUriContactToGroupResponse</span></span>](addnewteluricontacttogroupresponse.md)
    
- [<span data-ttu-id="f3d63-146">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f3d63-146">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f3d63-147">ユーザー</span><span class="sxs-lookup"><span data-stu-id="f3d63-147">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="f3d63-148">PersonaId</span><span class="sxs-lookup"><span data-stu-id="f3d63-148">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="f3d63-149">個人の Atype</span><span class="sxs-lookup"><span data-stu-id="f3d63-149">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="f3d63-150">CreationTime</span><span class="sxs-lookup"><span data-stu-id="f3d63-150">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="f3d63-151">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="f3d63-151">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="f3d63-152">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="f3d63-152">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="f3d63-153">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="f3d63-153">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="f3d63-154">FileAs</span><span class="sxs-lookup"><span data-stu-id="f3d63-154">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="f3d63-155">FileAsId</span><span class="sxs-lookup"><span data-stu-id="f3d63-155">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="f3d63-156">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="f3d63-156">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="f3d63-157">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="f3d63-157">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="f3d63-158">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="f3d63-158">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="f3d63-159">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="f3d63-159">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="f3d63-160">SourceId</span><span class="sxs-lookup"><span data-stu-id="f3d63-160">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="f3d63-161">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="f3d63-161">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="f3d63-162">IsWritable 可能</span><span class="sxs-lookup"><span data-stu-id="f3d63-162">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="f3d63-163">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="f3d63-163">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="f3d63-164">IsHidden</span><span class="sxs-lookup"><span data-stu-id="f3d63-164">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="f3d63-165">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="f3d63-165">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="f3d63-166">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="f3d63-166">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="f3d63-167">値</span><span class="sxs-lookup"><span data-stu-id="f3d63-167">Value</span></span>](value.md)
    
- [<span data-ttu-id="f3d63-168">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="f3d63-168">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="f3d63-169">属性 (string)</span><span class="sxs-lookup"><span data-stu-id="f3d63-169">Attribution (string)</span></span>](attribution-string.md)
    
- [<span data-ttu-id="f3d63-170">OtherTelephones</span><span class="sxs-lookup"><span data-stu-id="f3d63-170">OtherTelephones</span></span>](othertelephones.md)
    
- [<span data-ttu-id="f3d63-171">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="f3d63-171">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="f3d63-172">値</span><span class="sxs-lookup"><span data-stu-id="f3d63-172">Value</span></span>](value.md)
    
- [<span data-ttu-id="f3d63-173">Number</span><span class="sxs-lookup"><span data-stu-id="f3d63-173">Number</span></span>](number.md)
    
- [<span data-ttu-id="f3d63-174">型 (string)</span><span class="sxs-lookup"><span data-stu-id="f3d63-174">Type (string)</span></span>](type-string.md)
    
- [<span data-ttu-id="f3d63-175">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="f3d63-175">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="f3d63-176">属性 (string)</span><span class="sxs-lookup"><span data-stu-id="f3d63-176">Attribution (string)</span></span>](attribution-string.md)
    
## <a name="addnewteluricontacttogroup-operation-error-response-example"></a><span data-ttu-id="f3d63-177">AddNewTelUriContactToGroup 操作エラー応答の例</span><span class="sxs-lookup"><span data-stu-id="f3d63-177">AddNewTelUriContactToGroup operation error response example</span></span>

<span data-ttu-id="f3d63-178">次の例は、グループ識別子に、メールボックス内のグループを識別しない整形式の値が含まれている場合の、 **AddNewTelUriContactToGroup**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="f3d63-178">The following example shows an error response to an **AddNewTelUriContactToGroup** operation request when the group identifier contains a well-formed value that does not identify a group in the mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="545" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddNewTelUriContactToGroupResponse ResponseClass="Error" 
                                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>The specified object was not found in the store.</MessageText>
         <ResponseCode>ErrorItemNotFound</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </AddNewTelUriContactToGroupResponse>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="f3d63-179">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="f3d63-179">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="f3d63-180">AddNewTelUriContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="f3d63-180">AddNewTelUriContactToGroupResponse</span></span>](addnewteluricontacttogroupresponse.md)
    
- [<span data-ttu-id="f3d63-181">MessageText</span><span class="sxs-lookup"><span data-stu-id="f3d63-181">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="f3d63-182">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="f3d63-182">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="f3d63-183">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="f3d63-183">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
## <a name="see-also"></a><span data-ttu-id="f3d63-184">関連項目</span><span class="sxs-lookup"><span data-stu-id="f3d63-184">See also</span></span>

- [<span data-ttu-id="f3d63-185">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="f3d63-185">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="f3d63-186">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="f3d63-186">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    

