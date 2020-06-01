---
title: GetImItems 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 51186691-46d2-4d5c-b8bc-4ee2bb20fbe7
description: GetImItems EWS 操作についての情報を検索します。
ms.openlocfilehash: 960f4683dd478b0e5f8cf18fa8d1593b7433a249
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44456046"
---
# <a name="getimitems-operation"></a><span data-ttu-id="88c2a-103">GetImItems 操作</span><span class="sxs-lookup"><span data-stu-id="88c2a-103">GetImItems operation</span></span>

<span data-ttu-id="88c2a-104">**Getimitems** EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="88c2a-104">Find information about the **GetImItems** EWS operation.</span></span> 
  
<span data-ttu-id="88c2a-105">**Getimitems**操作は、インスタントメッセージング (im) グループと im 連絡先のペルソナに関する情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="88c2a-105">The **GetImItems** operation retrieves information about instant messaging (IM) groups and IM contact personas.</span></span> 
  
<span data-ttu-id="88c2a-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="88c2a-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getimitems-operation"></a><span data-ttu-id="88c2a-107">GetImItems 操作の使用</span><span class="sxs-lookup"><span data-stu-id="88c2a-107">Using the GetImItems operation</span></span>

<span data-ttu-id="88c2a-108">**Getimitems**操作は、グループと連絡先アイテムの識別子を受け入れ、グループと連絡先に関する情報のセットを返します。</span><span class="sxs-lookup"><span data-stu-id="88c2a-108">The **GetImItems** operation accepts group and contact item identifiers and returns a set of information about the groups and contacts.</span></span> <span data-ttu-id="88c2a-109">応答で返されるプロパティセットは、拡張プロパティ、複数の連絡先識別子、グループ識別子、および拡張プロパティ定義によって、引数として識別されます。</span><span class="sxs-lookup"><span data-stu-id="88c2a-109">The property sets returned in the response are identified by extended properties, multiple contact identifiers, group identifiers, and extended property definitions as arguments.</span></span> 
  
### <a name="getimitems-operation-soap-headers"></a><span data-ttu-id="88c2a-110">GetImItems 操作 SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="88c2a-110">GetImItems operation SOAP headers</span></span>

<span data-ttu-id="88c2a-111">**Getimitems**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="88c2a-111">The **GetImItems** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="88c2a-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="88c2a-112">**Header name**</span></span>|<span data-ttu-id="88c2a-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="88c2a-113">**Element**</span></span>|<span data-ttu-id="88c2a-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="88c2a-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="88c2a-115">**偽装**</span><span class="sxs-lookup"><span data-stu-id="88c2a-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="88c2a-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="88c2a-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="88c2a-117">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="88c2a-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="88c2a-118">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="88c2a-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="88c2a-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="88c2a-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="88c2a-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="88c2a-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="88c2a-121">RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。</span><span class="sxs-lookup"><span data-stu-id="88c2a-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="88c2a-122">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="88c2a-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="88c2a-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="88c2a-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="88c2a-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="88c2a-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="88c2a-125">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="88c2a-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="88c2a-126">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="88c2a-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="88c2a-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="88c2a-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="88c2a-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="88c2a-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="88c2a-129">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="88c2a-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="88c2a-130">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="88c2a-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getimitems-operation-request-example-get-detailed-information-about-im-contacts-and-groups"></a><span data-ttu-id="88c2a-131">GetImItems 操作要求の例: IM 連絡先とグループに関する詳細情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="88c2a-131">GetImItems operation request example: Get detailed information about IM contacts and groups</span></span>

