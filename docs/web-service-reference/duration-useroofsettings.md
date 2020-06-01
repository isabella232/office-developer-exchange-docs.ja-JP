---
title: Duration (UserOofSettings)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Duration
api_type:
- schema
ms.assetid: 01d67af3-658e-4acd-93e3-441ae827fdd3
description: Duration 要素は、OofState 要素が [スケジュール済み] に設定されている場合に、不在時 (OOF) の状態が有効である期間を指定します。
ms.openlocfilehash: 0ba0f1ea7498781c0cccb072c7ea0fa05414764c
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457299"
---
# <a name="duration-useroofsettings"></a>Duration (UserOofSettings)

**Duration**要素は、 [oofstate](oofstate.md)要素が [**スケジュール済み**] に設定されている場合に、不在時 (OOF) の状態が有効である期間を指定します。
  
```XML
<Duration>
   <StartTime/>
   <EndTime/> 
</Duration>
```

 **Duration**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[StartTime](starttime.md) <br/> |OOF 状態で設定された時間間隔の開始を表します。 この要素は必須です。  <br/> |
|[EndTime](endtime.md) <br/> |不在時の状態で設定された時間間隔の最後の部分を表します。 この要素は必須です。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[UserOofSettings](useroofsettings.md) <br/> |OOF 設定を指定します。  <br/><br/>この要素の XPath 式を次に示します。<br/><br/>`/SetUserOofSettingsRequest/UserOofSettings` <br/> |
|[OofSettings](oofsettings.md) <br/> |不在時の設定が含まれます。<br/><br/>この要素の XPath 式を次に示します。<br/><br/>`/GetUserOofSettingsResponse/OofSettings` <br/> |
|[不在](outofoffice.md) <br/> |不在 (OOF) 応答メッセージと、メールボックスの応答メッセージを送信する時間を定義します。  <br/> |
   
## <a name="remarks"></a>注釈

**期間**の種類は、 [DetailedSuggestionsWindow](detailedsuggestionswindow.md)、 [TimeWindow](timewindow.md)、および[不在](outofoffice.md)要素の型でもあります。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

[Setuseroofsettings 操作](setuseroofsettings-operation.md)要求の次の例では、 [Oofstate](oofstate.md)を**有効**にし、内部および外部の OOF メッセージを設定し、不在時の時間を10日間に設定します。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" xmlns:xsd="http://www.w3.org/2001/XMLSchema" xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Body>
    <SetUserOofSettingsRequest xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <Mailbox xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <Name>David Alexander</Name>
        <Address>someone@example.com</Address>
        <RoutingType>SMTP</RoutingType>
      </Mailbox>
      <UserOofSettings xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
        <OofState>Enabled</OofState>
        <ExternalAudience>All</ExternalAudience>
        <Duration>
          <StartTime>2005-10-05T00:00:00</StartTime>
          <EndTime>2005-10-25T00:00:00</EndTime>
        </Duration>
        <InternalReply>
          <Message>I am out of office.  This is my internal reply.</Message>
        </InternalReply>
        <ExternalReply>
          <Message>I am out of office. This is my external reply.</Message>
        </ExternalReply>
        <SetByLegacyClient>false</SetByLegacyClient>
      </UserOofSettings>
    </SetUserOofSettingsRequest>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserOofSettings 操作](getuseroofsettings-operation.md)  
- [SetUserOofSettings 操作](setuseroofsettings-operation.md)

