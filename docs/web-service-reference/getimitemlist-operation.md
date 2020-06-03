---
title: GetImItemList 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: e31d14e1-0c1f-4b69-98b7-157d59c13698
description: GetImItemList EWS 操作についての情報を検索します。
ms.openlocfilehash: aabe84054b93e7de8af6145942493a0224932e45
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44456067"
---
# <a name="getimitemlist-operation"></a><span data-ttu-id="54f6d-103">GetImItemList 操作</span><span class="sxs-lookup"><span data-stu-id="54f6d-103">GetImItemList operation</span></span>

<span data-ttu-id="54f6d-104">**Getimitemlist** EWS 操作についての情報を検索します。</span><span class="sxs-lookup"><span data-stu-id="54f6d-104">Find information about the **GetImItemList** EWS operation.</span></span> 
  
## <a name="using-the-getimitemlist-operation"></a><span data-ttu-id="54f6d-105">GetImItemList 操作の使用</span><span class="sxs-lookup"><span data-stu-id="54f6d-105">Using the GetImItemList operation</span></span>

<span data-ttu-id="54f6d-106">**Getimitemlist**操作は、メールボックス内のインスタントメッセージング (im) グループと im 連絡先のペルソナの一覧を取得します。</span><span class="sxs-lookup"><span data-stu-id="54f6d-106">The **GetImItemList** operation retrieves the list of instant messaging (IM) groups and IM contact personas in a mailbox.</span></span> <span data-ttu-id="54f6d-107">**Getimitemlist**操作は引数を受け取りません。</span><span class="sxs-lookup"><span data-stu-id="54f6d-107">The **GetImItemList** operation does not take any arguments.</span></span> 
  
<span data-ttu-id="54f6d-108">この操作は Exchange Server 2013 で導入されました。</span><span class="sxs-lookup"><span data-stu-id="54f6d-108">This operation was introduced in Exchange Server 2013.</span></span>
  
### <a name="getimitemlist-operation-soap-headers"></a><span data-ttu-id="54f6d-109">GetImItemList 操作 SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54f6d-109">GetImItemList operation SOAP headers</span></span>

<span data-ttu-id="54f6d-110">**Getimitemlist**操作では、次の表に示す SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="54f6d-110">The **GetImItemList** operation can use the SOAP headers that are listed in the following table.</span></span> 
  