<span data-ttu-id="88c2a-132">次の**Getimitems**操作要求の例は、IM 連絡先とグループに関する詳細情報を要求する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="88c2a-132">The following example of a **GetImItems** operation request shows how to request detailed information about IM contacts and groups.</span></span> <span data-ttu-id="88c2a-133">**Getimitems**操作は、1つまたは複数の連絡先またはグループの詳細を要求できます。</span><span class="sxs-lookup"><span data-stu-id="88c2a-133">A **GetImItems** operation can request one or more contact or group details.</span></span> <span data-ttu-id="88c2a-134">また、拡張プロパティを使用して、グループや連絡先のカスタムプロパティを取得することもできます。</span><span class="sxs-lookup"><span data-stu-id="88c2a-134">You can also use extended properties to get custom properties on groups and contacts.</span></span> <span data-ttu-id="88c2a-135">要求された拡張プロパティがアイテムに存在しない場合、応答は要求されたプロパティを無視し、既定のプロパティセットに対する応答を返します。</span><span class="sxs-lookup"><span data-stu-id="88c2a-135">If a requested extended property does not exist on an item, the response will ignore the requested property and return the response for the default property set.</span></span> <span data-ttu-id="88c2a-136">この例では、拡張プロパティを使用して、表示名を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="88c2a-136">This example shows you how to get the display name by using extended properties.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="88c2a-137">この記事のすべてのアイテム識別子と変更キーは、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="88c2a-137">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> <span data-ttu-id="88c2a-138">この操作では、キーの変更は無視されることに注意してください。</span><span class="sxs-lookup"><span data-stu-id="88c2a-138">Note that change keys are ignored by the service for this operation.</span></span> 
  
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
      <m:GetImItems>
         <m:ContactIds>
            <t:ItemId Id="AAMkADEzOTExYACABmEhpSAAA=" ChangeKey="EQAAABBmNDjF"/>
         </m:ContactIds>
         <m:GroupIds>
            <t:ItemId Id="AAMkADEzOTExYjJkBY7+0EAAA=" ChangeKey="EgAAAA=="/>
         </m:GroupIds>         
         <m:ExtendedProperties>
            <t:ExtendedProperty PropertyTag="0x3001" PropertyType="String"/>
         </m:ExtendedProperties>
      </m:GetImItems>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="88c2a-139">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="88c2a-139">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="88c2a-140">GetImItems</span><span class="sxs-lookup"><span data-stu-id="88c2a-140">GetImItems</span></span>](getimitems.md)
    
- [<span data-ttu-id="88c2a-141">ContactIds</span><span class="sxs-lookup"><span data-stu-id="88c2a-141">ContactIds</span></span>](contactids.md)
    
- [<span data-ttu-id="88c2a-142">ItemId</span><span class="sxs-lookup"><span data-stu-id="88c2a-142">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="88c2a-143">Groupid</span><span class="sxs-lookup"><span data-stu-id="88c2a-143">GroupIds</span></span>](groupids.md)
    
