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
description: GetServerTimeZones 操作は、Exchange サーバーで使用可能なタイムゾーン定義からの情報を返します。
ms.openlocfilehash: 1afe7fe13501af4a14f72c731703fe41e1f33049
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44460541"
---
# <a name="getservertimezones-operation"></a><span data-ttu-id="0b797-103">GetServerTimeZones 操作</span><span class="sxs-lookup"><span data-stu-id="0b797-103">GetServerTimeZones operation</span></span>

<span data-ttu-id="0b797-104">**GetServerTimeZones**操作は、Exchange サーバーで使用可能なタイムゾーン定義からの情報を返します。</span><span class="sxs-lookup"><span data-stu-id="0b797-104">The **GetServerTimeZones** operation returns information from time zone definitions that are available on an Exchange server.</span></span> 
  
## <a name="soap-headers"></a><span data-ttu-id="0b797-105">SOAP ヘッダー</span><span class="sxs-lookup"><span data-stu-id="0b797-105">SOAP Headers</span></span>

<span data-ttu-id="0b797-106">**GetServerTimeZones**操作では、次の表に記載されている SOAP ヘッダーを使用できます。</span><span class="sxs-lookup"><span data-stu-id="0b797-106">The **GetServerTimeZones** operation can use the SOAP headers that are listed and described in the following table.</span></span> 
  
|<span data-ttu-id="0b797-107">**Header**</span><span class="sxs-lookup"><span data-stu-id="0b797-107">**Header**</span></span>|<span data-ttu-id="0b797-108">**要素**</span><span class="sxs-lookup"><span data-stu-id="0b797-108">**Element**</span></span>|<span data-ttu-id="0b797-109">**説明**</span><span class="sxs-lookup"><span data-stu-id="0b797-109">**Description**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="0b797-110">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="0b797-110">MailboxCulture</span></span>  <br/> |[<span data-ttu-id="0b797-111">MailboxCulture</span><span class="sxs-lookup"><span data-stu-id="0b797-111">MailboxCulture</span></span>](mailboxculture.md) <br/> |<span data-ttu-id="0b797-112">メールボックスへのアクセスに使用する RFC3066 カルチャを指定します。</span><span class="sxs-lookup"><span data-stu-id="0b797-112">Identifies the RFC3066 culture to be used to access the mailbox.</span></span>  <br/> |
|<span data-ttu-id="0b797-113">RequestVersion</span><span class="sxs-lookup"><span data-stu-id="0b797-113">RequestVersion</span></span>  <br/> |[<span data-ttu-id="0b797-114">RequestServerVersion</span><span class="sxs-lookup"><span data-stu-id="0b797-114">RequestServerVersion</span></span>](requestserverversion.md) <br/> |<span data-ttu-id="0b797-115">操作要求のスキーマバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="0b797-115">Identifies the schema version for the operation request.</span></span>  <br/> |
|<span data-ttu-id="0b797-116">ServerVersion</span><span class="sxs-lookup"><span data-stu-id="0b797-116">ServerVersion</span></span>  <br/> |[<span data-ttu-id="0b797-117">ServerVersionInfo</span><span class="sxs-lookup"><span data-stu-id="0b797-117">ServerVersionInfo</span></span>](serverversioninfo.md) <br/> |<span data-ttu-id="0b797-118">要求に応答したサーバーのバージョンを識別します。</span><span class="sxs-lookup"><span data-stu-id="0b797-118">Identifies the version of the server that responded to the request.</span></span>  <br/> |
   
## <a name="getservertimezones-request-examples"></a><span data-ttu-id="0b797-119">GetServerTimeZones 要求の例</span><span class="sxs-lookup"><span data-stu-id="0b797-119">GetServerTimeZones request examples</span></span>

### <a name="getting-the-name-and-identifier-of-each-time-zone"></a><span data-ttu-id="0b797-120">各タイムゾーンの名前と識別子を取得する</span><span class="sxs-lookup"><span data-stu-id="0b797-120">Getting the Name and Identifier of Each Time Zone</span></span>

<span data-ttu-id="0b797-121">次のコード例は、東部標準時と太平洋標準時のタイムゾーンの名前と識別子を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="0b797-121">The following code example shows how to retrieve the name and identifier for the Eastern Standard Time and Pacific Standard Time time zones.</span></span>
  
### <a name="code"></a><span data-ttu-id="0b797-122">コード</span><span class="sxs-lookup"><span data-stu-id="0b797-122">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="0b797-123">コメント</span><span class="sxs-lookup"><span data-stu-id="0b797-123">Comments</span></span>

<span data-ttu-id="0b797-124">各[Id (TimeZone)](id-timezone.md)要素には、要求されているタイムゾーン定義の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0b797-124">Each [Id (TimeZone)](id-timezone.md) element contains the identifier of a time zone definition that is being requested.</span></span> <span data-ttu-id="0b797-125">すべてのタイムゾーンに関する情報を要求するには、要求から[Ids](ids.md)要素を省略します。</span><span class="sxs-lookup"><span data-stu-id="0b797-125">To request information for all time zones, omit the [Ids](ids.md) element from the request.</span></span> 
  
### <a name="getting-the-full-definition-of-each-time-zone"></a><span data-ttu-id="0b797-126">各タイムゾーンの完全な定義を取得する</span><span class="sxs-lookup"><span data-stu-id="0b797-126">Getting the Full Definition of Each Time Zone</span></span>

