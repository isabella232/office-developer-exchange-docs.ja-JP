---
title: GetImItemList 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e31d14e1-0c1f-4b69-98b7-157d59c13698
description: 操作 GetImItemList EWS についての情報を検索します。
ms.openlocfilehash: 3977b0ad31e819cd973ce261ba3152b3840003b3
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760758"
---
# <a name="getimitemlist-operation"></a><span data-ttu-id="4fc85-103">GetImItemList 操作</span><span class="sxs-lookup"><span data-stu-id="4fc85-103">GetImItemList operation</span></span>

<span data-ttu-id="4fc85-104">**GetImItemList** EWS の操作に関する情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="4fc85-104">Find information about the **GetImItemList** EWS operation.</span></span> 
  
## <a name="using-the-getimitemlist-operation"></a><span data-ttu-id="4fc85-105">GetImItemList 操作を使用します。</span><span class="sxs-lookup"><span data-stu-id="4fc85-105">Using the GetImItemList operation</span></span>

<span data-ttu-id="4fc85-106">**GetImItemList**操作は、インスタント メッセージング (IM) のグループの一覧を取得し、IM は、メールボックス内のペルソナをお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="4fc85-106">The **GetImItemList** operation retrieves the list of instant messaging (IM) groups and IM contact personas in a mailbox.</span></span> <span data-ttu-id="4fc85-107">**GetImItemList**操作には、引数になりません。</span><span class="sxs-lookup"><span data-stu-id="4fc85-107">The **GetImItemList** operation does not take any arguments.</span></span> 
  
<span data-ttu-id="4fc85-108">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="4fc85-108">This operation was introduced in Exchange Server 2013.</span></span>
  
### <a name="getimitemlist-operation-soap-headers"></a><span data-ttu-id="4fc85-109">GetImItemList 操作の SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4fc85-109">GetImItemList operation SOAP headers</span></span>

<span data-ttu-id="4fc85-110">**GetImItemList**操作は、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="4fc85-110">The **GetImItemList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="4fc85-111">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="4fc85-111">**Header name**</span></span>|<span data-ttu-id="4fc85-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="4fc85-112">**Element**</span></span>|<span data-ttu-id="4fc85-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="4fc85-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="4fc85-114">**偽装**</span><span class="sxs-lookup"><span data-stu-id="4fc85-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="4fc85-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="4fc85-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="4fc85-116">クライアント アプリケーションが偽装するユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="4fc85-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="4fc85-117">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="4fc85-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="4fc85-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="4fc85-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="4fc85-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="4fc85-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="4fc85-120">RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。</span><span class="sxs-lookup"><span data-stu-id="4fc85-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="4fc85-121">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="4fc85-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="4fc85-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="4fc85-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="4fc85-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="4fc85-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="4fc85-124">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="4fc85-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="4fc85-125">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="4fc85-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="4fc85-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="4fc85-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="4fc85-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="4fc85-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="4fc85-128">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="4fc85-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="4fc85-129">このヘッダーは、応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="4fc85-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getimitemlist-operation-request-example-request-your-im-items-list"></a><span data-ttu-id="4fc85-130">GetImItemList 操作の要求の例: IM の項目の一覧を要求します。</span><span class="sxs-lookup"><span data-stu-id="4fc85-130">GetImItemList operation request example: Request your IM items list</span></span>

<span data-ttu-id="4fc85-131">**GetImItemList**操作要求の次の使用例は、IM グループの一覧を要求する方法を示し、IM は、メールボックス内のペルソナをお問い合わせください。</span><span class="sxs-lookup"><span data-stu-id="4fc85-131">The following example of a **GetImItemList** operation request shows how to request the list of IM groups and IM contact personas in a mailbox.</span></span> <span data-ttu-id="4fc85-132">**GetImItemList**要素は、SOAP 本文での唯一の要素のオプションです。</span><span class="sxs-lookup"><span data-stu-id="4fc85-132">The **GetImItemList** element is the only element option in the SOAP body.</span></span> 
  
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
      <m:GetImItemList/>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="4fc85-133">要求 SOAP 本体にはには、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4fc85-133">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="4fc85-134">GetImItemList</span><span class="sxs-lookup"><span data-stu-id="4fc85-134">GetImItemList</span></span>](getimitemlist.md)
    