- [<span data-ttu-id="88c2a-144">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span><span class="sxs-lookup"><span data-stu-id="88c2a-144">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span></span>](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [<span data-ttu-id="88c2a-145">ExtendedProperty (PathToExtendedFieldType)</span><span class="sxs-lookup"><span data-stu-id="88c2a-145">ExtendedProperty (PathToExtendedFieldType)</span></span>](extendedproperty-pathtoextendedfieldtype.md)
    
## <a name="successful-getimitems-operation-response"></a><span data-ttu-id="88c2a-146">成功した GetImItems 操作の応答</span><span class="sxs-lookup"><span data-stu-id="88c2a-146">Successful GetImItems operation response</span></span>

<span data-ttu-id="88c2a-147">次の例は、IM 連絡先とグループを取得するための**Getimitems**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="88c2a-147">The following example shows a successful response to a **GetImItems** request to get an IM contact and group.</span></span> <span data-ttu-id="88c2a-148">表示名は、拡張プロパティで要求されます。</span><span class="sxs-lookup"><span data-stu-id="88c2a-148">The display name is requested in an extended property.</span></span> <span data-ttu-id="88c2a-149">IM 連絡先は、ペルソナの形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="88c2a-149">IM contacts are returned in the form of a persona.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="https://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetImItemsResponse ResponseClass="Success" 
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImItemList>
            <Groups xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <ImGroup>
                  <DisplayName>Exchange SDK Team</DisplayName>
                  <GroupType>IPM.DistList.MOC.UserGroup</GroupType>
                  <ExchangeStoreId Id="AAMkADEzQrAABY7+0EAAA=" ChangeKey="EgAAAA=="/>
                  <MemberCorrelationKey>
                     <ItemId Id="AAMkADEzOTExYjeGgGqm4QrAABmEhpSAAA=" ChangeKey="EQAAAA=="/>
                  </MemberCorrelationKey>
                  <ExtendedProperties>
                     <ExtendedProperty>
                        <ExtendedFieldURI PropertyTag="0x3001" PropertyType="String"/>
                        <Value>Exchange SDK Team</Value>
                     </ExtendedProperty>
                  </ExtendedProperties>
               </ImGroup>
            </Groups>
            <Personas xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <Persona>
                  <PersonaId Id="AAQkADEzOTBZImBzN5J/uHXc="/>
                  <PersonaType>Person</PersonaType>
                  <CreationTime>2012-11-07T00:10:35Z</CreationTime>
                  <DisplayName>Tony Smith</DisplayName>
                  <DisplayNameFirstLast>Tony Smith</DisplayNameFirstLast>
                  <DisplayNameLastFirst>Tony Smith</DisplayNameLastFirst>
                  <FileAs/>
                  <FileAsId>None</FileAsId>
                  <ImAddress>tsmith@contoso.com</ImAddress>
                  <RelevanceScore>2147483647</RelevanceScore>
                  <Attributions>
                     <Attribution>
                        <Id>0</Id>
                        <SourceId Id="AAMkADEzhQaoeGgGqm4QrAABmEhpSAAA=" ChangeKey="EQArAABmNDjF"/>
                        <DisplayName>Lync Contacts</DisplayName>
                        <IsWritable>false</IsWritable>
                        <IsQuickContact>true</IsQuickContact>
                        <IsHidden>false</IsHidden>
                     </Attribution>
                  </Attributions>
                  <DisplayNames>
                     <StringAttributedValue>
                        <Value>Tony Smith</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </DisplayNames>
                  <FileAsIds>
                     <StringAttributedValue>
                        <Value>None</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </FileAsIds>
                  <ImAddresses>
                     <StringAttributedValue>
                        <Value>tsmith@contoso.com</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </ImAddresses>
                  <ExtendedProperties>
                     <ExtendedPropertyAttributedValue>
                        <Value>
                           <ExtendedFieldURI PropertyTag="0x3001" PropertyType="String"/>
                           <Value>Tony Smith</Value>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </ExtendedPropertyAttributedValue>
                  </ExtendedProperties>
               </Persona>
            </Personas>
         </ImItemList>
      </GetImItemsResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="88c2a-150">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="88c2a-150">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="88c2a-151">GetImItemsResponse</span><span class="sxs-lookup"><span data-stu-id="88c2a-151">GetImItemsResponse</span></span>](getimitemsresponse.md)
    
- [<span data-ttu-id="88c2a-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="88c2a-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="88c2a-153">ImItemList</span><span class="sxs-lookup"><span data-stu-id="88c2a-153">ImItemList</span></span>](imitemlist.md)
    
- [<span data-ttu-id="88c2a-154">グループ (ArrayOfImGroupType)</span><span class="sxs-lookup"><span data-stu-id="88c2a-154">Groups (ArrayOfImGroupType)</span></span>](groups-arrayofimgrouptype.md)
    
