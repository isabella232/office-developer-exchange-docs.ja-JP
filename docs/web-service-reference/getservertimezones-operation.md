---
title: GetServerTimeZones 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- GetServerTimeZones
api_type:
- schema
ms.assetid: 680173e1-e916-466b-b573-5a3182316345
description: GetServerTimeZones 操作は、サーバー上で使用可能なタイム ゾーン定義から情報をExchangeします。
ms.openlocfilehash: f46222251729d5e82042f267d4b6293afb16de00
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59516952"
---
# <a name="getservertimezones-operation"></a>GetServerTimeZones 操作

**GetServerTimeZones** 操作は、サーバー上で使用可能なタイム ゾーン定義から情報をExchangeします。 
  
## <a name="soap-headers"></a>SOAP ヘッダー

**GetServerTimeZones** 操作では、次の表に示す SOAP ヘッダーを使用できます。 
  
|**Header**|**Element**|**説明**|
|:-----|:-----|:-----|
|MailboxCulture  <br/> |[MailboxCulture](mailboxculture.md) <br/> |メールボックスへのアクセスに使用する RFC3066 カルチャを識別します。  <br/> |
|RequestVersion  <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマ バージョンを識別します。  <br/> |
|ServerVersion  <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。  <br/> |
   
## <a name="getservertimezones-request-examples"></a>GetServerTimeZones 要求の例

### <a name="getting-the-name-and-identifier-of-each-time-zone"></a>各タイム ゾーンの名前と識別子を取得する

次のコード例は、東部標準時と太平洋標準時のタイム ゾーンの名前と識別子を取得する方法を示しています。
  
### <a name="code"></a>コード

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

### <a name="comments"></a>コメント

各 [Id (TimeZone)](id-timezone.md) 要素には、要求されているタイム ゾーン定義の識別子が含まれる。 すべてのタイム ゾーンの情報を要求するには、 [要求から Ids](ids.md) 要素を省略します。 
  
### <a name="getting-the-full-definition-of-each-time-zone"></a>各タイム ゾーンの完全な定義を取得する

次のコード例は、東部標準時ゾーンの完全なタイム ゾーン定義を取得する方法を示しています。
  
### <a name="code"></a>コード

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

### <a name="comments"></a>コメント

各 [Id (TimeZone)](id-timezone.md) 要素には、要求されているタイム ゾーン定義の識別子が含まれる。 すべてのタイム ゾーンの情報を要求するには、 [要求から Ids](ids.md) 要素を省略します。 
  
## <a name="getservertimezones-response-examples"></a>GetServerTimeZones 応答の例

### <a name="receiving-the-time-zone-name-and-identifier-only"></a>タイム ゾーン名と識別子のみ受け取る

**GetServerTimeZones** 応答の次の例は **、ReturnFullTimeZoneData** 属性が false に設定された **GetServerTimeZones** 要求に対する正常な応答を示 **しています**。 応答には、東部標準時と太平洋標準時のタイム ゾーンの名前と識別子が含まれる。
  
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

### <a name="receiving-a-full-time-zone-definition"></a>フル タイム ゾーン定義の受信

**GetServerTimeZones** 応答の次の例は **、ReturnFullTimeZoneData** 属性が true に設定された **GetServerTimeZones** 要求に対する正常な応答を示 **しています**。 応答には、東部標準時のタイム ゾーンの完全なタイム ゾーン定義が含まれる。
  
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

## <a name="see-also"></a>関連項目



[GetServerTimeZones](getservertimezones.md)
  
[GetServerTimeZonesResponse](getservertimezonesresponse.md)
  
 **GetServerTimeZonesType**


[EWS 操作 (Exchange](ews-operations-in-exchange.md)
  
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