## <a name="successful-getimitemlist-operation-response"></a><span data-ttu-id="4fc85-135">GetImItemList 操作の成功の応答</span><span class="sxs-lookup"><span data-stu-id="4fc85-135">Successful GetImItemList operation response</span></span>

<span data-ttu-id="4fc85-136">成功した要求への応答、 **GetImItemList**操作の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4fc85-136">The following example shows a successful response to a **GetImItemList** operation request.</span></span> <span data-ttu-id="4fc85-137">応答には、IM の 4 つのグループが含まれています。</span><span class="sxs-lookup"><span data-stu-id="4fc85-137">The response contains four IM groups.</span></span> <span data-ttu-id="4fc85-138">IM グループの 3 つの-その他の連絡先、タグ、および [お気に入り]-は、Exchange ストア内の既定のグループです。</span><span class="sxs-lookup"><span data-stu-id="4fc85-138">Three of the IM groups — Other Contacts, Tagged, and Favorites — are default groups in the Exchange store.</span></span> <span data-ttu-id="4fc85-139">MyCustomGroup2 グループは、ユーザーが作成したユーザー設定のグループです。</span><span class="sxs-lookup"><span data-stu-id="4fc85-139">The MyCustomGroup2 group is a custom user-created group.</span></span> <span data-ttu-id="4fc85-140">その他の連絡先とタグのグループのメンバーではありません。</span><span class="sxs-lookup"><span data-stu-id="4fc85-140">The Other Contacts and Tagged groups do not have members.</span></span> <span data-ttu-id="4fc85-141">お気に入りグループは、1 つのメンバーを持っています。</span><span class="sxs-lookup"><span data-stu-id="4fc85-141">The Favorites group has a single contact member.</span></span> <span data-ttu-id="4fc85-142">MyCustomGroup2 は、2 つのメンバーの連絡先を持っています。</span><span class="sxs-lookup"><span data-stu-id="4fc85-142">The MyCustomGroup2 has two member contacts.</span></span> <span data-ttu-id="4fc85-143">アイテム識別子は、 **GetItem**の後続の要求を実行して、IM の連絡先に関する詳細情報を取得するために提供されます。</span><span class="sxs-lookup"><span data-stu-id="4fc85-143">The item identifiers are provided so that subsequent **GetItem** requests can be performed to get more information about the IM contacts.</span></span> 
  
<span data-ttu-id="4fc85-144">この例では、2 つのペルソナを返します。</span><span class="sxs-lookup"><span data-stu-id="4fc85-144">This example returns two personas.</span></span> <span data-ttu-id="4fc85-145">最初のペルソナは、2 つの連絡先アイテムを表します: アンソニー ・ スミスとトニー ・ スミス。</span><span class="sxs-lookup"><span data-stu-id="4fc85-145">The first persona represents two contact items: Anthony Smith and Tony Smith.</span></span> <span data-ttu-id="4fc85-146">**ペルソナ**オブジェクトでは、結合された連絡先の情報が返されます。</span><span class="sxs-lookup"><span data-stu-id="4fc85-146">The combined contact information is returned in the **Persona** object.</span></span> <span data-ttu-id="4fc85-147">2 番目のペルソナは、Adam は Terence の表示名を持つ 1 つの連絡先を表します。</span><span class="sxs-lookup"><span data-stu-id="4fc85-147">The second persona represents a single contact with the display name of Terence Adams.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="4fc85-148">Exchange ストア識別子、項目の識別子、送信元識別子、フォルダーの識別子、およびペルソナの識別子は、読みやすさを保持するために短縮されています。</span><span class="sxs-lookup"><span data-stu-id="4fc85-148">The Exchange store identifiers, item identifiers, source identifiers, folder identifiers, and persona identifiers have been shortened to preserve readability.</span></span> 
  