|<span data-ttu-id="54f6d-111">**ヘッダー名**</span><span class="sxs-lookup"><span data-stu-id="54f6d-111">**Header name**</span></span>|<span data-ttu-id="54f6d-112">**要素**</span><span class="sxs-lookup"><span data-stu-id="54f6d-112">**Element**</span></span>|<span data-ttu-id="54f6d-113">**説明**</span><span class="sxs-lookup"><span data-stu-id="54f6d-113">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="54f6d-114">**偽装**</span><span class="sxs-lookup"><span data-stu-id="54f6d-114">**Impersonation**</span></span> <br/> |[<span data-ttu-id="54f6d-115">ExchangeImpersonation</span><span class="sxs-lookup"><span data-stu-id="54f6d-115">ExchangeImpersonation</span></span>](exchangeimpersonation.md) <br/> |<span data-ttu-id="54f6d-116">クライアントアプリケーションが偽装しているユーザーを識別します。</span><span class="sxs-lookup"><span data-stu-id="54f6d-116">Identifies the user whom the client application is impersonating.</span></span> <span data-ttu-id="54f6d-117">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="54f6d-117">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="54f6d-118">**MailboxCulture**</span><span class="sxs-lookup"><span data-stu-id="54f6d-118">**MailboxCulture**</span></span> <br/> |[<span data-ttu-id="54f6d-119">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="54f6d-119">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="54f6d-120">RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。</span><span class="sxs-lookup"><span data-stu-id="54f6d-120">Identifies the culture, as defined in RFC 3066, "Tags for the Identification of Languages", to be used to access the mailbox.</span></span> <span data-ttu-id="54f6d-121">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="54f6d-121">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="54f6d-122">**RequestVersion**</span><span class="sxs-lookup"><span data-stu-id="54f6d-122">**RequestVersion**</span></span> <br/> |[<span data-ttu-id="54f6d-123">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="54f6d-123">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="54f6d-124">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="54f6d-124">Identifies the schema version for the operation request.</span></span> <span data-ttu-id="54f6d-125">このヘッダーは、要求に適用されます。</span><span class="sxs-lookup"><span data-stu-id="54f6d-125">This header is applicable to a request.</span></span>  <br/> |
|<span data-ttu-id="54f6d-126">**ServerVersion**</span><span class="sxs-lookup"><span data-stu-id="54f6d-126">**ServerVersion**</span></span> <br/> |[<span data-ttu-id="54f6d-127">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="54f6d-127">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="54f6d-128">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="54f6d-128">Identifies the version of the server that responded to the request.</span></span> <span data-ttu-id="54f6d-129">このヘッダーは応答に適用されます。</span><span class="sxs-lookup"><span data-stu-id="54f6d-129">This header is applicable to a response.</span></span>  <br/> |
   
## <a name="getimitemlist-operation-request-example-request-your-im-items-list"></a><span data-ttu-id="54f6d-130">GetImItemList 操作要求の例: IM アイテムリストの要求</span><span class="sxs-lookup"><span data-stu-id="54f6d-130">GetImItemList operation request example: Request your IM items list</span></span>

<span data-ttu-id="54f6d-131">次の**Getimitemlist**操作要求の例は、メールボックス内の im グループと im 連絡先のペルソナの一覧を要求する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="54f6d-131">The following example of a **GetImItemList** operation request shows how to request the list of IM groups and IM contact personas in a mailbox.</span></span> <span data-ttu-id="54f6d-132">**Getimitemlist**要素は、SOAP 本文の唯一の要素オプションです。</span><span class="sxs-lookup"><span data-stu-id="54f6d-132">The **GetImItemList** element is the only element option in the SOAP body.</span></span> 
  
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
      <m:GetImItemList/>
   </soap:Body>
</soap:Envelope>
```

<span data-ttu-id="54f6d-133">要求 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="54f6d-133">The request SOAP body contains the following element:</span></span>
  
- [<span data-ttu-id="54f6d-134">GetImItemList</span><span class="sxs-lookup"><span data-stu-id="54f6d-134">GetImItemList</span></span>](getimitemlist.md)
    
## <a name="successful-getimitemlist-operation-response"></a><span data-ttu-id="54f6d-135">成功した GetImItemList 操作の応答</span><span class="sxs-lookup"><span data-stu-id="54f6d-135">Successful GetImItemList operation response</span></span>

<span data-ttu-id="54f6d-136">次の例は、 **Getimitemlist**操作要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="54f6d-136">The following example shows a successful response to a **GetImItemList** operation request.</span></span> <span data-ttu-id="54f6d-137">応答には、4つの IM グループが含まれます。</span><span class="sxs-lookup"><span data-stu-id="54f6d-137">The response contains four IM groups.</span></span> <span data-ttu-id="54f6d-138">3つの IM グループ (その他の連絡先、タグ付きおよびお気に入り) は、Exchange ストア内の既定のグループです。</span><span class="sxs-lookup"><span data-stu-id="54f6d-138">Three of the IM groups — Other Contacts, Tagged, and Favorites — are default groups in the Exchange store.</span></span> <span data-ttu-id="54f6d-139">MyCustomGroup2 グループは、ユーザーが作成したカスタムグループです。</span><span class="sxs-lookup"><span data-stu-id="54f6d-139">The MyCustomGroup2 group is a custom user-created group.</span></span> <span data-ttu-id="54f6d-140">他の連絡先とタグ付きグループにはメンバーがありません。</span><span class="sxs-lookup"><span data-stu-id="54f6d-140">The Other Contacts and Tagged groups do not have members.</span></span> <span data-ttu-id="54f6d-141">お気に入りグループには、単一の連絡先メンバーがあります。</span><span class="sxs-lookup"><span data-stu-id="54f6d-141">The Favorites group has a single contact member.</span></span> <span data-ttu-id="54f6d-142">MyCustomGroup2 には、2つのメンバーの連絡先があります。</span><span class="sxs-lookup"><span data-stu-id="54f6d-142">The MyCustomGroup2 has two member contacts.</span></span> <span data-ttu-id="54f6d-143">その後の**GetItem**要求を実行して、IM 連絡先に関する詳細情報を取得できるように、アイテムの識別子が提供されます。</span><span class="sxs-lookup"><span data-stu-id="54f6d-143">The item identifiers are provided so that subsequent **GetItem** requests can be performed to get more information about the IM contacts.</span></span> 
  
<span data-ttu-id="54f6d-144">この例では、2つのペルソナを返します。</span><span class="sxs-lookup"><span data-stu-id="54f6d-144">This example returns two personas.</span></span> <span data-ttu-id="54f6d-145">最初のペルソナは、Anthony Smith と Tony Smith という2つの連絡先アイテムを表します。</span><span class="sxs-lookup"><span data-stu-id="54f6d-145">The first persona represents two contact items: Anthony Smith and Tony Smith.</span></span> <span data-ttu-id="54f6d-146">複合された連絡先情報は、 **Persona**オブジェクトで返されます。</span><span class="sxs-lookup"><span data-stu-id="54f6d-146">The combined contact information is returned in the **Persona** object.</span></span> <span data-ttu-id="54f6d-147">2番目のペルソナは、Terence の表示名を持つ単一の連絡先を表します。</span><span class="sxs-lookup"><span data-stu-id="54f6d-147">The second persona represents a single contact with the display name of Terence Adams.</span></span> 
  
> [!NOTE]
> <span data-ttu-id="54f6d-148">読みやすくするために、Exchange ストア識別子、アイテム識別子、ソース識別子、フォルダー識別子、およびペルソナ識別子が短縮されています。</span><span class="sxs-lookup"><span data-stu-id="54f6d-148">The Exchange store identifiers, item identifiers, source identifiers, folder identifiers, and persona identifiers have been shortened to preserve readability.</span></span> 
  
```XML
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
      <GetImItemListResponse ResponseClass="Success" 
                             xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
         <ResponseCode>NoError</ResponseCode>
         <ImItemList>
            <Groups xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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
            <Personas xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
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

<span data-ttu-id="54f6d-149">応答 SOAP 本文には、次の要素が含まれています。</span><span class="sxs-lookup"><span data-stu-id="54f6d-149">The response SOAP body contains the following elements:</span></span>
  
- [<span data-ttu-id="54f6d-150">GetImItemListResponse</span><span class="sxs-lookup"><span data-stu-id="54f6d-150">GetImItemListResponse</span></span>](getimitemlistresponse.md)
    
- [<span data-ttu-id="54f6d-151">ResponseCode</span><span class="sxs-lookup"><span data-stu-id="54f6d-151">ResponseCode</span></span>](responsecode.md)
    
- [<span data-ttu-id="54f6d-152">ImItemList</span><span class="sxs-lookup"><span data-stu-id="54f6d-152">ImItemList</span></span>](imitemlist.md)
    
- [<span data-ttu-id="54f6d-153">DisplayName (文字列)</span><span class="sxs-lookup"><span data-stu-id="54f6d-153">DisplayName (string)</span></span>](displayname-string.md)
    
- [<span data-ttu-id="54f6d-154">GroupType</span><span class="sxs-lookup"><span data-stu-id="54f6d-154">GroupType</span></span>](grouptype.md)
    
- [<span data-ttu-id="54f6d-155">ExchangeStoreId</span><span class="sxs-lookup"><span data-stu-id="54f6d-155">ExchangeStoreId</span></span>](exchangestoreid.md)
    
- [<span data-ttu-id="54f6d-156">MemberCorrelationKey</span><span class="sxs-lookup"><span data-stu-id="54f6d-156">MemberCorrelationKey</span></span>](membercorrelationkey.md)
    
- [<span data-ttu-id="54f6d-157">ItemId</span><span class="sxs-lookup"><span data-stu-id="54f6d-157">ItemId</span></span>](itemid.md)
    
- [<span data-ttu-id="54f6d-158">ペルソナ</span><span class="sxs-lookup"><span data-stu-id="54f6d-158">Personas</span></span>](personas-ex15websvcsotherref.md)
    
- [<span data-ttu-id="54f6d-159">PersonaId</span><span class="sxs-lookup"><span data-stu-id="54f6d-159">PersonaId</span></span>](personaid.md)
    
- [<span data-ttu-id="54f6d-160">個人の Atype</span><span class="sxs-lookup"><span data-stu-id="54f6d-160">PersonaType</span></span>](personatype.md)
    
- [<span data-ttu-id="54f6d-161">CreationTime</span><span class="sxs-lookup"><span data-stu-id="54f6d-161">CreationTime</span></span>](creationtime.md)
    
- [<span data-ttu-id="54f6d-162">DisplayNameFirstLast</span><span class="sxs-lookup"><span data-stu-id="54f6d-162">DisplayNameFirstLast</span></span>](displaynamefirstlast.md)
    
- [<span data-ttu-id="54f6d-163">DisplayNameLastFirst</span><span class="sxs-lookup"><span data-stu-id="54f6d-163">DisplayNameLastFirst</span></span>](displaynamelastfirst.md)
    
- [<span data-ttu-id="54f6d-164">FileAs</span><span class="sxs-lookup"><span data-stu-id="54f6d-164">FileAs</span></span>](fileas.md)
    
- [<span data-ttu-id="54f6d-165">FileAsId</span><span class="sxs-lookup"><span data-stu-id="54f6d-165">FileAsId</span></span>](fileasid.md)
    
- [<span data-ttu-id="54f6d-166">GivenName</span><span class="sxs-lookup"><span data-stu-id="54f6d-166">GivenName</span></span>](givenname.md)
    
- [<span data-ttu-id="54f6d-167">姓</span><span class="sxs-lookup"><span data-stu-id="54f6d-167">Surname</span></span>](surname.md)
    
- [<span data-ttu-id="54f6d-168">EmailAddress (非 Emptystringtype)</span><span class="sxs-lookup"><span data-stu-id="54f6d-168">EmailAddress (NonEmptyStringType)</span></span>](emailaddress-nonemptystringtype.md)
    
- [<span data-ttu-id="54f6d-169">Name (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="54f6d-169">Name (EmailAddressType)</span></span>](name-emailaddresstype.md)
    
- [<span data-ttu-id="54f6d-170">RoutingType (EmailAddressType)</span><span class="sxs-lookup"><span data-stu-id="54f6d-170">RoutingType (EmailAddressType)</span></span>](routingtype-emailaddresstype.md)
    
- [<span data-ttu-id="54f6d-171">EmailAddresses (ArrayOfEmailAddressesType)</span><span class="sxs-lookup"><span data-stu-id="54f6d-171">EmailAddresses (ArrayOfEmailAddressesType)</span></span>](emailaddresses-arrayofemailaddressestype.md)
    
- [<span data-ttu-id="54f6d-172">ImAddress (文字列)</span><span class="sxs-lookup"><span data-stu-id="54f6d-172">ImAddress (String)</span></span>](imaddress-string.md)
    
- [<span data-ttu-id="54f6d-173">RelevanceScore</span><span class="sxs-lookup"><span data-stu-id="54f6d-173">RelevanceScore</span></span>](relevancescore.md)
    
- [<span data-ttu-id="54f6d-174">Attributions (ArrayOfPersonaAttributionsType)</span><span class="sxs-lookup"><span data-stu-id="54f6d-174">Attributions (ArrayOfPersonaAttributionsType)</span></span>](attributions-arrayofpersonaattributionstype.md)
    
- [<span data-ttu-id="54f6d-175">属性 (PersonaAttributionType)</span><span class="sxs-lookup"><span data-stu-id="54f6d-175">Attribution (PersonaAttributionType)</span></span>](attribution-personaattributiontype.md)
    
- [<span data-ttu-id="54f6d-176">ID (文字列)</span><span class="sxs-lookup"><span data-stu-id="54f6d-176">ID (String)</span></span>](id-string.md)
    
- [<span data-ttu-id="54f6d-177">SourceId</span><span class="sxs-lookup"><span data-stu-id="54f6d-177">SourceId</span></span>](sourceid.md)
    
- [<span data-ttu-id="54f6d-178">IsWritable 可能</span><span class="sxs-lookup"><span data-stu-id="54f6d-178">IsWritable</span></span>](iswritable.md)
    
- [<span data-ttu-id="54f6d-179">IsQuickContact</span><span class="sxs-lookup"><span data-stu-id="54f6d-179">IsQuickContact</span></span>](isquickcontact.md)
    
- [<span data-ttu-id="54f6d-180">IsHidden</span><span class="sxs-lookup"><span data-stu-id="54f6d-180">IsHidden</span></span>](ishidden.md)
    
- [<span data-ttu-id="54f6d-181">FolderId</span><span class="sxs-lookup"><span data-stu-id="54f6d-181">FolderId</span></span>](folderid.md)
    
- [<span data-ttu-id="54f6d-182">StringAttributedValue</span><span class="sxs-lookup"><span data-stu-id="54f6d-182">StringAttributedValue</span></span>](stringattributedvalue.md)
    
- [<span data-ttu-id="54f6d-183">FileAses</span><span class="sxs-lookup"><span data-stu-id="54f6d-183">FileAses</span></span>](fileases.md)
    
- [<span data-ttu-id="54f6d-184">FileAsIds</span><span class="sxs-lookup"><span data-stu-id="54f6d-184">FileAsIds</span></span>](fileasids.md)
    
- [<span data-ttu-id="54f6d-185">与えた名前</span><span class="sxs-lookup"><span data-stu-id="54f6d-185">GivenNames</span></span>](givennames.md)
    
- [<span data-ttu-id="54f6d-186">Surnames</span><span class="sxs-lookup"><span data-stu-id="54f6d-186">Surnames</span></span>](surnames.md)
    
- [<span data-ttu-id="54f6d-187">ホーム電話</span><span class="sxs-lookup"><span data-stu-id="54f6d-187">HomePhones</span></span>](homephones.md)
    
- [<span data-ttu-id="54f6d-188">PhoneNumberAttributedValue</span><span class="sxs-lookup"><span data-stu-id="54f6d-188">PhoneNumberAttributedValue</span></span>](phonenumberattributedvalue.md)
    
- [<span data-ttu-id="54f6d-189">MobilePhones</span><span class="sxs-lookup"><span data-stu-id="54f6d-189">MobilePhones</span></span>](mobilephones.md)
    
- [<span data-ttu-id="54f6d-190">Emails1</span><span class="sxs-lookup"><span data-stu-id="54f6d-190">Emails1</span></span>](emails1.md)
    
- [<span data-ttu-id="54f6d-191">EmailAddressAttributedValue</span><span class="sxs-lookup"><span data-stu-id="54f6d-191">EmailAddressAttributedValue</span></span>](emailaddressattributedvalue.md)
    
- [<span data-ttu-id="54f6d-192">ImAddresses</span><span class="sxs-lookup"><span data-stu-id="54f6d-192">ImAddresses</span></span>](imaddresses.md)
    
- [<span data-ttu-id="54f6d-193">Value (ExtendedPropertyType)</span><span class="sxs-lookup"><span data-stu-id="54f6d-193">Value (ExtendedPropertyType)</span></span>](value-extendedpropertytype.md)
    
## <a name="getimitemlist-operation-error-response"></a><span data-ttu-id="54f6d-194">GetImItemList 操作エラー応答</span><span class="sxs-lookup"><span data-stu-id="54f6d-194">GetImItemList operation error response</span></span>

<span data-ttu-id="54f6d-195">次の例は、 **Getimitemlist**操作要求へのエラー応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="54f6d-195">The following example shows an error response to a **GetImItemList** operation request.</span></span> <span data-ttu-id="54f6d-196">これは、SOAP ヘッダーに誤って要求されたサーバーバージョンが含まれる要求に対する応答です。</span><span class="sxs-lookup"><span data-stu-id="54f6d-196">This is a response to a request that contains an incorrect requested server version in the SOAP header.</span></span> <span data-ttu-id="54f6d-197">このエラー応答は SOAP 違反であり、EWS スキーマでは表示されません。</span><span class="sxs-lookup"><span data-stu-id="54f6d-197">This error response is a SOAP fault and is not represented in the EWS schema.</span></span> 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
   <s:Body>
      <s:Fault>
         <faultcode xmlns:a="https://schemas.microsoft.com/exchange/services/2006/types">a:ErrorIncorrectSchemaVersion</faultcode>
         <faultstring xml:lang="en-US">The request is valid but does not specify the correct server version in the RequestServerVersion SOAP header.  Ensure that the RequestServerVersion SOAP header is set with the correct RequestServerVersionValue.</faultstring>
         <detail>
            <e:ResponseCode xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">ErrorIncorrectSchemaVersion</e:ResponseCode>
            <e:Message xmlns:e="https://schemas.microsoft.com/exchange/services/2006/errors">The request is valid but does not specify the correct server version in the RequestServerVersion SOAP header.  Ensure that the RequestServerVersion SOAP header is set with the correct RequestServerVersionValue.</e:Message>
         </detail>
      </s:Fault>
   </s:Body>
</s:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="54f6d-198">関連項目</span><span class="sxs-lookup"><span data-stu-id="54f6d-198">See also</span></span>

- [<span data-ttu-id="54f6d-199">AddImGroup 操作</span><span class="sxs-lookup"><span data-stu-id="54f6d-199">AddImGroup operation</span></span>](addimgroup-operation.md)
    
- [<span data-ttu-id="54f6d-200">Exchange 内の EWS のユーザーと連絡先</span><span class="sxs-lookup"><span data-stu-id="54f6d-200">People and contacts in EWS in Exchange</span></span>](https://msdn.microsoft.com/library/043c33be-a0d1-4bad-a840-85715eda4813%28Office.15%29.aspx)
    
- [<span data-ttu-id="54f6d-201">GetImItems 操作</span><span class="sxs-lookup"><span data-stu-id="54f6d-201">GetImItems operation</span></span>](getimitems-operation.md)
    

