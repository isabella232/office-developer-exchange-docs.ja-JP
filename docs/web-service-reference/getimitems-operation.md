---
title: GetImItems 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 51186691-46d2-4d5c-b8bc-4ee2bb20fbe7
description: 操作 GetImItems EWS についての情報を検索します。
ms.openlocfilehash: 4335cc22b22dc5f102f2221f7fdb22a506ba026f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760759"
---
# <a name="getimitems-operation"></a><span data-ttu-id="a0b59-103">GetImItems 操作</span><span class="sxs-lookup"><span data-stu-id="a0b59-103">GetImItems operation</span></span>

<span data-ttu-id="a0b59-104">**GetImItems** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="a0b59-104">Find information about the **GetImItems** EWS operation.</span></span> 
  
<span data-ttu-id="a0b59-105">**GetImItems**操作は、インスタント メッセージング (IM) のグループに関する情報を取得し、ペルソナが IM にお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="a0b59-105">The **GetImItems** operation retrieves information about instant messaging (IM) groups and IM contact personas.</span></span> 
  
<span data-ttu-id="a0b59-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="a0b59-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getimitems-operation"></a><span data-ttu-id="a0b59-107">GetImItems 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="a0b59-107">Using the GetImItems operation</span></span>

<span data-ttu-id="a0b59-108">**GetImItems**操作ではグループと連絡先アイテムの識別子グループと取引先担当者に関する情報のセットを返します。</span><span class="sxs-lookup"><span data-stu-id="a0b59-108">The **GetImItems** operation accepts group and contact item identifiers and returns a set of information about the groups and contacts.</span></span> <span data-ttu-id="a0b59-109">応答で返されるプロパティのセットは拡張プロパティを複数の取引先担当者の識別子、グループの識別子によって識別され、引数としてプロパティの定義を拡張します。</span><span class="sxs-lookup"><span data-stu-id="a0b59-109">The property sets returned in the response are identified by extended properties, multiple contact identifiers, group identifiers, and extended property definitions as arguments.</span></span> 
  
### <a name="getimitems-operation-soap-headers"></a><span data-ttu-id="a0b59-110">GetImItems 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a0b59-110">GetImItems operation SOAP headers</span></span>

<span data-ttu-id="a0b59-111">**GetImItems**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="a0b59-111">The **GetImItems** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="a0b59-112">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="a0b59-112">**Header name**</span></span>|<span data-ttu-id="a0b59-113">**要素**</span><span class="sxs-lookup"><span data-stu-id="a0b59-113">**Element**</span></span>|<span data-ttu-id="a0b59-114">**説明**</span><span class="sxs-lookup"><span data-stu-id="a0b59-114">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a0b59-115">**偽装**</span><span class="sxs-lookup"><span data-stu-id="a0b59-115">**Impersonation**</span></span> <br/> |[<span data-ttu-id="a0b59-116">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="a0b59-116">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="a0b59-117">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="a0b59-117">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="a0b59-118">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="a0b59-118">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a0b59-119">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="a0b59-119">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="a0b59-120">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="a0b59-120">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="a0b59-121">RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="a0b59-121">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="a0b59-122">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="a0b59-122">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a0b59-123">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="a0b59-123">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="a0b59-124">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="a0b59-124">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="a0b59-125">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="a0b59-125">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="a0b59-126">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="a0b59-126">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="a0b59-127">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="a0b59-127">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="a0b59-128">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a0b59-128">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="a0b59-129">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="a0b59-129">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="a0b59-130">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="a0b59-130">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getimitems-operation-request-example-get-detailed-information-about-im-contacts-and-groups"></a><span data-ttu-id="a0b59-131">GetImItems 操作の要求の例: IM の連絡先およびグループに関する詳細情報を取得します。</span><span class="sxs-lookup"><span data-stu-id="a0b59-131">GetImItems operation request example: Get detailed information about IM contacts and groups</span></span>

