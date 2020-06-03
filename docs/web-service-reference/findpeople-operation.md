---
title: FindPeople 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 446106b7-ff2d-4107-90c1-29f4d38ba128
description: FindPeople EWS 操作に関する情報を検索します。
ms.openlocfilehash: ab5edc3f140e34123ce1f009c401ddd61a0e2598
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462909"
---
# <a name="findpeople-operation"></a><span data-ttu-id="901de-103">FindPeople 操作</span><span class="sxs-lookup"><span data-stu-id="901de-103">FindPeople operation</span></span>

<span data-ttu-id="901de-104">**Findpeople** EWS 操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="901de-104">Find information about the **FindPeople** EWS operation.</span></span> 
  
<span data-ttu-id="901de-105">**Findpeople**操作は、指定された連絡先フォルダーからすべての persona オブジェクトを取得するか、指定されたクエリ文字列と一致する連絡先を取得します。</span><span class="sxs-lookup"><span data-stu-id="901de-105">The **FindPeople** operation returns all persona objects from a specified Contacts folder or retrieves contacts that match a specified query string.</span></span> 
  
<span data-ttu-id="901de-106">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="901de-106">This operation was introduced in Exchange Server 2013.</span></span>
  
## <a name="using-the-findpeople-operation"></a><span data-ttu-id="901de-107">FindPeople 操作の使用</span><span class="sxs-lookup"><span data-stu-id="901de-107">Using the FindPeople operation</span></span>

<span data-ttu-id="901de-108">**Findpeople**操作は集計された連絡先情報を返します。</span><span class="sxs-lookup"><span data-stu-id="901de-108">The **FindPeople** operation returns aggregated contact information.</span></span> 
  
<span data-ttu-id="901de-109">**Findpeople**操作は、集約制限を追加し、追加のプロパティを返す機能を追加することによって、 [Restriction](restriction.md)および[baseshape](baseshape.md)複合型の既存の機能に基づいて構築されます。</span><span class="sxs-lookup"><span data-stu-id="901de-109">The **FindPeople** operation builds on the existing functionality of the [Restriction](restriction.md) and [BaseShape](baseshape.md) complex types by adding an aggregation restriction and the ability to return additional properties.</span></span> <span data-ttu-id="901de-110">制限を使用することにより、クライアントは "IM アドレスを持つ結果のみを返す" などのフィルターを指定できます。</span><span class="sxs-lookup"><span data-stu-id="901de-110">By using a restriction, a client can specify filters such as "only return results that have an IM address".</span></span> <span data-ttu-id="901de-111">既定の検索動作では、指定したユーザーの個人用メールボックスとグローバルアドレス一覧 (GAL) の両方が対象になります。</span><span class="sxs-lookup"><span data-stu-id="901de-111">The default search behavior targets both the specified user's personal mailbox and the global address list (GAL).</span></span> <span data-ttu-id="901de-112">GAL をプライマリ検索フォルダーとして検索する場合は、この操作では GAL の参照が許可されないため、制限ではなくクエリ文字列を指定する必要があります。</span><span class="sxs-lookup"><span data-stu-id="901de-112">When searching the GAL as the primary search folder, you must specify a query string instead of a restriction, because this operation does not allow for browsing of the GAL.</span></span> 
  
### <a name="findpeople-operation-soap-headers"></a><span data-ttu-id="901de-113">FindPeople 操作 SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="901de-113">FindPeople operation SOAP headers</span></span>

