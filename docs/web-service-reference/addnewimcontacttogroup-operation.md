---
title: AddNewImContactToGroup 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 0cb5525f-faa3-48f1-9551-df55ffc26f46
description: AddNewImContactToGroup EWS 操作についての情報を検索します。
ms.openlocfilehash: e91cc067b4161b366e6713a9adc16873e63b1562
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44465030"
---
# <a name="addnewimcontacttogroup-operation"></a><span data-ttu-id="57029-103">AddNewImContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="57029-103">AddNewImContactToGroup operation</span></span>

<span data-ttu-id="57029-104">**AddNewImContactToGroup** EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="57029-104">Find information about the **AddNewImContactToGroup** EWS operation.</span></span> 
  
<span data-ttu-id="57029-105">**AddNewImContactToGroup**操作は、新しい連絡先をインスタントメッセージング (IM) グループに追加します。</span><span class="sxs-lookup"><span data-stu-id="57029-105">The **AddNewImContactToGroup** operation adds a new contact to an instant messaging (IM) group.</span></span> 
  
<span data-ttu-id="57029-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="57029-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-addnewimcontacttogroup-operation"></a><span data-ttu-id="57029-107">AddNewImContactToGroup 操作の使用</span><span class="sxs-lookup"><span data-stu-id="57029-107">Using the AddNewImContactToGroup operation</span></span>

<span data-ttu-id="57029-108">**AddNewImContactToGroup**操作は、次の3つの引数を受け取り、IM グループに新しい連絡先を追加します。</span><span class="sxs-lookup"><span data-stu-id="57029-108">The **AddNewImContactToGroup** operation takes the following three arguments to add a new contact to an IM group:</span></span> 
  
- <span data-ttu-id="57029-109">**Imaddress**プロパティ-連絡先の IM アドレスを識別します。</span><span class="sxs-lookup"><span data-stu-id="57029-109">**ImAddress** property - Identifies the contact's IM address.</span></span> <span data-ttu-id="57029-110">このプロパティは必須です。</span><span class="sxs-lookup"><span data-stu-id="57029-110">This property is required.</span></span> 
    
- <span data-ttu-id="57029-111">**DisplayName**プロパティ-連絡先の表示名を識別します。</span><span class="sxs-lookup"><span data-stu-id="57029-111">**DisplayName** property - Identifies the contact's display name.</span></span> 
    
- <span data-ttu-id="57029-112">**GroupId**プロパティ-連絡先が追加されるグループを識別します。</span><span class="sxs-lookup"><span data-stu-id="57029-112">**GroupId** property - Identifies the group that the contact is added to.</span></span> 
    
<span data-ttu-id="57029-113">この操作は、グループに追加された連絡先のペルソナを返します。</span><span class="sxs-lookup"><span data-stu-id="57029-113">This operation returns the persona of the contact that was added to the group.</span></span>
  
### <a name="addnewimcontacttogroup-operation-soap-headers"></a><span data-ttu-id="57029-114">AddNewImContactToGroup 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="57029-114">AddNewImContactToGroup operation SOAP headers</span></span>

