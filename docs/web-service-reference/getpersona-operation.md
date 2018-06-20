---
title: GetPersona 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e2146df0-53d0-4caf-9758-b600bbc14b6a
description: 操作 GetPersona EWS についての情報を検索します。
ms.openlocfilehash: c6ac357eaa34e9bae2fe0a79a4a2d02449100e78
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760828"
---
# <a name="getpersona-operation"></a><span data-ttu-id="7ea48-103">GetPersona 操作</span><span class="sxs-lookup"><span data-stu-id="7ea48-103">GetPersona operation</span></span>

<span data-ttu-id="7ea48-104">**GetPersona** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="7ea48-104">Find information about the **GetPersona** EWS operation.</span></span> 
  
<span data-ttu-id="7ea48-105">**GetPersona**操作では、ペルソナに関連付けられているプロパティのセットを返します。</span><span class="sxs-lookup"><span data-stu-id="7ea48-105">The **GetPersona** operation returns a set of properties that are associated with a persona.</span></span> 
  
<span data-ttu-id="7ea48-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="7ea48-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getpersona-operation"></a><span data-ttu-id="7ea48-107">GetPersona 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="7ea48-107">Using the GetPersona operation</span></span>

<span data-ttu-id="7ea48-108">**GetPersona**操作では、ペルソナの形で集約の連絡先情報へのアクセスを提供します。</span><span class="sxs-lookup"><span data-stu-id="7ea48-108">The **GetPersona** operation provides access to aggregated contact information in the form of a persona.</span></span> <span data-ttu-id="7ea48-109">要求内の[PersonaId](personaid.md)要素を返す、ペルソナを識別します。</span><span class="sxs-lookup"><span data-stu-id="7ea48-109">The [PersonaId](personaid.md) element in the request identifies the persona to return in the response.</span></span> <span data-ttu-id="7ea48-110">応答には、ペルソナのプロパティの既定の設定またはカスタム プロパティ セットを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="7ea48-110">The response can contain a default set of persona properties or a custom property set.</span></span> <span data-ttu-id="7ea48-111">プロパティを使用していないが処理され、サーバーからクライアントに送信しないように設定するカスタム プロパティを指定することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="7ea48-111">We recommend that you specify a custom property set so that unused properties are not processed and sent from the server to the client.</span></span> 
  
### <a name="getpersona-operation-soap-headers"></a><span data-ttu-id="7ea48-112">GetPersona 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7ea48-112">GetPersona operation SOAP headers</span></span>

<span data-ttu-id="7ea48-113">**GetPersona**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="7ea48-113">The **GetPersona** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="7ea48-114">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="7ea48-114">**Header name**</span></span>|<span data-ttu-id="7ea48-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="7ea48-115">**Element**</span></span>|<span data-ttu-id="7ea48-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="7ea48-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="7ea48-117">**偽装**</span><span class="sxs-lookup"><span data-stu-id="7ea48-117">**Impersonation**</span></span> <br/> |[<span data-ttu-id="7ea48-118">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="7ea48-118">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="7ea48-119">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="7ea48-119">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="7ea48-120">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="7ea48-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7ea48-121">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="7ea48-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="7ea48-122">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="7ea48-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="7ea48-123">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="7ea48-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="7ea48-124">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="7ea48-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="7ea48-125">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="7ea48-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="7ea48-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="7ea48-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="7ea48-127">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="7ea48-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="7ea48-128">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="7ea48-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getpersona-operation-request-example-return-a-default-set-of-properties-for-a-persona"></a><span data-ttu-id="7ea48-129">GetPersona 操作の要求の例: ペルソナのプロパティの既定のセットを返す</span><span class="sxs-lookup"><span data-stu-id="7ea48-129">GetPersona operation request example: Return a default set of properties for a persona</span></span>

<span data-ttu-id="7ea48-130">**GetPersona**操作要求の次の例では、ペルソナに関連付けられているプロパティの既定のセットを返す方法を示します。</span><span class="sxs-lookup"><span data-stu-id="7ea48-130">The following example of a **GetPersona** operation request shows how to return a default set of properties that are associated with a persona.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <GetPersona>
         <PersonaId Id="AAQkADEzAQAKtOtR/l4MlLqHWORfhSYKU="/>
      </GetPersona>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="7ea48-131">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7ea48-131">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7ea48-132">GetPersona</span><span class="sxs-lookup"><span data-stu-id="7ea48-132">GetPersona</span></span>](getpersona.md)
    