```XML
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Header>
      <h:ServerVersionInfo MajorVersion="15" 
                           MinorVersion="0" 
                           MajorBuildNumber="349" 
                           MinorBuildNumber="0" 
                           Version="Exchange2013" 
                           xmlns="http://schemas.microsoft.com/exchange/services/2006/types" 
                           xmlns:xsd="http://www.w3.org/2001/XMLSchema" 
                           xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
                           xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types" />
   </s:Header>
   <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
           xmlns:xsd="http://www.w3.org/2001/XMLSchema">
      <GetImItemListResponse ResponseClass="Success" 
                             xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImItemList>
            <Groups xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <ImGroup>
                  <DisplayName>Other Contacts</DisplayName>
                  <GroupType>IPM.DistList.MOC.OtherContacts</GroupType>
                  <ExchangeStoreId Id="AAMkAGQ1MjJjMTBkLThQoTbWAAAAAAQUAAA=" 
                                   ChangeKey="EgAAAA==" />
               </ImGroup>
               <ImGroup>
                  <DisplayName>Tagged</DisplayName>
                  <GroupType>IPM.DistList.MOC.Tagged</GroupType>
                  <ExchangeStoreId Id="AAMkAGQ1MjJAAQTAAA=" 
                                   ChangeKey="EgAAAA==" />
               </ImGroup>
               <ImGroup>
                  <DisplayName>Favorites</DisplayName>
                  <GroupType>IPM.DistList.MOC.Favorites</GroupType>
                  <ExchangeStoreId Id="AAMkAGQ1MjJjMTAAAAAQSAAA=" 
                                   ChangeKey="EgAAAA==" />
                  <MemberCorrelationKey>
                     <ItemId Id="AAMkAGQ1MjJtt/bhQoTbWAAAAAAvcAAA=" 
                             ChangeKey="EQAAAA==" />
                  </MemberCorrelationKey>
               </ImGroup>
               <ImGroup>
                  <DisplayName>MyCustomGroup2</DisplayName>
                  <GroupType>IPM.DistList.MOC.UserGroup</GroupType>
                  <ExchangeStoreId Id="AAMkAGQ1MjJjKAAA=" 
                                   ChangeKey="EgAAAA==" />
                  <MemberCorrelationKey>
                     <ItemId Id="AAMkAGQ1Matt/bhQoTbWAAAAAAvcAAA=" 
                             ChangeKey="EQAAAA==" />
                     <ItemId Id="AAMkAGQ1MjJjMTBkTbWAAAAAAveAAA=" 
                             ChangeKey="EQAAAA==" />
                  </MemberCorrelationKey>
               </ImGroup>
            </Groups>
            <Personas xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
               <Persona>
                  <PersonaId Id="AAQkAGQ1MjJjMTBkLTc4YkZmRkYQAQAFgxE1nBcqRGgYWWorM9/+s=" />
                  <PersonaType>Person</PersonaType>
                  <CreationTime>2012-01-12T22:14:36Z</CreationTime>
                  <DisplayName>Anthony Smith</DisplayName>
                  <DisplayNameFirstLast>Anthony Smith</DisplayNameFirstLast>
                  <DisplayNameLastFirst>Smith Anthony</DisplayNameLastFirst>
                  <FileAs>Smith, Anthony</FileAs>
                  <FileAsId>LastCommaFirst</FileAsId>
                  <GivenName>Anthony</GivenName>
                  <Surname>Smith</Surname>
                  <EmailAddress>
                     <Name>tsmith@contoso.com</Name>
                     <EmailAddress>tsmith@contoso.com</EmailAddress>
                     <RoutingType>SMTP</RoutingType>
                  </EmailAddress>
                  <EmailAddresses>
                     <EmailAddress>
                        <Name>tsmith@contoso.com</Name>
                        <EmailAddress>tsmith@contoso.com</EmailAddress>
                        <RoutingType>SMTP</RoutingType>
                     </EmailAddress>
                  </EmailAddresses>
                  <ImAddress>tsmith@contoso.com</ImAddress>
                  <RelevanceScore>2147483647</RelevanceScore>
                  <Attributions>
                     <Attribution>
                        <Id>0</Id>
                        <SourceId Id="AQMkAGQ1MjIAYzEwZC03OGNlLTQ5Bq239uFChNtYAAAIvDAAAAA==" 
                                  ChangeKey="EQAAABYAAABtF8oI7iVOQatt/bhQoTbWAAAAADB3" />
                        <DisplayName>Outlook</DisplayName>
                        <IsWritable>true</IsWritable>
                        <IsQuickContact>false</IsQuickContact>
                        <IsHidden>false</IsHidden>
                        <FolderId Id="AQMkAGQ1MjIAYzEMikE3AQBtF8oI7iVOQatt/bhQoTbWAAADEAAAAA==" 
                                  ChangeKey="AQAAAA==" />
                     </Attribution>
                     <Attribution>
                        <Id>1</Id>
                        <SourceId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Ny04/bhQoTbWAAAAAAveAAA=" 
                                  ChangeKey="EQAAABYAAABtF8oI7iVOQatt/bhQoTbWAAAAAAym" />
                        <DisplayName>Outlook</DisplayName>
                        <IsWritable>true</IsWritable>
                        <IsQuickContact>true</IsQuickContact>
                        <IsHidden>false</IsHidden>
                        <FolderId Id="AAMkAGQ1MjJjMTBkLTc4Y2UtNDA5Qatt/bhQoTbWAAAAAAvZAAA=" 
                                  ChangeKey="AQAAAA==" />
                     </Attribution>
                  </Attributions>
                  <DisplayNames>
                     <StringAttributedValue>
                        <Value>Anthony Smith</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                     <StringAttributedValue>
                        <Value>Tony Smith</Value>
                        <Attributions>
                           <Attribution>1</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </DisplayNames>
                  <FileAses>
                     <StringAttributedValue>
                        <Value>Smith, Anthony</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </FileAses>
                  <FileAsIds>
                     <StringAttributedValue>
                        <Value>LastCommaFirst</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                     <StringAttributedValue>
                        <Value>None</Value>
                        <Attributions>
                           <Attribution>1</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </FileAsIds>
                  <GivenNames>
                     <StringAttributedValue>
                        <Value>Anthony</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </GivenNames>
                  <Surnames>
                     <StringAttributedValue>
                        <Value>Smith</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </Surnames>
                  <HomePhones>
                     <PhoneNumberAttributedValue>
                        <Value>
                           <Number>4255550110</Number>
                           <Type>Home</Type>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </PhoneNumberAttributedValue>
                  </HomePhones>
                  <MobilePhones>
                     <PhoneNumberAttributedValue>
                        <Value>
                           <Number>4255550120</Number>
                           <Type>Mobile</Type>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </PhoneNumberAttributedValue>
                  </MobilePhones>
                  <Emails1>
                     <EmailAddressAttributedValue>
                        <Value>
                           <Name>tsmith@contoso.com</Name>
                           <EmailAddress>tsmith@contoso.com</EmailAddress>
                           <RoutingType>SMTP</RoutingType>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                           <Attribution>1</Attribution>
                        </Attributions>
                     </EmailAddressAttributedValue>
                  </Emails1>
                  <ImAddresses>
                     <StringAttributedValue>
                        <Value>tsmith@contoso.com</Value>
                        <Attributions>
                           <Attribution>1</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </ImAddresses>
               </Persona>
               <Persona>
                  <PersonaId Id="AAQkAGQ1MjJjMTBkLkYQAQAJ3EkhEEXN5KufGbSYJanZk=" />
                  <PersonaType>Person</PersonaType>
                  <CreationTime>2012-01-05T23:06:58Z</CreationTime>
                  <DisplayName>Terence Adams</DisplayName>
                  <DisplayNameFirstLast>Terence Adams</DisplayNameFirstLast>
                  <DisplayNameLastFirst>Terence Adams</DisplayNameLastFirst>
                  <FileAsId>None</FileAsId>
                  <EmailAddress>
                     <Name>Terence Adams</Name>
                     <EmailAddress>tadams@contoso.com</EmailAddress>
                     <RoutingType>SMTP</RoutingType>
                  </EmailAddress>
                  <EmailAddresses>
                     <EmailAddress>
                        <Name>Terence Adams</Name>
                        <EmailAddress>tadams@contoso.com</EmailAddress>
                        <RoutingType>SMTP</RoutingType>
                     </EmailAddress>
                  </EmailAddresses>
                  <ImAddress>tadams@contoso.com</ImAddress>
                  <RelevanceScore>2147483647</RelevanceScore>
                  <Attributions>
                     <Attribution>
                        <Id>0</Id>
                        <SourceId Id="AAMkAGQ1MjVOQatt/bhQoTbWAAAA7iVOQatt/bhQoTbWAAAAAAvcAAA=" 
                                  ChangeKey="EQAAABYAAABtF8oI7iVOQatt/bhQoTbWAAAAAAyg" />
                        <DisplayName>Outlook</DisplayName>
                        <IsWritable>true</IsWritable>
                        <IsQuickContact>true</IsQuickContact>
                        <IsHidden>false</IsHidden>
                        <FolderId Id="AAMkAGQ1MjJjMTBkLTc4Y2rBtF8oI7iVOQatt/bhQoTbWAAAAAAvZAAA=" 
                                  ChangeKey="AQAAAA==" />
                     </Attribution>
                  </Attributions>
                  <DisplayNames>
                     <StringAttributedValue>
                        <Value>Terence Adams</Value>
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
                  <Emails1>
                     <EmailAddressAttributedValue>
                        <Value>
                           <Name>Terence Adams</Name>
                           <EmailAddress>tadams@contoso.com</EmailAddress>
                           <RoutingType>SMTP</RoutingType>
                        </Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </EmailAddressAttributedValue>
                  </Emails1>
                  <ImAddresses>
                     <StringAttributedValue>
                        <Value>tadams@contoso.com</Value>
                        <Attributions>
                           <Attribution>0</Attribution>
                        </Attributions>
                     </StringAttributedValue>
                  </ImAddresses>
               </Persona>
            </Personas>
         </ImItemList>
      </GetImItemListResponse>
   </s:Body>
</s:Envelope>
```