<span data-ttu-id="a0b59-132">**GetImItems**操作要求の次の使用例は、IM の連絡先およびグループに関する詳細情報を要求する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="a0b59-132">The following example of a **GetImItems** operation request shows how to request detailed information about IM contacts and groups.</span></span> <span data-ttu-id="a0b59-133">**GetImItems**操作では、1 つまたは複数の連絡先を要求したり、詳細情報をグループ化することができます。</span><span class="sxs-lookup"><span data-stu-id="a0b59-133">A **GetImItems** operation can request one or more contact or group details.</span></span> <span data-ttu-id="a0b59-134">グループおよび連絡先のカスタム プロパティを取得するのに拡張プロパティを使用することもできます。</span><span class="sxs-lookup"><span data-stu-id="a0b59-134">You can also use extended properties to get custom properties on groups and contacts.</span></span> <span data-ttu-id="a0b59-135">要求された拡張プロパティが存在しないアイテムの場合、応答は要求されたプロパティを無視する、既定のプロパティ セットへの応答を返します。</span><span class="sxs-lookup"><span data-stu-id="a0b59-135">If a requested extended property does not exist on an item, the response will ignore the requested property and return the response for the default property set.</span></span> <span data-ttu-id="a0b59-136">この例では、拡張プロパティを使用して表示名を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="a0b59-136">This example shows you how to get the display name by using extended properties.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="a0b59-137">すべての項目の識別子と変更キーをこの資料では、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="a0b59-137">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> <span data-ttu-id="a0b59-138">この操作のサービスされているキーの変更を無視します。</span><span class="sxs-lookup"><span data-stu-id="a0b59-138">Note that change keys are ignored by the service for this operation.</span></span> 
  
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

<span data-ttu-id="a0b59-139">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a0b59-139">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a0b59-140">GetImItems</span><span class="sxs-lookup"><span data-stu-id="a0b59-140">GetImItems</span></span>](getimitems.md)
    
- [<span data-ttu-id="a0b59-141">ContactIds</span><span class="sxs-lookup"><span data-stu-id="a0b59-141">ContactIds</span></span>](contactids.md)
    
- [<span data-ttu-id="a0b59-142">ItemId</span><span class="sxs-lookup"><span data-stu-id="a0b59-142">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="a0b59-143">GroupIds</span><span class="sxs-lookup"><span data-stu-id="a0b59-143">GroupIds</span></span>](groupids.md)
    
