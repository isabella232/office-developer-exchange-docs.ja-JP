---
title: GetPersona 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e2146df0-53d0-4caf-9758-b600bbc14b6a
description: GetPersona EWS 操作についての情報を検索します。
ms.openlocfilehash: 2b335c694a85f87c96432ea6d7c1c674613d2f17
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460947"
---
# <a name="getpersona-operation"></a><span data-ttu-id="9d7c4-103">GetPersona 操作</span><span class="sxs-lookup"><span data-stu-id="9d7c4-103">GetPersona operation</span></span>

<span data-ttu-id="9d7c4-104">**Getpersona** EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-104">Find information about the **GetPersona** EWS operation.</span></span> 
  
<span data-ttu-id="9d7c4-105">**Getpersona**操作は、ペルソナに関連付けられている一連のプロパティを返します。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-105">The **GetPersona** operation returns a set of properties that are associated with a persona.</span></span> 
  
<span data-ttu-id="9d7c4-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-getpersona-operation"></a><span data-ttu-id="9d7c4-107">GetPersona 操作の使用</span><span class="sxs-lookup"><span data-stu-id="9d7c4-107">Using the GetPersona operation</span></span>

<span data-ttu-id="9d7c4-108">**Getpersona**操作は、一連の連絡先情報へのアクセスをペルソナの形式で提供します。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-108">The **GetPersona** operation provides access to aggregated contact information in the form of a persona.</span></span> <span data-ttu-id="9d7c4-109">要求の[個人エイド](personaid.md)要素は、応答で返されるペルソナを識別します。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-109">The [PersonaId](personaid.md) element in the request identifies the persona to return in the response.</span></span> <span data-ttu-id="9d7c4-110">応答には、既定のペルソナプロパティセットまたはカスタムプロパティセットを含めることができます。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-110">The response can contain a default set of persona properties or a custom property set.</span></span> <span data-ttu-id="9d7c4-111">カスタムプロパティセットを指定して、使用されていないプロパティを処理して、サーバーからクライアントに送信することをお勧めします。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-111">We recommend that you specify a custom property set so that unused properties are not processed and sent from the server to the client.</span></span> 
  
### <a name="getpersona-operation-soap-headers"></a><span data-ttu-id="9d7c4-112">GetPersona operation SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="9d7c4-112">GetPersona operation SOAP headers</span></span>

<span data-ttu-id="9d7c4-113">**Getpersona**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-113">The **GetPersona** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="9d7c4-114">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="9d7c4-114">**Header name**</span></span>|<span data-ttu-id="9d7c4-115">**要素**</span><span class="sxs-lookup"><span data-stu-id="9d7c4-115">**Element**</span></span>|<span data-ttu-id="9d7c4-116">**説明**</span><span class="sxs-lookup"><span data-stu-id="9d7c4-116">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="9d7c4-117">**偽装**</span><span class="sxs-lookup"><span data-stu-id="9d7c4-117">**Impersonation**</span></span> <br/> |[<span data-ttu-id="9d7c4-118">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="9d7c4-118">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="9d7c4-119">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-119">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="9d7c4-120">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-120">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="9d7c4-121">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="9d7c4-121">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="9d7c4-122">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="9d7c4-122">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="9d7c4-123">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-123">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="9d7c4-124">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-124">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="9d7c4-125">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="9d7c4-125">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="9d7c4-126">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="9d7c4-126">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="9d7c4-127">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-127">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="9d7c4-128">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-128">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getpersona-operation-request-example-return-a-default-set-of-properties-for-a-persona"></a><span data-ttu-id="9d7c4-129">GetPersona operation 要求の例: ペルソナの既定のプロパティセットを返します。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-129">GetPersona operation request example: Return a default set of properties for a persona</span></span>

<span data-ttu-id="9d7c4-130">次の**Getpersona** operation 要求の例は、ペルソナに関連付けられている既定のプロパティセットを返す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-130">The following example of a **GetPersona** operation request shows how to return a default set of properties that are associated with a persona.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013"/>
   </soap:Header>
   <soap:Body xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <GetPersona>
         <PersonaId Id="AAQkADEzAQAKtOtR/l4MlLqHWORfhSYKU="/>
      </GetPersona>
   </soap:Body>
</soap:Envelope>