- [<span data-ttu-id="7ea48-133">PersonaId</span><span class="sxs-lookup"><span data-stu-id="7ea48-133">PersonaId</span></span>](personaid.md)
    
## <a name="successful-getpersona-operation-response"></a><span data-ttu-id="7ea48-134">GetPersona 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="7ea48-134">Successful GetPersona operation response</span></span>

<span data-ttu-id="7ea48-135">成功した要求への応答、 **GetPersona**操作の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ea48-135">The following example shows a successful response to a **GetPersona** operation request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="7ea48-136">すべての項目の識別子と変更キーをこの資料では、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="7ea48-136">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="432" 
                           MinorBuildNumber="5" 
                           Version="Exchange2013"
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                     xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetPersonaResponseMessage ResponseClass="Success"
                      xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <Persona>
            <PersonaId Id="AAQkADEzAQAKtOtR="
              xmlns="http://schemas.microsoft.com/exchange/services/2006/types"/>
            <PersonaType xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Person</PersonaType>
            <CreationTime xmlns="http://schemas.microsoft.com/exchange/services/2006/types">2012-06-01T17:00:34Z</CreationTime>
            <DisplayName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayName>
            <DisplayNameFirstLast xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayNameFirstLast>
            <DisplayNameLastFirst xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Johnson Brian</DisplayNameLastFirst>
            <FileAs xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Johnson, Brian</FileAs>
            <FileAsId xmlns="http://schemas.microsoft.com/exchange/services/2006/types">None</FileAsId>
            <GivenName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Brian</GivenName>
            <Surname xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Johnsoon</Surname>
            <CompanyName xmlns="http://schemas.microsoft.com/exchange/services/2006/types">Contoso</CompanyName>
            <RelevanceScore xmlns="http://schemas.microsoft.com/exchange/services/2006/types">4255550110</RelevanceScore>
            <Attributions xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Attribution>
                  <Id>0</Id>
                  <SourceId Id="AAMkA =" ChangeKey="EQAAABY+"/>
                  <DisplayName>Outlook</DisplayName>
                  <IsWritable>true</IsWritable>
                  <IsQuickContact>false</IsQuickContact>
                  <IsHidden>false</IsHidden>
                  <FolderId Id="AAMkA=" ChangeKey="AQAAAA=="/>
               </Attribution>
            </Attributions>
            <DisplayNames xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </DisplayNames>
            <FileAses xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson, Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAses>
            <FileAsIds xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>None</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAsIds>
            <GivenNames xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </GivenNames>
            <Surnames xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </Surnames>
            <MobilePhones xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <PhoneNumberAttributedValue>
                  <Value>
                     <Number>(425)555-0110</Number>
                     <Type>Mobile</Type>
                  </Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </PhoneNumberAttributedValue>
            </MobilePhones>
            <CompanyNames xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Contoso</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </CompanyNames>
         </Persona>
      </GetPersonaResponseMessage>
   </s:Body>
</s:Envelope>

