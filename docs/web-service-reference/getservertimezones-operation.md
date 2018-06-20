---
title: GetServerTimeZones 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- GetServerTimeZones
api_type:
- schema
ms.assetid: 680173e1-e916-466b-b573-5a3182316345
description: GetServerTimeZones 操作では、Exchange サーバーで利用可能なタイム ゾーン定義の情報を返します。
ms.openlocfilehash: 9b202d510a599c9082d075228be4c479a2086753
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760860"
---
# <a name="getservertimezones-operation"></a><span data-ttu-id="a15a6-103">GetServerTimeZones 操作</span><span class="sxs-lookup"><span data-stu-id="a15a6-103">GetServerTimeZones operation</span></span>

<span data-ttu-id="a15a6-104">**GetServerTimeZones**操作では、Exchange サーバーで利用可能なタイム ゾーン定義の情報を返します。</span><span class="sxs-lookup"><span data-stu-id="a15a6-104">The **GetServerTimeZones** operation returns information from time zone definitions that are available on an Exchange server.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="a15a6-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a15a6-105">SOAP Headers</span></span>

<span data-ttu-id="a15a6-106">**GetServerTimeZones**操作が一覧表示され、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="a15a6-106">The **GetServerTimeZones** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="a15a6-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="a15a6-107">**Header**</span></span>|<span data-ttu-id="a15a6-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="a15a6-108">**Element**</span></span>|<span data-ttu-id="a15a6-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="a15a6-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="a15a6-110">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="a15a6-110">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="a15a6-111">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="a15a6-111">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="a15a6-112">RFC3066 カルチャを使用してメールボックスへのアクセスを識別します。</span><span class="sxs-lookup"><span data-stu-id="a15a6-112">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="a15a6-113">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="a15a6-113">RequestVersion</span></span>  <br/> |[<span data-ttu-id="a15a6-114">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="a15a6-114">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="a15a6-115">操作要求のスキーマのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="a15a6-115">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="a15a6-116">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="a15a6-116">ServerVersion</span></span>  <br/> |[<span data-ttu-id="a15a6-117">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="a15a6-117">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="a15a6-118">要求に応答するサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="a15a6-118">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getservertimezones-request-examples"></a><span data-ttu-id="a15a6-119">GetServerTimeZones 要求の例</span><span class="sxs-lookup"><span data-stu-id="a15a6-119">GetServerTimeZones request examples</span></span>

### <a name="getting-the-name-and-identifier-of-each-time-zone"></a><span data-ttu-id="a15a6-120">名前と各タイム ゾーンの Id を取得します。</span><span class="sxs-lookup"><span data-stu-id="a15a6-120">Getting the Name and Identifier of Each Time Zone</span></span>

<span data-ttu-id="a15a6-121">次のコード例では、名前と、東部標準時、太平洋標準時のタイム ゾーンの識別子を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="a15a6-121">The following code example shows how to retrieve the name and identifier for the Eastern Standard Time and Pacific Standard Time time zones.</span></span>
  
### <a name="code"></a><span data-ttu-id="a15a6-122">コード</span><span class="sxs-lookup"><span data-stu-id="a15a6-122">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetServerTimeZones ReturnFullTimeZoneData="false">
      <m:Ids>
        <t:Id>Eastern Standard Time</Id>
        <t:Id>Pacific Standard Time</Id>
      </m:Ids>
    </m:GetServerTimeZones>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="a15a6-123">コメント</span><span class="sxs-lookup"><span data-stu-id="a15a6-123">Comments</span></span>

<span data-ttu-id="a15a6-124">[Id (タイムゾーン)](id-timezone.md)の各要素には、要求されているタイム ゾーンの定義の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a15a6-124">Each [Id (TimeZone)](id-timezone.md) element contains the identifier of a time zone definition that is being requested.</span></span> <span data-ttu-id="a15a6-125">すべてのタイム ゾーンの情報を要求するには、要求元の[Id](ids.md)要素を省略します。</span><span class="sxs-lookup"><span data-stu-id="a15a6-125">To request information for all time zones, omit the [Ids](ids.md) element from the request.</span></span> 
  
### <a name="getting-the-full-definition-of-each-time-zone"></a><span data-ttu-id="a15a6-126">各タイム ゾーンの完全な定義を取得します。</span><span class="sxs-lookup"><span data-stu-id="a15a6-126">Getting the Full Definition of Each Time Zone</span></span>

<span data-ttu-id="a15a6-127">次のコード例では、東部標準時のタイム ゾーンのタイム ゾーン定義を取得する方法を示します。</span><span class="sxs-lookup"><span data-stu-id="a15a6-127">The following code example shows how to retrieve the full time zone definition for the Eastern Standard Time time zone.</span></span>
  
### <a name="code"></a><span data-ttu-id="a15a6-128">コード</span><span class="sxs-lookup"><span data-stu-id="a15a6-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2010"/>
  </soap:Header>
  <soap:Body>
    <m:GetServerTimeZones ReturnFullTimeZoneData="true">
      <m:Ids>
        <t:Id>Eastern Standard Time</Id>
      </m:Ids>
    </m:GetServerTimeZones>
  </soap:Body>
</soap:Envelope>
```

### <a name="comments"></a><span data-ttu-id="a15a6-129">コメント</span><span class="sxs-lookup"><span data-stu-id="a15a6-129">Comments</span></span>

<span data-ttu-id="a15a6-130">[Id (タイムゾーン)](id-timezone.md)の各要素には、要求されているタイム ゾーンの定義の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a15a6-130">Each [Id (TimeZone)](id-timezone.md) element contains the identifier of a time zone definition that is being requested.</span></span> <span data-ttu-id="a15a6-131">すべてのタイム ゾーンの情報を要求するには、要求元の[Id](ids.md)要素を省略します。</span><span class="sxs-lookup"><span data-stu-id="a15a6-131">To request information for all time zones, omit the [Ids](ids.md) element from the request.</span></span> 
  
## <a name="getservertimezones-response-examples"></a><span data-ttu-id="a15a6-132">GetServerTimeZones の応答の例</span><span class="sxs-lookup"><span data-stu-id="a15a6-132">GetServerTimeZones response examples</span></span>

### <a name="receiving-the-time-zone-name-and-identifier-only"></a><span data-ttu-id="a15a6-133">のみ、タイム ゾーンの名前と識別子を受け取る</span><span class="sxs-lookup"><span data-stu-id="a15a6-133">Receiving the Time Zone Name and Identifier Only</span></span>

<span data-ttu-id="a15a6-134">**GetServerTimeZones**の応答の例を次に**ReturnFullTimeZoneData**属性が**false**に設定された**GetServerTimeZones**要求に正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="a15a6-134">The following example of a **GetServerTimeZones** response shows a successful response to a **GetServerTimeZones** request in which the **ReturnFullTimeZoneData** attribute was set to **false**.</span></span> <span data-ttu-id="a15a6-135">応答には、名前と、東部標準時、太平洋標準時のタイム ゾーンの識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a15a6-135">The response contains the name and identifier for the Eastern Standard Time and Pacific Standard Time time zones.</span></span>
  
### <a name="code"></a><span data-ttu-id="a15a6-136">コード</span><span class="sxs-lookup"><span data-stu-id="a15a6-136">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetServerTimeZonesResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetServerTimeZonesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</ResponseCode>
          <m:TimeZoneDefinitions>
            <t:TimeZoneDefinition Id="Eastern Standard Time" Name="(GMT-05:00) Eastern Time (US &amp;amp; Canada)" />
            <t:TimeZoneDefinition Id="Pacific Standard Time" Name="(GMT-08:00) Pacific Time (US &amp;amp; Canada)" />
          </m:TimeZoneDefinitions>
        </m:GetServerTimeZonesResponseMessage>
      </m:ResponseMessages>
    </m:GetServerTimeZonesResponse>
  </soap:Body>
</soap:Envelope>
```

### <a name="receiving-a-full-time-zone-definition"></a><span data-ttu-id="a15a6-137">タイム ゾーンの定義を受信します。</span><span class="sxs-lookup"><span data-stu-id="a15a6-137">Receiving a Full Time Zone Definition</span></span>

<span data-ttu-id="a15a6-138">**GetServerTimeZones**の応答の例を次に**ReturnFullTimeZoneData**属性が**true**に設定された**GetServerTimeZones**要求に正常な応答を示します。</span><span class="sxs-lookup"><span data-stu-id="a15a6-138">The following example of a **GetServerTimeZones** response shows a successful response to a **GetServerTimeZones** request in which the **ReturnFullTimeZoneData** attribute was set to **true**.</span></span> <span data-ttu-id="a15a6-139">応答には、東部標準時のタイム ゾーンのタイム ゾーン定義が含まれています。</span><span class="sxs-lookup"><span data-stu-id="a15a6-139">The response contains the full time zone definition for the Eastern Standard Time time zone.</span></span>
  
### <a name="code"></a><span data-ttu-id="a15a6-140">コード</span><span class="sxs-lookup"><span data-stu-id="a15a6-140">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/" 
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:xsd="http://www.w3.org/2001/XMLSchema">
  <soap:Header>
    <t:ServerVersionInfo MajorVersion="14" 
                         MinorVersion="0" 
                         MajorBuildNumber="639" 
                         MinorBuildNumber="11" 
                         Version="Exchange2010" 
                         xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetServerTimeZonesResponse xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages">
      <m:ResponseMessages>
        <m:GetServerTimeZonesResponseMessage ResponseClass="Success">
          <m:ResponseCode>NoError</ResponseCode>
          <m:TimeZoneDefinitions>
            <t:TimeZoneDefinition Id="Eastern Standard Time" Name="(GMT-05:00) Eastern Time (US &amp;amp; Canada)">
              <t:Periods>
                <t:Period Bias="PT5H" Name="Standard" Id="trule:Microsoft/Registry/EasternStandardTime/2006-Standard" />
                <t:Period Bias="PT4H" Name="Daylight" Id="trule:Microsoft/Registry/EasternStandardTime/2006-Daylight" />
                <t:Period Bias="PT5H" Name="Standard" Id="trule:Microsoft/Registry/EasternStandardTime/2007-Standard" />
                <t:Period Bias="PT4H" Name="Daylight" Id="trule:Microsoft/Registry/EasternStandardTime/2007-Daylight" />
              </t:Periods>
              <t:TransitionsGroups>
                <t:TransitionsGroup Id="0">
                  <t:RecurringDayTransition>
                    <t:To Kind="Period">trule:Microsoft/Registry/EasternStandardTime/2006-Daylight</t:To>
                    <t:TimeOffset>PT2H</t:TimeOffset>
                    <t:Month>4</t:Month>
                    <t:DayOfWeek>Sunday</t:DayOfWeek>
                    <t:Occurrence>1</t:Occurrence>
                  </t:RecurringDayTransition>
                  <t:RecurringDayTransition>
                    <t:To Kind="Period">trule:Microsoft/Registry/EasternStandardTime/2006-Standard</t:To>
                    <t:TimeOffset>PT2H</t:TimeOffset>
                    <t:Month>10</t:Month>
                    <t:DayOfWeek>Sunday</t:DayOfWeek>
                    <t:Occurrence>-1</t:Occurrence>
                  </t:RecurringDayTransition>
                </t:TransitionsGroup>
                <t:TransitionsGroup Id="1">
                  <t:RecurringDayTransition>
                    <t:To Kind="Period">trule:Microsoft/Registry/EasternStandardTime/2007-Daylight</t:To>
                    <t:TimeOffset>PT2H</t:TimeOffset>
                    <t:Month>3</t:Month>
                    <t:DayOfWeek>Sunday</t:DayOfWeek>
                    <t:Occurrence>2</t:Occurrence>
                  </t:RecurringDayTransition>
                  <t:RecurringDayTransition>
                    <t:To Kind="Period">trule:Microsoft/Registry/EasternStandardTime/2007-Standard</t:To>
                    <t:TimeOffset>PT2H</t:TimeOffset>
                    <t:Month>11</t:Month>
                    <t:DayOfWeek>Sunday</t:DayOfWeek>
                    <t:Occurrence>1</t:Occurrence>
                  </t:RecurringDayTransition>
                </t:TransitionsGroup>
              </t:TransitionsGroups>
              <t:Transitions>
                <t:Transition>
                  <t:To Kind="Group">0</t:To>
                </t:Transition>
                <t:AbsoluteDateTransition>
                  <t:To Kind="Group">1</t:To>
                  <t:DateTime>2007-01-01T00:00:00</t:DateTime>
                </t:AbsoluteDateTransition>
              </t:Transitions>
            </t:TimeZoneDefinition>
          </m:TimeZoneDefinitions>
        </m:GetServerTimeZonesResponseMessage>
      </m:ResponseMessages>
    </m:GetServerTimeZonesResponse>
  </soap:Body>
</soap:Envelope>
```

## <a name="see-also"></a><span data-ttu-id="a15a6-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="a15a6-141">See also</span></span>



[<span data-ttu-id="a15a6-142">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="a15a6-142">GetServerTimeZones</span></span>](getservertimezones.md)
  
[<span data-ttu-id="a15a6-143">GetServerTimeZonesResponse</span><span class="sxs-lookup"><span data-stu-id="a15a6-143">GetServerTimeZonesResponse</span></span>](getservertimezonesresponse.md)
  
 <span data-ttu-id="a15a6-144">**GetServerTimeZonesType**</span><span class="sxs-lookup"><span data-stu-id="a15a6-144">**GetServerTimeZonesType**</span></span>


[<span data-ttu-id="a15a6-145">Exchange での EWS の操作</span><span class="sxs-lookup"><span data-stu-id="a15a6-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="a15a6-146">Exchange での EWS の XML 要素</span><span class="sxs-lookup"><span data-stu-id="a15a6-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