<span data-ttu-id="901de-114">**Findpeople**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="901de-114">The **FindPeople** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="901de-115">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="901de-115">**Header name**</span></span>|<span data-ttu-id="901de-116">**要素**</span><span class="sxs-lookup"><span data-stu-id="901de-116">**Element**</span></span>|<span data-ttu-id="901de-117">**説明**</span><span class="sxs-lookup"><span data-stu-id="901de-117">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="901de-118">**偽装**</span><span class="sxs-lookup"><span data-stu-id="901de-118">**Impersonation**</span></span> <br/> |[<span data-ttu-id="901de-119">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="901de-119">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="901de-120">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="901de-120">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="901de-121">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="901de-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="901de-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="901de-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="901de-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="901de-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="901de-124">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="901de-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="901de-125">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="901de-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="901de-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="901de-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="901de-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="901de-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="901de-128">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="901de-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="901de-129">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="901de-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="findpeople-operation-request-example"></a><span data-ttu-id="901de-130">FindPeople 操作の要求の例</span><span class="sxs-lookup"><span data-stu-id="901de-130">FindPeople operation request example</span></span>

<span data-ttu-id="901de-131">**Findpeople**操作要求の次の例は、連絡先フォルダーから最初の100の連絡先を返す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="901de-131">The following example of a **FindPeople** operation request shows how to return the first 100 contacts from the Contacts folder.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
      <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
      <m:FindPeople>
         <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
         <m:ParentFolderId>
            <t:DistinguishedFolderId Id="contacts"/>
         </m:ParentFolderId>
      </m:FindPeople>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="901de-132">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="901de-132">The request SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="901de-133">FindPeople</span><span class="sxs-lookup"><span data-stu-id="901de-133">FindPeople</span></span>](findpeople.md)
    
- [<span data-ttu-id="901de-134">IndexedPageItemView</span><span class="sxs-lookup"><span data-stu-id="901de-134">IndexedPageItemView</span></span>](indexedpageitemview.md)
    
- [<span data-ttu-id="901de-135">ParentFolderId (TargetFolderIdType)</span><span class="sxs-lookup"><span data-stu-id="901de-135">ParentFolderId (TargetFolderIdType)</span></span>](parentfolderid-targetfolderidtype.md)
    
- [<span data-ttu-id="901de-136">DistinguishedFolderId</span><span class="sxs-lookup"><span data-stu-id="901de-136">DistinguishedFolderId</span></span>](distinguishedfolderid.md)
    
<span data-ttu-id="901de-137">**Findpeople**操作要求の次の例は、クエリ文字列を使用して GAL から最初の100の連絡先を返す方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="901de-137">The following example of a **FindPeople** operation request shows how to return the first 100 contacts from the GAL by using a query string.</span></span> <span data-ttu-id="901de-138">**DistinguishedFolderId**を "directory" に設定すると、GAL がペルソナのプライマリソースとして検索されます。</span><span class="sxs-lookup"><span data-stu-id="901de-138">Setting the **DistinguishedFolderId** to "directory" will search the GAL as the primary source of personas.</span></span> 
  
```XML
<?xml version="1.0" encoding="UTF-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
   <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
   </soap:Header>
   <soap:Body >
    <m:FindPeople>
      <m:PersonaShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="persona:DisplayName"/>
          <t:FieldURI FieldURI="persona:Title"/>
        </t:AdditionalProperties>
      </m:PersonaShape>
      <m:IndexedPageItemView BasePoint="Beginning" MaxEntriesReturned="100" Offset="0"/>
      <m:ParentFolderId>
        <t:DistinguishedFolderId Id="directory"/>
      </m:ParentFolderId>
      <m:QueryString>adams</m:QueryString>
    </m:FindPeople>
  </soap:Body>
</soap:Envelope>
```

## <a name="successful-findpeople-operation-response"></a><span data-ttu-id="901de-139">成功した FindPeople 操作の応答</span><span class="sxs-lookup"><span data-stu-id="901de-139">Successful FindPeople operation response</span></span>