```

<span data-ttu-id="9d7c4-131">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-131">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="9d7c4-132">GetPersona</span><span class="sxs-lookup"><span data-stu-id="9d7c4-132">GetPersona</span></span>](getpersona.md)
    
- [<span data-ttu-id="9d7c4-133">PersonaId</span><span class="sxs-lookup"><span data-stu-id="9d7c4-133">PersonaId</span></span>](personaid.md)
    
## <a name="successful-getpersona-operation-response"></a><span data-ttu-id="9d7c4-134">成功した GetPersona 操作応答</span><span class="sxs-lookup"><span data-stu-id="9d7c4-134">Successful GetPersona operation response</span></span>

<span data-ttu-id="9d7c4-135">次の例は、 **Getpersona**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-135">The following example shows a successful response to a **GetPersona** operation request.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="9d7c4-136">この記事のすべてのアイテム識別子と変更キーは、読みやすくするために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-136">All item identifiers and change keys in this article have been shortened to preserve readability.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="432" 
                           MinorBuildNumber="5" 
                           Version="Exchange2013"
                           xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                     xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
      xmlns:xsd="http://www.w3.org/2001/XMLSchema"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"/>
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetPersonaResponseMessage ResponseClass="Success"
                      xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <Persona>
            <PersonaId Id="AAQkADEzAQAKtOtR="
              xmlns="https://schemas.microsoft.com/exchange/services/2006/types"/>
            <PersonaType xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Person</PersonaType>
            <CreationTime xmlns="https://schemas.microsoft.com/exchange/services/2006/types">2012-06-01T17:00:34Z</CreationTime>
            <DisplayName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayName>
            <DisplayNameFirstLast xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian Johnson</DisplayNameFirstLast>
            <DisplayNameLastFirst xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnson Brian</DisplayNameLastFirst>
            <FileAs xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnson, Brian</FileAs>
            <FileAsId xmlns="https://schemas.microsoft.com/exchange/services/2006/types">None</FileAsId>
            <GivenName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Brian</GivenName>
            <Surname xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Johnsoon</Surname>
            <CompanyName xmlns="https://schemas.microsoft.com/exchange/services/2006/types">Contoso</CompanyName>
            <RelevanceScore xmlns="https://schemas.microsoft.com/exchange/services/2006/types">4255550110</RelevanceScore>
            <Attributions xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
            <DisplayNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </DisplayNames>
            <FileAses xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson, Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAses>
            <FileAsIds xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>None</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </FileAsIds>
            <GivenNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Brian</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </GivenNames>
            <Surnames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
               <StringAttributedValue>
                  <Value>Johnson</Value>
                  <Attributions>
                     <Attribution>0</Attribution>
                  </Attributions>
               </StringAttributedValue>
            </Surnames>
            <MobilePhones xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
            <CompanyNames xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="9d7c4-137">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-137">The response SOAP body contains the following elements:</span></span>
  
- <span data-ttu-id="9d7c4-138">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9d7c4-138">GetPersonaResponseMessage</span></span>
    
- [<span data-ttu-id="9d7c4-139">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9d7c4-139">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="9d7c4-140">ユーザー</span><span class="sxs-lookup"><span data-stu-id="9d7c4-140">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="9d7c4-141">PersonaId</span><span class="sxs-lookup"><span data-stu-id="9d7c4-141">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="9d7c4-142">個人の Atype</span><span class="sxs-lookup"><span data-stu-id="9d7c4-142">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="9d7c4-143">CreationTime</span><span class="sxs-lookup"><span data-stu-id="9d7c4-143">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="9d7c4-144">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="9d7c4-144">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="9d7c4-145">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="9d7c4-145">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="9d7c4-146">FileAs</span><span class="sxs-lookup"><span data-stu-id="9d7c4-146">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="9d7c4-147">FileAsId</span><span class="sxs-lookup"><span data-stu-id="9d7c4-147">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="9d7c4-148">GivenName</span><span class="sxs-lookup"><span data-stu-id="9d7c4-148">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="9d7c4-149">姓</span><span class="sxs-lookup"><span data-stu-id="9d7c4-149">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="9d7c4-150">CompanyName</span><span class="sxs-lookup"><span data-stu-id="9d7c4-150">CompanyName</span></span>](companyname.md)
    
- [<span data-ttu-id="9d7c4-151">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="9d7c4-151">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="9d7c4-152">Attributions (ArrayOfValueAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="9d7c4-152">Attributions (ArrayOfValueAttributionsType)</span></span>](attributions-arrayofvalueattributionstype.md)
    
- [<span data-ttu-id="9d7c4-153">属性 (string)</span><span class="sxs-lookup"><span data-stu-id="9d7c4-153">Attribution (string)</span></span>](attribution-string.md)
    
- [<span data-ttu-id="9d7c4-154">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="9d7c4-154">ID (String)</span></span>](id-string.md)
    
- <span data-ttu-id="9d7c4-155">[SourceId](sourceid.md)SourceId</span><span class="sxs-lookup"><span data-stu-id="9d7c4-155">[SourceId](sourceid.md) SourceId</span></span> 
    
- [<span data-ttu-id="9d7c4-156">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="9d7c4-156">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="9d7c4-157">IsWritable 可能</span><span class="sxs-lookup"><span data-stu-id="9d7c4-157">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="9d7c4-158">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="9d7c4-158">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="9d7c4-159">IsHidden</span><span class="sxs-lookup"><span data-stu-id="9d7c4-159">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="9d7c4-160">FolderId</span><span class="sxs-lookup"><span data-stu-id="9d7c4-160">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="9d7c4-161">DisplayNames</span><span class="sxs-lookup"><span data-stu-id="9d7c4-161">DisplayNames</span></span>](displaynames.md)
    
- [<span data-ttu-id="9d7c4-162">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="9d7c4-162">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="9d7c4-163">値 (ArrayOfStringValueType)</span><span class="sxs-lookup"><span data-stu-id="9d7c4-163">Value (ArrayOfStringValueType)</span></span>](value-arrayofstringvaluetype.md)
    
- [<span data-ttu-id="9d7c4-164">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="9d7c4-164">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="9d7c4-165">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="9d7c4-165">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="9d7c4-166">FileAses</span><span class="sxs-lookup"><span data-stu-id="9d7c4-166">FileAses</span></span>](fileases.md)
    
- [<span data-ttu-id="9d7c4-167">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="9d7c4-167">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="9d7c4-168">与えた名前</span><span class="sxs-lookup"><span data-stu-id="9d7c4-168">GivenNames</span></span>](givennames.md)
    
- [<span data-ttu-id="9d7c4-169">Surnames</span><span class="sxs-lookup"><span data-stu-id="9d7c4-169">Surnames</span></span>](surnames.md)
    
- [<span data-ttu-id="9d7c4-170">MobilePhones</span><span class="sxs-lookup"><span data-stu-id="9d7c4-170">MobilePhones</span></span>](mobilephones.md)
    
- [<span data-ttu-id="9d7c4-171">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="9d7c4-171">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="9d7c4-172">Value (PersonaPhoneNumberType)</span><span class="sxs-lookup"><span data-stu-id="9d7c4-172">Value (PersonaPhoneNumberType)</span></span>](value-personaphonenumbertype.md)
    
- [<span data-ttu-id="9d7c4-173">数値</span><span class="sxs-lookup"><span data-stu-id="9d7c4-173">Number</span></span>](number.md)
    
- [<span data-ttu-id="9d7c4-174">型 (string)</span><span class="sxs-lookup"><span data-stu-id="9d7c4-174">Type (string)</span></span>](type-string.md)
    
- [<span data-ttu-id="9d7c4-175">会社名</span><span class="sxs-lookup"><span data-stu-id="9d7c4-175">CompanyNames</span></span>](companynames.md)
    
## <a name="getpersona-operation-error-response"></a><span data-ttu-id="9d7c4-176">GetPersona operation のエラー応答</span><span class="sxs-lookup"><span data-stu-id="9d7c4-176">GetPersona operation error response</span></span>

<span data-ttu-id="9d7c4-177">次の例は、 **Getpersona**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-177">The following example shows an error response to a **GetPersona** operation request.</span></span> <span data-ttu-id="9d7c4-178">これは、誤って指定されたペルソナ識別子を含む要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-178">This is a response to a request that contains an incorrectly specified persona identifier.</span></span> 
  
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
      <GetPersonaResponseMessage ResponseClass="Error" 
                                 xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <MessageText>Id is malformed.</MessageText>
         <ResponseCode>ErrorInvalidIdMalformed</ResponseCode>
         <DescriptiveLinkKey>0</DescriptiveLinkKey>
      </GetPersonaResponseMessage>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="9d7c4-179">エラー応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="9d7c4-179">The error response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="9d7c4-180">GetPersonaResponseMessage</span><span class="sxs-lookup"><span data-stu-id="9d7c4-180">GetPersonaResponseMessage</span></span>](getpersonaresponsemessage.md)
    
- [<span data-ttu-id="9d7c4-181">MessageText</span><span class="sxs-lookup"><span data-stu-id="9d7c4-181">MessageText</span></span>](messagetext.md)
    
- [<span data-ttu-id="9d7c4-182">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="9d7c4-182">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="9d7c4-183">DescriptiveLinkKey</span><span class="sxs-lookup"><span data-stu-id="9d7c4-183">DescriptiveLinkKey</span></span>](descriptivelinkkey.md)
    
<span data-ttu-id="9d7c4-184">EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)</span><span class="sxs-lookup"><span data-stu-id="9d7c4-184">For additional error codes that are generic to EWS and specific to this operation, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="9d7c4-185">関連項目</span><span class="sxs-lookup"><span data-stu-id="9d7c4-185">See also</span></span>

- [<span data-ttu-id="9d7c4-186">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="9d7c4-186">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
    
- [<span data-ttu-id="9d7c4-187">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="9d7c4-187">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="9d7c4-188">FindPeople 操作</span><span class="sxs-lookup"><span data-stu-id="9d7c4-188">FindPeople operation</span></span>](findpeople-operation.md)
    