```

<span data-ttu-id="7ea48-137">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7ea48-137">The response SOAP body contains the following elements:</span></span>
  
- <span data-ttu-id="7ea48-138">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7ea48-138">GetPersonaResponseMessage</span></span>
    
- [<span data-ttu-id="7ea48-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7ea48-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7ea48-140">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="7ea48-140">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="7ea48-141">PersonaId</span><span class="sxs-lookup"><span data-stu-id="7ea48-141">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="7ea48-142">PersonaType</span><span class="sxs-lookup"><span data-stu-id="7ea48-142">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="7ea48-143">CreationTime</span><span class="sxs-lookup"><span data-stu-id="7ea48-143">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="7ea48-144">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="7ea48-144">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="7ea48-145">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="7ea48-145">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="7ea48-146">表題</span><span class="sxs-lookup"><span data-stu-id="7ea48-146">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="7ea48-147">FileAsId</span><span class="sxs-lookup"><span data-stu-id="7ea48-147">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="7ea48-148">GivenName</span><span class="sxs-lookup"><span data-stu-id="7ea48-148">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="7ea48-149">姓</span><span class="sxs-lookup"><span data-stu-id="7ea48-149">Surname</span></span>](surname.md)
    
- <span data-ttu-id="7ea48-150">[[得意先名]](companyname.md)</span><span class="sxs-lookup"><span data-stu-id="7ea48-150">[CompanyName](companyname.md)</span></span>
    
- [<span data-ttu-id="7ea48-151">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="7ea48-151">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="7ea48-152">帰属 (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="7ea48-152">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="7ea48-153">属性 (文字列)</span><span class="sxs-lookup"><span data-stu-id="7ea48-153">Attribution (string)</span></span>](attribution-string.md)
    
- [<span data-ttu-id="7ea48-154">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="7ea48-154">ID (String)</span></span>](id-string.md)
    
- <span data-ttu-id="7ea48-155">[SourceId](sourceid.md)SourceId</span><span class="sxs-lookup"><span data-stu-id="7ea48-155">[SourceId](sourceid.md) SourceId</span></span> 
    
- [<span data-ttu-id="7ea48-156">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="7ea48-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="7ea48-157">IsWritable</span><span class="sxs-lookup"><span data-stu-id="7ea48-157">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="7ea48-158">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="7ea48-158">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="7ea48-159">IsHidden</span><span class="sxs-lookup"><span data-stu-id="7ea48-159">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="7ea48-160">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="7ea48-160">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="7ea48-161">表示名</span><span class="sxs-lookup"><span data-stu-id="7ea48-161">DisplayNames</span></span>](displaynames.md)
    
- [<span data-ttu-id="7ea48-162">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="7ea48-162">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="7ea48-163">値 (ArrayOfStringValueType)</span><span class="sxs-lookup"><span data-stu-id="7ea48-163">Value (ArrayOfStringValueType)</span></span>](value-arrayofstringvaluetype.md)
    
- [<span data-ttu-id="7ea48-164">帰属 (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="7ea48-164">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="7ea48-165">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="7ea48-165">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="7ea48-166">FileAses</span><span class="sxs-lookup"><span data-stu-id="7ea48-166">FileAses</span></span>](fileases.md)
    
- [<span data-ttu-id="7ea48-167">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="7ea48-167">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="7ea48-168">GivenNames</span><span class="sxs-lookup"><span data-stu-id="7ea48-168">GivenNames</span></span>](givennames.md)
    
- [<span data-ttu-id="7ea48-169">姓</span><span class="sxs-lookup"><span data-stu-id="7ea48-169">Surnames</span></span>](surnames.md)
    
- [<span data-ttu-id="7ea48-170">MobilePhones</span><span class="sxs-lookup"><span data-stu-id="7ea48-170">MobilePhones</span></span>](mobilephones.md)
    
- [<span data-ttu-id="7ea48-171">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="7ea48-171">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="7ea48-172">値 (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="7ea48-172">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md)
    
- [<span data-ttu-id="7ea48-173">番号</span><span class="sxs-lookup"><span data-stu-id="7ea48-173">Number</span></span>](number.md)
    
- [<span data-ttu-id="7ea48-174">型 (文字列)</span><span class="sxs-lookup"><span data-stu-id="7ea48-174">Type (string)</span></span>](type-string.md)
    
- [<span data-ttu-id="7ea48-175">CompanyNames</span><span class="sxs-lookup"><span data-stu-id="7ea48-175">CompanyNames</span></span>](companynames.md)
    
## <a name="getpersona-operation-error-response"></a><span data-ttu-id="7ea48-176">GetPersona 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="7ea48-176">GetPersona operation error response</span></span>

<span data-ttu-id="7ea48-177">**GetPersona**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="7ea48-177">The following example shows an error response to a **GetPersona** operation request.</span></span> <span data-ttu-id="7ea48-178">これは、ペルソナを誤って指定された識別子を含む要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="7ea48-178">This is a response to a request that contains an incorrectly specified persona identifier.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="578" 
                           MinorBuildNumber="11" 
                           Version="Exchange2013" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetPersonaResponseMessage ResponseClass="Error" 
                                 xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Id is malformed.</MessageText>
         <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetPersonaResponseMessage>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="7ea48-179">エラー応答 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="7ea48-179">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="7ea48-180">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="7ea48-180">GetPersonaResponseMessage</span></span>](getpersonaresponsemessage.md)
    
- [<span data-ttu-id="7ea48-181">MessageText</span><span class="sxs-lookup"><span data-stu-id="7ea48-181">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="7ea48-182">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="7ea48-182">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="7ea48-183">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="7ea48-183">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="7ea48-184">EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7ea48-184">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="7ea48-185">関連項目</span><span class="sxs-lookup"><span data-stu-id="7ea48-185">See also</span></span>

- [<span data-ttu-id="7ea48-186">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="7ea48-186">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="7ea48-187">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="7ea48-187">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="7ea48-188">FindPeople 操作</span><span class="sxs-lookup"><span data-stu-id="7ea48-188">FindPeople operation</span></span>](findpeople-operation.md)
    

