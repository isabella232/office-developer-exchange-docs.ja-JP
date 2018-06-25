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
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760860"
---
# <a name="getservertimezones-operation"></a>GetServerTimeZones 操作

**GetServerTimeZones**操作では、Exchange サーバーで利用可能なタイム ゾーン定義の情報を返します。 
  
## <a name="soap-headers"></a>SOAP ヘッダー

**GetServerTimeZones**操作が一覧表示され、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**Header**|**要素**|**説明**|
|:-----|:-----|:-----|
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC3066 カルチャを使用してメールボックスへのアクセスを識別します。  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。  <br/> |
   
## <a name="getservertimezones-request-examples"></a>GetServerTimeZones 要求の例

### <a name="getting-the-name-and-identifier-of-each-time-zone"></a>名前と各タイム ゾーンの Id を取得します。

次のコード例では、名前と、東部標準時、太平洋標準時のタイム ゾーンの識別子を取得する方法を示します。
  
### <a name="code"></a>コード

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

### <a name="comments"></a>コメント

[Id (タイムゾーン)](id-timezone.md)の各要素には、要求されているタイム ゾーンの定義の識別子が含まれています。 すべてのタイム ゾーンの情報を要求するには、要求元の[Id](ids.md)要素を省略します。 
  
### <a name="getting-the-full-definition-of-each-time-zone"></a>各タイム ゾーンの完全な定義を取得します。

次のコード例では、東部標準時のタイム ゾーンのタイム ゾーン定義を取得する方法を示します。
  
### <a name="code"></a>コード

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

### <a name="comments"></a>コメント

[Id (タイムゾーン)](id-timezone.md)の各要素には、要求されているタイム ゾーンの定義の識別子が含まれています。 すべてのタイム ゾーンの情報を要求するには、要求元の[Id](ids.md)要素を省略します。 
  
## <a name="getservertimezones-response-examples"></a>GetServerTimeZones の応答の例

### <a name="receiving-the-time-zone-name-and-identifier-only"></a>のみ、タイム ゾーンの名前と識別子を受け取る

**GetServerTimeZones**の応答の例を次に**ReturnFullTimeZoneData**属性が**false**に設定された**GetServerTimeZones**要求に正常な応答を示します。 応答には、名前と、東部標準時、太平洋標準時のタイム ゾーンの識別子が含まれています。
  
### <a name="code"></a>コード

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

### <a name="receiving-a-full-time-zone-definition"></a>タイム ゾーンの定義を受信します。

**GetServerTimeZones**の応答の例を次に**ReturnFullTimeZoneData**属性が**true**に設定された**GetServerTimeZones**要求に正常な応答を示します。 応答には、東部標準時のタイム ゾーンのタイム ゾーン定義が含まれています。
  
### <a name="code"></a>コード

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

## <a name="see-also"></a>関連項目



[GetServerTimeZones](getservertimezones.md)
  
[GetServerTimeZonesResponse](getservertimezonesresponse.md)
  
 **GetServerTimeZonesType**


[Exchange での EWS の操作](ews-operations-in-exchange.md)
  
- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