<span data-ttu-id="0b797-127">次のコード例は、東部標準時タイムゾーンの全タイムゾーン定義を取得する方法を示しています。</span><span class="sxs-lookup"><span data-stu-id="0b797-127">The following code example shows how to retrieve the full time zone definition for the Eastern Standard Time time zone.</span></span>
  
### <a name="code"></a><span data-ttu-id="0b797-128">コード</span><span class="sxs-lookup"><span data-stu-id="0b797-128">Code</span></span>

```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
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

### <a name="comments"></a><span data-ttu-id="0b797-129">コメント</span><span class="sxs-lookup"><span data-stu-id="0b797-129">Comments</span></span>

<span data-ttu-id="0b797-130">各[Id (TimeZone)](id-timezone.md)要素には、要求されているタイムゾーン定義の識別子が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0b797-130">Each [Id (TimeZone)](id-timezone.md) element contains the identifier of a time zone definition that is being requested.</span></span> <span data-ttu-id="0b797-131">すべてのタイムゾーンに関する情報を要求するには、要求から[Ids](ids.md)要素を省略します。</span><span class="sxs-lookup"><span data-stu-id="0b797-131">To request information for all time zones, omit the [Ids](ids.md) element from the request.</span></span> 
  
## <a name="getservertimezones-response-examples"></a><span data-ttu-id="0b797-132">GetServerTimeZones 応答の例</span><span class="sxs-lookup"><span data-stu-id="0b797-132">GetServerTimeZones response examples</span></span>

### <a name="receiving-the-time-zone-name-and-identifier-only"></a><span data-ttu-id="0b797-133">タイムゾーンの名前と識別子のみを受信する</span><span class="sxs-lookup"><span data-stu-id="0b797-133">Receiving the Time Zone Name and Identifier Only</span></span>

<span data-ttu-id="0b797-134">**GetServerTimeZones** response の次の例は、 **ReturnFullTimeZoneData**属性が**false**に設定されている**GetServerTimeZones**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="0b797-134">The following example of a **GetServerTimeZones** response shows a successful response to a **GetServerTimeZones** request in which the **ReturnFullTimeZoneData** attribute was set to **false**.</span></span> <span data-ttu-id="0b797-135">応答には、東部標準時と太平洋標準時のタイムゾーンの名前と識別子が含まれます。</span><span class="sxs-lookup"><span data-stu-id="0b797-135">The response contains the name and identifier for the Eastern Standard Time and Pacific Standard Time time zones.</span></span>
  
### <a name="code"></a><span data-ttu-id="0b797-136">コード</span><span class="sxs-lookup"><span data-stu-id="0b797-136">Code</span></span>

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
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetServerTimeZonesResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

### <a name="receiving-a-full-time-zone-definition"></a><span data-ttu-id="0b797-137">完全なタイムゾーン定義を受信する</span><span class="sxs-lookup"><span data-stu-id="0b797-137">Receiving a Full Time Zone Definition</span></span>

<span data-ttu-id="0b797-138">**GetServerTimeZones** response の次の例は、 **ReturnFullTimeZoneData**属性が**true**に設定されている**GetServerTimeZones**要求に対する正常な応答を示しています。</span><span class="sxs-lookup"><span data-stu-id="0b797-138">The following example of a **GetServerTimeZones** response shows a successful response to a **GetServerTimeZones** request in which the **ReturnFullTimeZoneData** attribute was set to **true**.</span></span> <span data-ttu-id="0b797-139">応答には、東部標準時 (東部標準時) タイムゾーンの完全なタイムゾーン定義が含まれています。</span><span class="sxs-lookup"><span data-stu-id="0b797-139">The response contains the full time zone definition for the Eastern Standard Time time zone.</span></span>
  
### <a name="code"></a><span data-ttu-id="0b797-140">コード</span><span class="sxs-lookup"><span data-stu-id="0b797-140">Code</span></span>

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
                         xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" />
  </soap:Header>
  <soap:Body>
    <GetServerTimeZonesResponse xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types"
                                xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="see-also"></a><span data-ttu-id="0b797-141">関連項目</span><span class="sxs-lookup"><span data-stu-id="0b797-141">See also</span></span>



[<span data-ttu-id="0b797-142">GetServerTimeZones</span><span class="sxs-lookup"><span data-stu-id="0b797-142">GetServerTimeZones</span></span>](getservertimezones.md)
  
[<span data-ttu-id="0b797-143">GetServerTimeZonesResponse</span><span class="sxs-lookup"><span data-stu-id="0b797-143">GetServerTimeZonesResponse</span></span>](getservertimezonesresponse.md)
  
 <span data-ttu-id="0b797-144">**GetServerTimeZonesType**</span><span class="sxs-lookup"><span data-stu-id="0b797-144">**GetServerTimeZonesType**</span></span>


[<span data-ttu-id="0b797-145">Exchange での EWS 操作</span><span class="sxs-lookup"><span data-stu-id="0b797-145">EWS operations in Exchange</span></span>](ews-operations-in-exchange.md)
  
- [<span data-ttu-id="0b797-146">Exchange の EWS XML 要素</span><span class="sxs-lookup"><span data-stu-id="0b797-146">EWS XML elements in Exchange</span></span>](ews-xml-elements-in-exchange.md)