- [<span data-ttu-id="a0b59-144">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span><span class="sxs-lookup"><span data-stu-id="a0b59-144">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span></span>](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [<span data-ttu-id="a0b59-145">ExtendedProperty (PathToExtendedFieldType)</span><span class="sxs-lookup"><span data-stu-id="a0b59-145">ExtendedProperty (PathToExtendedFieldType)</span></span>](extendedproperty-pathtoextendedfieldtype.md)
    
## <a name="successful-getimitems-operation-response"></a><span data-ttu-id="a0b59-146">GetImItems 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="a0b59-146">Successful GetImItems operation response</span></span>

<span data-ttu-id="a0b59-147">IM の連絡先とグループを取得する**GetImItems**要求に正常な応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="a0b59-147">The following example shows a successful response to a **GetImItems** request to get an IM contact and group.</span></span> <span data-ttu-id="a0b59-148">拡張プロパティの表示名が要求されます。</span><span class="sxs-lookup"><span data-stu-id="a0b59-148">The display name is requested in an extended property.</span></span> <span data-ttu-id="a0b59-149">IM の連絡先は、ペルソナの形式で返されます。</span><span class="sxs-lookup"><span data-stu-id="a0b59-149">IM contacts are returned in the form of a persona.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="556" 
                           MinorBuildNumber="8" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetImItemsResponse ResponseClass="Success" 
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImItemList>
            <Groups xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
            <Personas xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="a0b59-150">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a0b59-150">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="a0b59-151">GetImItemsResponse</span><span class="sxs-lookup"><span data-stu-id="a0b59-151">GetImItemsResponse</span></span>](getimitemsresponse.md)
    
- [<span data-ttu-id="a0b59-152">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="a0b59-152">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="a0b59-153">ImItemList</span><span class="sxs-lookup"><span data-stu-id="a0b59-153">ImItemList</span></span>](imitemlist.md)
    
- [<span data-ttu-id="a0b59-154">グループ (ArrayOfImGroupType)</span><span class="sxs-lookup"><span data-stu-id="a0b59-154">Groups (ArrayOfImGroupType)</span></span>](groups-arrayofimgrouptype.md)
    
- [<span data-ttu-id="a0b59-155">ImGroup</span><span class="sxs-lookup"><span data-stu-id="a0b59-155">ImGroup</span></span>](imgroup.md)
    
- [<span data-ttu-id="a0b59-156">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="a0b59-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="a0b59-157">GroupType</span><span class="sxs-lookup"><span data-stu-id="a0b59-157">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="a0b59-158">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="a0b59-158">ExchangeStoreId</span></span>](exchangestoreid.md)
    
- [<span data-ttu-id="a0b59-159">MemberCorrelationKey</span><span class="sxs-lookup"><span data-stu-id="a0b59-159">MemberCorrelationKey</span></span>](membercorrelationkey.md)
    
- [<span data-ttu-id="a0b59-160">ItemId</span><span class="sxs-lookup"><span data-stu-id="a0b59-160">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="a0b59-161">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span><span class="sxs-lookup"><span data-stu-id="a0b59-161">ExtendedProperties (NonEmptyArrayOfExtendedFieldURIs)</span></span>](extendedproperties-nonemptyarrayofextendedfielduris.md)
    
- [<span data-ttu-id="a0b59-162">ExtendedProperty (PathToExtendedFieldType)</span><span class="sxs-lookup"><span data-stu-id="a0b59-162">ExtendedProperty (PathToExtendedFieldType)</span></span>](extendedproperty-pathtoextendedfieldtype.md)
    
- [<span data-ttu-id="a0b59-163">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="a0b59-163">Personas</span></span>](personas-ex15websvcsotherref.md)
    
- [<span data-ttu-id="a0b59-164">PersonaId</span><span class="sxs-lookup"><span data-stu-id="a0b59-164">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="a0b59-165">PersonaType</span><span class="sxs-lookup"><span data-stu-id="a0b59-165">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="a0b59-166">CreationTime</span><span class="sxs-lookup"><span data-stu-id="a0b59-166">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="a0b59-167">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="a0b59-167">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="a0b59-168">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="a0b59-168">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="a0b59-169">表題</span><span class="sxs-lookup"><span data-stu-id="a0b59-169">FileAs</span></span>](fileas.md)
    
- <span data-ttu-id="a0b59-170">[FileAsId](fileasid.md)FileAsId</span><span class="sxs-lookup"><span data-stu-id="a0b59-170">[FileAsId](fileasid.md) FileAsId</span></span> 
    
- [<span data-ttu-id="a0b59-171">ImAddress (文字列)</span><span class="sxs-lookup"><span data-stu-id="a0b59-171">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="a0b59-172">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="a0b59-172">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="a0b59-173">帰属 (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="a0b59-173">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="a0b59-174">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="a0b59-174">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="a0b59-175">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="a0b59-175">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="a0b59-176">SourceId</span><span class="sxs-lookup"><span data-stu-id="a0b59-176">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="a0b59-177">IsWritable</span><span class="sxs-lookup"><span data-stu-id="a0b59-177">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="a0b59-178">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="a0b59-178">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="a0b59-179">IsHidden</span><span class="sxs-lookup"><span data-stu-id="a0b59-179">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="a0b59-180">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="a0b59-180">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="a0b59-181">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="a0b59-181">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="a0b59-182">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="a0b59-182">ImAddresses</span></span>](imaddresses.md)
    
- [<span data-ttu-id="a0b59-183">値 (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="a0b59-183">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md)
    
## <a name="getimitems-operation-error-response"></a><span data-ttu-id="a0b59-184">GetImItems 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="a0b59-184">GetImItems operation error response</span></span>

<span data-ttu-id="a0b59-185">**GetImItems**操作では、識別子を検証しないし、サービスに、無効な取引先担当者またはグループの識別子が指定されている場合期待される**ErrorInvalidImContactId**または**ErrorInvalidImGroupId**エラー応答が返されません。</span><span class="sxs-lookup"><span data-stu-id="a0b59-185">The **GetImItems** operation does not validate identifiers and will not return the expected **ErrorInvalidImContactId** or **ErrorInvalidImGroupId** error response if an invalid contact or group identifier is provided to the service.</span></span> 
  
## <a name="see-also"></a><span data-ttu-id="a0b59-186">関連項目</span><span class="sxs-lookup"><span data-stu-id="a0b59-186">See also</span></span>

- [<span data-ttu-id="a0b59-187">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="a0b59-187">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="a0b59-188">GetImItemList 操作</span><span class="sxs-lookup"><span data-stu-id="a0b59-188">GetImItemList operation</span></span>](getimitemlist-operation.md)
    