<span data-ttu-id="4fc85-149">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="4fc85-149">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="4fc85-150">GetImItemListResponse</span><span class="sxs-lookup"><span data-stu-id="4fc85-150">GetImItemListResponse</span></span>](getimitemlistresponse.md)
    
- [<span data-ttu-id="4fc85-151">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="4fc85-151">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="4fc85-152">ImItemList</span><span class="sxs-lookup"><span data-stu-id="4fc85-152">ImItemList</span></span>](imitemlist.md)
    
- [<span data-ttu-id="4fc85-153">表示名 (文字列)</span><span class="sxs-lookup"><span data-stu-id="4fc85-153">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="4fc85-154">GroupType</span><span class="sxs-lookup"><span data-stu-id="4fc85-154">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="4fc85-155">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="4fc85-155">ExchangeStoreId</span></span>](exchangestoreid.md)
    
- [<span data-ttu-id="4fc85-156">MemberCorrelationKey</span><span class="sxs-lookup"><span data-stu-id="4fc85-156">MemberCorrelationKey</span></span>](membercorrelationkey.md)
    
- [<span data-ttu-id="4fc85-157">ItemId</span><span class="sxs-lookup"><span data-stu-id="4fc85-157">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="4fc85-158">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="4fc85-158">Personas</span></span>](personas-ex15websvcsotherref.md)
    