- [<span data-ttu-id="88c2a-155">ImGroup</span><span class="sxs-lookup"><span data-stu-id="88c2a-155">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="88c2a-156">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="88c2a-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="88c2a-157">GroupType</span><span class="sxs-lookup"><span data-stu-id="88c2a-157">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="88c2a-158">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="88c2a-158">ExchangeStoreId</span></span>](exchangestoreid.md)
    
- [<span data-ttu-id="88c2a-159">MemberCorrelationKey</span><span class="sxs-lookup"><span data-stu-id="88c2a-159">MemberCorrelationKey</span></span>](membercorrelationkey.md)
    
- [<span data-ttu-id="88c2a-160">ItemId</span><span class="sxs-lookup"><span data-stu-id="88c2a-160">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="88c2a-161">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span><span class="sxs-lookup"><span data-stu-id="88c2a-161">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span></span>](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [<span data-ttu-id="88c2a-162">ExtendedProperty (PathToExtendedFieldType)</span><span class="sxs-lookup"><span data-stu-id="88c2a-162">ExtendedProperty (PathToExtendedFieldType)</span></span>](extendedproperty-pathtoextendedfieldtype.md)
    
- [<span data-ttu-id="88c2a-163">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="88c2a-163">Personas</span></span>](personas-ex15websvcsotherref.md)
    
- [<span data-ttu-id="88c2a-164">PersonaId</span><span class="sxs-lookup"><span data-stu-id="88c2a-164">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="88c2a-165">個人の Atype</span><span class="sxs-lookup"><span data-stu-id="88c2a-165">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="88c2a-166">CreationTime</span><span class="sxs-lookup"><span data-stu-id="88c2a-166">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="88c2a-167">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="88c2a-167">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="88c2a-168">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="88c2a-168">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="88c2a-169">FileAs</span><span class="sxs-lookup"><span data-stu-id="88c2a-169">FileAs</span></span>](fileas.md)
    
- <span data-ttu-id="88c2a-170">[Fileasid](fileasid.md)FileAsId</span><span class="sxs-lookup"><span data-stu-id="88c2a-170">[FileAsId](fileasid.md) FileAsId</span></span> 
    
- [<span data-ttu-id="88c2a-171">ImAddress (文字列)</span><span class="sxs-lookup"><span data-stu-id="88c2a-171">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="88c2a-172">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="88c2a-172">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="88c2a-173">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="88c2a-173">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="88c2a-174">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="88c2a-174">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="88c2a-175">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="88c2a-175">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="88c2a-176">SourceId</span><span class="sxs-lookup"><span data-stu-id="88c2a-176">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="88c2a-177">IsWritable 可能</span><span class="sxs-lookup"><span data-stu-id="88c2a-177">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="88c2a-178">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="88c2a-178">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="88c2a-179">IsHidden</span><span class="sxs-lookup"><span data-stu-id="88c2a-179">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="88c2a-180">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="88c2a-180">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="88c2a-181">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="88c2a-181">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="88c2a-182">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="88c2a-182">ImAddresses</span></span>](imaddresses.md)
    
- [<span data-ttu-id="88c2a-183">Value (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="88c2a-183">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md)
    
## <a name="getimitems-operation-error-response"></a><span data-ttu-id="88c2a-184">GetImItems 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="88c2a-184">GetImItems operation error response</span></span>

<span data-ttu-id="88c2a-185">**Getimitems**操作は、識別子を検証しません。無効な連絡先またはグループの識別子がサービスに指定されている場合、 **ErrorInvalidImContactId**または**ErrorInvalidImGroupId**のエラー応答は返されません。</span><span class="sxs-lookup"><span data-stu-id="88c2a-185">The **GetImItems** operation does not validate identifiers and will not return the expected **ErrorInvalidImContactId** or **ErrorInvalidImGroupId** error response if an invalid contact or group identifier is provided to the service.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="88c2a-186">関連項目</span><span class="sxs-lookup"><span data-stu-id="88c2a-186">See also</span></span>

- [<span data-ttu-id="88c2a-187">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="88c2a-187">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="88c2a-188">GetImItemList 操作</span><span class="sxs-lookup"><span data-stu-id="88c2a-188">GetImItemList operation</span></span>](getimitemlist-operation.md)
    