<span data-ttu-id="57029-115">**AddNewImContactToGroup**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="57029-115">The **AddNewImContactToGroup** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="57029-116">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="57029-116">**Header name**</span></span>|<span data-ttu-id="57029-117">**要素**</span><span class="sxs-lookup"><span data-stu-id="57029-117">**Element**</span></span>|<span data-ttu-id="57029-118">**説明**</span><span class="sxs-lookup"><span data-stu-id="57029-118">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="57029-119">**偽装**</span><span class="sxs-lookup"><span data-stu-id="57029-119">**Impersonation**</span></span> <br/> |[<span data-ttu-id="57029-120">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="57029-120">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="57029-121">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="57029-121">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="57029-122">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="57029-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="57029-123">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="57029-123">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="57029-124">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="57029-124">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="57029-125">RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。</span><span class="sxs-lookup"><span data-stu-id="57029-125">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="57029-126">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="57029-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="57029-127">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="57029-127">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="57029-128">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="57029-128">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="57029-129">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="57029-129">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="57029-130">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="57029-130">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="57029-131">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="57029-131">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="57029-132">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="57029-132">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="57029-133">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="57029-133">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="57029-134">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="57029-134">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="addnewimcontacttogroup-operation-request-example-add-a-new-im-contact-to-a-group"></a><span data-ttu-id="57029-135">AddNewImContactToGroup 操作要求の例: 新しい IM 連絡先をグループに追加します。</span><span class="sxs-lookup"><span data-stu-id="57029-135">AddNewImContactToGroup operation request example: Add a new IM contact to a group</span></span>

<span data-ttu-id="57029-136">次の**AddNewImContactToGroup**操作要求の例は、新しい連絡先を既存の IM グループに追加する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="57029-136">The following example of an **AddNewImContactToGroup** operation request shows how to add a new contact to an existing IM group.</span></span> <span data-ttu-id="57029-137">この例の**GroupId**プロパティの値は、 [addimgroup 操作](addimgroup-operation.md)の結果から返されました。</span><span class="sxs-lookup"><span data-stu-id="57029-137">The **GroupId** property value for this example was returned from results of the [AddImGroup operation](addimgroup-operation.md).</span></span> <span data-ttu-id="57029-138">**ExchangeStoreId**プロパティには、 **GroupId**プロパティの値が含まれています。</span><span class="sxs-lookup"><span data-stu-id="57029-138">The **ExchangeStoreId** property contains the **GroupId** property value.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
      <t:MailboxCulture>en-US</t:MailboxCulture>
      <t:TimeZoneContext>
         <t:TimeZoneDefinition Id="GMT Standard Time"/>
      </t:TimeZoneContext>
   </soap:Header>
   <soap:Body >
      <m:AddNewImContactToGroup>
         <m:ImAddress>tsmith@contoso.com</m:ImAddress>
         <m:DisplayName>Tony Smith</m:DisplayName>
         <m:GroupId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDAAAQKAAA="
                    ChangeKey="EgAAAA=="/>
      </m:AddNewImContactToGroup>
   </soap:Body>
</soap:Envelope>
```

> [!NOTE]
> <span data-ttu-id="57029-139">**GroupId**値は読みやすいように短縮されています。</span><span class="sxs-lookup"><span data-stu-id="57029-139">The **GroupId** value has been shortened to preserve readability.</span></span> 
  
<span data-ttu-id="57029-140">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="57029-140">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="57029-141">AddNewImContactToGroup</span><span class="sxs-lookup"><span data-stu-id="57029-141">AddNewImContactToGroup</span></span>](addnewimcontacttogroup.md)
    
- [<span data-ttu-id="57029-142">ImAddress (文字列)</span><span class="sxs-lookup"><span data-stu-id="57029-142">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="57029-143">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="57029-143">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="57029-144">GroupId</span><span class="sxs-lookup"><span data-stu-id="57029-144">GroupId</span></span>](groupid.md)
    
## <a name="successful-addnewimcontacttogroup-operation-response"></a><span data-ttu-id="57029-145">成功した AddNewImContactToGroup 操作の応答</span><span class="sxs-lookup"><span data-stu-id="57029-145">Successful AddNewImContactToGroup operation response</span></span>

<span data-ttu-id="57029-146">次の例は、 **AddNewImContactToGroup**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="57029-146">The following example shows a successful response to an **AddNewImContactToGroup** operation request.</span></span> <span data-ttu-id="57029-147">応答には、新しく作成された連絡先のペルソナが含まれています。</span><span class="sxs-lookup"><span data-stu-id="57029-147">The response contains the persona of the newly created contact.</span></span> <span data-ttu-id="57029-148">連絡先が Exchange の [クイック連絡先] フォルダーに追加されます。</span><span class="sxs-lookup"><span data-stu-id="57029-148">The contact is added to the Quick Contacts folder in Exchange.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="57029-149">読みやすくするために、識別子が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="57029-149">Identifiers have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <h:ServerVersionInfo MajorVersion="15" 
                         MinorVersion="0" 
                         MajorBuildNumber="349" 
                         MinorBuildNumber="0" 
                         Version="Exchange2013" 
                         xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                         xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                         xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <AddNewImContactToGroupResponse ResponseClass="Success" 
                                    xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Persona>
        <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MTYzNGNkZmRkYQAQAJ3EkhEEXN5KufGbSYJanZk=" 
                   xmlns="https://schemas.microsoft.com/exchange/services/2006/types" />
        <PersonaType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Person</PersonaType>
        <CreationTime xmlns="https://schemas.microsoft.com/exchange/services/2006/types">2012-01-05T23:06:58Z</CreationTime>
        <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayName>
        <DisplayNameFirstLast xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayNameFirstLast>
        <DisplayNameLastFirst xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Tony Smith</DisplayNameLastFirst>
        <FileAsId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">None</FileAsId>
        <EmailAddress xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Name>Tony Smith</Name>
          <Address>tsmith@contoso.com</Address>
          <RoutingType>SMTP</RoutingType>
        </EmailAddress>
        <EmailAddresses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <EmailAddress>
            <Name>Tony Smith</Name>
            <Address>tsmith@contoso.com</Address>
            <RoutingType>SMTP</RoutingType>
          </EmailAddress>
        </EmailAddresses>
        <ImAddress xmlns="https://schemas.microsoft.com/exchange/services/2006/types">tsmith@contoso.com</ImAddress>
        <RelevanceScore xmlns="https://schemas.microsoft.com/exchange/services/2006/types">2147483647</RelevanceScore>
        <Attributions xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Attribution>
            <Id>0</Id>
            <SourceId Id="BtF8oI7iVOQatt/bhQoTbWAAAAAAvcAAA=" 
                      ChangeKey="EQAAABYAAABtF8oIQoTbWAAAAAAyg" />
            <DisplayName>Outlook</DisplayName>
            <IsWritable>true</IsWritable>
            <IsQuickContact>true</IsQuickContact>
            <IsHidden>false</IsHidden>
            <FolderId Id="AAMkAGQ1MjJjMTBkLTc4YhQoTbWAAAAAAvZAAA=" 
                      ChangeKey="AQAAAA==" />
          </Attribution>
        </Attributions>
        <DisplayNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>Tony Smith</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </DisplayNames>
        <FileAsIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>None</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </FileAsIds>
        <Emails1 xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <EmailAddressAttributedValue>
            <Value>
              <Name>Tony Smith</Name>
              <Address>tsmith@contoso.com</Address>
              <RoutingType>SMTP</RoutingType>
            </Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </EmailAddressAttributedValue>
        </Emails1>
        <ImAddresses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <StringAttributedValue>
            <Value>tsmith@contoso.com</Value>
            <Attributions>
              <Attribution>0</Attribution>
            </Attributions>
          </StringAttributedValue>
        </ImAddresses>
      </Persona>
    </AddNewImContactToGroupResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="57029-150">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="57029-150">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="57029-151">AddNewImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="57029-151">AddNewImContactToGroupResponse</span></span>](addnewimcontacttogroupresponse.md)
    
- [<span data-ttu-id="57029-152">ユーザー</span><span class="sxs-lookup"><span data-stu-id="57029-152">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="57029-153">PersonaId</span><span class="sxs-lookup"><span data-stu-id="57029-153">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="57029-154">個人の Atype</span><span class="sxs-lookup"><span data-stu-id="57029-154">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="57029-155">CreationTime</span><span class="sxs-lookup"><span data-stu-id="57029-155">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="57029-156">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="57029-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="57029-157">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="57029-157">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="57029-158">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="57029-158">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="57029-159">FileAsId</span><span class="sxs-lookup"><span data-stu-id="57029-159">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="57029-160">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="57029-160">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="57029-161">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="57029-161">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="57029-162">Address (string)</span><span class="sxs-lookup"><span data-stu-id="57029-162">Address (string)</span></span>](address-string.md)
    
- [<span data-ttu-id="57029-163">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="57029-163">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="57029-164">ImAddress (文字列)</span><span class="sxs-lookup"><span data-stu-id="57029-164">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="57029-165">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="57029-165">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="57029-166">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="57029-166">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="57029-167">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="57029-167">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="57029-168">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="57029-168">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="57029-169">SourceId</span><span class="sxs-lookup"><span data-stu-id="57029-169">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="57029-170">IsWritable 可能</span><span class="sxs-lookup"><span data-stu-id="57029-170">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="57029-171">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="57029-171">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="57029-172">IsHidden</span><span class="sxs-lookup"><span data-stu-id="57029-172">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="57029-173">FolderId</span><span class="sxs-lookup"><span data-stu-id="57029-173">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="57029-174">DisplayNames</span><span class="sxs-lookup"><span data-stu-id="57029-174">DisplayNames</span></span>](displaynames.md)
    
- [<span data-ttu-id="57029-175">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="57029-175">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="57029-176">値 (ArrayOfStringValueType)</span><span class="sxs-lookup"><span data-stu-id="57029-176">Value (ArrayOfStringValueType)</span></span>](value-arrayofstringvaluetype.md)
    
- [<span data-ttu-id="57029-177">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="57029-177">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="57029-178">Emails1</span><span class="sxs-lookup"><span data-stu-id="57029-178">Emails1</span></span>](emails1.md)
    
- [<span data-ttu-id="57029-179">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="57029-179">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
    
- [<span data-ttu-id="57029-180">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="57029-180">ImAddresses</span></span>](imaddresses.md)
    
## <a name="addnewimcontacttogroup-operation-error-response"></a><span data-ttu-id="57029-181">AddNewImContactToGroup 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="57029-181">AddNewImContactToGroup operation error response</span></span>

<span data-ttu-id="57029-182">次の例は、 **AddNewImContactToGroup**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="57029-182">The following example shows an error response to a **AddNewImContactToGroup** operation request.</span></span> <span data-ttu-id="57029-183">これは、依頼者のメールボックスにないグループに連絡先を追加する要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="57029-183">This is a response to a request to add a contact to a group that is not in the requester's mailbox.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="578" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <AddNewImContactToGroupResponse ResponseClass="Error" 
                                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>No mailbox with such guid.</MessageText>
         <ResponseCode>ErrorNonExistentMailbox</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
         <MessageXml>
            <t:Value Name="MailboxGuid" xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">d5fasdadcw3d-23de-2341-8f59-b71523fsddda</t:Value>
         </MessageXml>
      </AddNewImContactToGroupResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="57029-184">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="57029-184">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="57029-185">AddNewImContactToGroupResponse</span><span class="sxs-lookup"><span data-stu-id="57029-185">AddNewImContactToGroupResponse</span></span>](addnewimcontacttogroupresponse.md)
    
- [<span data-ttu-id="57029-186">MessageText</span><span class="sxs-lookup"><span data-stu-id="57029-186">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="57029-187">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="57029-187">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="57029-188">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="57029-188">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
- [<span data-ttu-id="57029-189">MessageXml</span><span class="sxs-lookup"><span data-stu-id="57029-189">MessageXml</span></span>](messagexml.md)
    
<span data-ttu-id="57029-190">EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)</span><span class="sxs-lookup"><span data-stu-id="57029-190">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="57029-191">関連項目</span><span class="sxs-lookup"><span data-stu-id="57029-191">See also</span></span>



[<span data-ttu-id="57029-192">AddImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="57029-192">AddImGroup operation</span></span>](addimgroup-operation.md)
  
[<span data-ttu-id="57029-193">AddImContactToGroup 操作</span><span class="sxs-lookup"><span data-stu-id="57029-193">AddImContactToGroup operation</span></span>](addimcontacttogroup-operation.md)
  
[<span data-ttu-id="57029-194">AddImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="57029-194">AddImGroup operation</span></span>](addimgroup-operation.md)
  
[<span data-ttu-id="57029-195">RemoveImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="57029-195">RemoveImGroup operation</span></span>](removeimgroup-operation.md)
  
[<span data-ttu-id="57029-196">SetImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="57029-196">SetImGroup operation</span></span>](setimgroup-operation.md)


[<span data-ttu-id="57029-197">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="57029-197">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)