<span data-ttu-id="901de-140">次の例は、 **Findpeople**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="901de-140">The following example shows a successful response to a **FindPeople** operation request.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?><s:Envelope 
   xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
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
    <FindPeopleResponse ResponseClass="Success" 
                        xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <People>
        <Persona xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04ZjU5LWI3MTYzNGNkZmRkYQAQAOjFqObcLmtOlzlRnHdXQjo=" />
          <CreationTime>2012-01-11T22:25:37Z</CreationTime>
          <DisplayName>Terry Adams</DisplayName>
          <DisplayNameFirstLast>Terry Adams</DisplayNameFirstLast>
          <DisplayNameLastFirst>Adams Terry</DisplayNameLastFirst>
          <FileAs>Adams, Terry</FileAs>
          <GivenName>Terry</GivenName>
          <Surname>Adams</Surname>
          <EmailAddress>
            <Name>terry@litwareinc.com</Name>
            <EmailAddress>terry@litwareinc.com</EmailAddress>
            <RoutingType>SMTP</RoutingType>
          </EmailAddress>
          <EmailAddresses>
            <EmailAddress>
              <Name>terry@litwareinc.com</Name>
              <EmailAddress>terry@litwareinc.com</EmailAddress>
              <RoutingType>SMTP</RoutingType>
            </EmailAddress>
            <EmailAddress>
              <Name>tadams@contoso.com</Name>
              <EmailAddress>tadams@contoso.com</EmailAddress>
              <RoutingType>SMTP</RoutingType>
            </EmailAddress>
          </EmailAddresses>
          <RelevanceScore>2147483647</RelevanceScore>
        </Persona>
      </People>
      <TotalNumberOfPeopleInView>1</TotalNumberOfPeopleInView>
    </FindPeopleResponse>
  </s:Body>
</s:Envelope>
```

<span data-ttu-id="901de-141">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="901de-141">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="901de-142">FindPeopleResponse</span><span class="sxs-lookup"><span data-stu-id="901de-142">FindPeopleResponse</span></span>](findpeopleresponse.md)
    
- [<span data-ttu-id="901de-143">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="901de-143">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="901de-144">ユーザー</span><span class="sxs-lookup"><span data-stu-id="901de-144">People</span></span>](people.md)
    
- [<span data-ttu-id="901de-145">ユーザー</span><span class="sxs-lookup"><span data-stu-id="901de-145">Persona</span></span>](persona.md)
    
- [<span data-ttu-id="901de-146">PersonaId</span><span class="sxs-lookup"><span data-stu-id="901de-146">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="901de-147">CreationTime</span><span class="sxs-lookup"><span data-stu-id="901de-147">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="901de-148">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="901de-148">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="901de-149">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="901de-149">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="901de-150">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="901de-150">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="901de-151">FileAs</span><span class="sxs-lookup"><span data-stu-id="901de-151">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="901de-152">GivenName</span><span class="sxs-lookup"><span data-stu-id="901de-152">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="901de-153">姓</span><span class="sxs-lookup"><span data-stu-id="901de-153">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="901de-154">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="901de-154">EmailAddresses (ArrayOfEmailAddressesType)</span></span>](emailaddresses-arrayofemailaddressestype.md)
    
- [<span data-ttu-id="901de-155">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="901de-155">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="901de-156">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="901de-156">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="901de-157">EmailAddress (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="901de-157">EmailAddress (EmailAddressType)</span></span>](emailaddress-emailaddresstype.md)
    
- [<span data-ttu-id="901de-158">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="901de-158">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="901de-159">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="901de-159">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="901de-160">TotalNumberOfPeopleInView</span><span class="sxs-lookup"><span data-stu-id="901de-160">TotalNumberOfPeopleInView</span></span>](totalnumberofpeopleinview.md)
    
## <a name="findpeople-operation-error-response"></a><span data-ttu-id="901de-161">FindPeople 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="901de-161">FindPeople operation error response</span></span>

<span data-ttu-id="901de-162">EWS に汎用のエラーコードについては[、「応答](responsecode.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="901de-162">For error codes that are generic to EWS, see [ResponseCode](responsecode.md).</span></span>
  
## <a name="see-also"></a><span data-ttu-id="901de-163">関連項目</span><span class="sxs-lookup"><span data-stu-id="901de-163">See also</span></span>

- [<span data-ttu-id="901de-164">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="901de-164">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="901de-165">GetPersona 操作</span><span class="sxs-lookup"><span data-stu-id="901de-165">GetPersona operation</span></span>](getpersona-operation.md)
    