- [<span data-ttu-id="4fc85-159">PersonaId</span><span class="sxs-lookup"><span data-stu-id="4fc85-159">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="4fc85-160">PersonaType</span><span class="sxs-lookup"><span data-stu-id="4fc85-160">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="4fc85-161">CreationTime</span><span class="sxs-lookup"><span data-stu-id="4fc85-161">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="4fc85-162">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="4fc85-162">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="4fc85-163">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="4fc85-163">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="4fc85-164">表題</span><span class="sxs-lookup"><span data-stu-id="4fc85-164">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="4fc85-165">FileAsId</span><span class="sxs-lookup"><span data-stu-id="4fc85-165">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="4fc85-166">GivenName</span><span class="sxs-lookup"><span data-stu-id="4fc85-166">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="4fc85-167">姓</span><span class="sxs-lookup"><span data-stu-id="4fc85-167">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="4fc85-168">EmailAddress (NonEmptyStringType)</span><span class="sxs-lookup"><span data-stu-id="4fc85-168">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="4fc85-169">名 (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="4fc85-169">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="4fc85-170">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="4fc85-170">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="4fc85-171">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="4fc85-171">EmailAddresses (ArrayOfEmailAddressesType)</span></span>](emailaddresses-arrayofemailaddressestype.md)
    
- [<span data-ttu-id="4fc85-172">ImAddress (文字列)</span><span class="sxs-lookup"><span data-stu-id="4fc85-172">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="4fc85-173">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="4fc85-173">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="4fc85-174">帰属 (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="4fc85-174">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="4fc85-175">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="4fc85-175">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="4fc85-176">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="4fc85-176">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="4fc85-177">SourceId</span><span class="sxs-lookup"><span data-stu-id="4fc85-177">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="4fc85-178">IsWritable</span><span class="sxs-lookup"><span data-stu-id="4fc85-178">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="4fc85-179">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="4fc85-179">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="4fc85-180">IsHidden</span><span class="sxs-lookup"><span data-stu-id="4fc85-180">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="4fc85-181">フォルダー Id</span><span class="sxs-lookup"><span data-stu-id="4fc85-181">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="4fc85-182">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="4fc85-182">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="4fc85-183">FileAses</span><span class="sxs-lookup"><span data-stu-id="4fc85-183">FileAses</span></span>](fileases.md)
    
- [<span data-ttu-id="4fc85-184">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="4fc85-184">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="4fc85-185">GivenNames</span><span class="sxs-lookup"><span data-stu-id="4fc85-185">GivenNames</span></span>](givennames.md)
    
- [<span data-ttu-id="4fc85-186">姓</span><span class="sxs-lookup"><span data-stu-id="4fc85-186">Surnames</span></span>](surnames.md)
    
- [<span data-ttu-id="4fc85-187">HomePhones</span><span class="sxs-lookup"><span data-stu-id="4fc85-187">HomePhones</span></span>](homephones.md)
    
- [<span data-ttu-id="4fc85-188">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="4fc85-188">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="4fc85-189">MobilePhones</span><span class="sxs-lookup"><span data-stu-id="4fc85-189">MobilePhones</span></span>](mobilephones.md)
    
- [<span data-ttu-id="4fc85-190">Emails1</span><span class="sxs-lookup"><span data-stu-id="4fc85-190">Emails1</span></span>](emails1.md)
    
- [<span data-ttu-id="4fc85-191">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="4fc85-191">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
    
- [<span data-ttu-id="4fc85-192">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="4fc85-192">ImAddresses</span></span>](imaddresses.md)
    
- [<span data-ttu-id="4fc85-193">値 (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="4fc85-193">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md)
    
## <a name="getimitemlist-operation-error-response"></a><span data-ttu-id="4fc85-194">GetImItemList 操作のエラー応答</span><span class="sxs-lookup"><span data-stu-id="4fc85-194">GetImItemList operation error response</span></span>

<span data-ttu-id="4fc85-195">**GetImItemList**操作の要求に対してエラー応答の例を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4fc85-195">The following example shows an error response to a **GetImItemList** operation request.</span></span> <span data-ttu-id="4fc85-196">これは、SOAP ヘッダーで要求されたサーバーの正しくないバージョンを含む要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="4fc85-196">This is a response to a request that contains an incorrect requested server version in the SOAP header.</span></span> <span data-ttu-id="4fc85-197">このエラー応答は、SOAP 違反し、EWS のスキーマには表示されません。</span><span class="sxs-lookup"><span data-stu-id="4fc85-197">This error response is a SOAP fault and is not represented in the EWS schema.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="http://schemas.microsoft.com/exchange/services/2006/types">a:ErrorIncorrectSchemaVersion</faultcode>
         <faultstring xml:lang="en-US">The request is valid but does not specify the correct server version in the RequestServerVersion SOAP header.  Ensure that the RequestServerVersion SOAP header is set with the correct RequestServerVersionValue.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">ErrorIncorrectSchemaVersion</e:ResponseCode>
            <e:Message xmlns:e="http://schemas.microsoft.com/exchange/services/2006/errors">The request is valid but does not specify the correct server version in the RequestServerVersion SOAP header.  Ensure that the RequestServerVersion SOAP header is set with the correct RequestServerVersionValue.</e:Message>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="4fc85-198">関連項目</span><span class="sxs-lookup"><span data-stu-id="4fc85-198">See also</span></span>

- [<span data-ttu-id="4fc85-199">AddImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="4fc85-199">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="4fc85-200">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="4fc85-200">People and contacts in EWS in Exchange</span></span>](http://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="4fc85-201">GetImItems 操作</span><span class="sxs-lookup"><span data-stu-id="4fc85-201">GetImItems operation</span></span>](getimitems-operation.md)
    

