---
title: GetReminders 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 1b56f83f-3b87-4b55-8259-fde6692da681
description: GetReminders EWS 操作に関する情報を検索します。
ms.openlocfilehash: e47dbb6ffceac3535bb72f93ee27bbb3f3f259e6
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513564"
---
# <a name="getreminders-operation"></a>GetReminders 操作

**GetReminders** EWS 操作に関する情報を検索します。 
  
**GetReminders Exchange** Web サービス (EWS) 操作は、予定表アイテムとタスク アイテムのアラームを取得します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-getreminders-operation"></a>GetReminders 操作の使用

**GetReminders 操作** は、要求で渡された要素の値に応じて、ユーザーのメールボックス内の現在および将来の予定表アイテムとタスク アイテムのリマインダーを取得します。 この操作では、すべての現在および将来の予定表アイテムと、アラームが設定されているタスクを取得できます。 プライベート予定表アイテムは、応答に含まれます。 リマインダーのないタスクは応答に含まれません。また、リマインダーやフォローアップ フラグを含むメールでもありません。 
  
すべての現在のアラームを取得するには[、ReminderType](remindertype.md)を Allに[、EndTime](endtime-remindermessagedatatype.md)を現在の時刻に設定することをお勧めします。 
  
[BeginTime 要素と EndTime](begintime.md)要素が要求に含まれている場合、応答には **、BeginTime** と **EndTime** の間に発生するアラームが含まれる予定表アイテムとタスク アイテムのリマインダーが含まれます。 
  
次の表では **、BeginTime** 要素と EndTime 要素が含まれている場合の **ReminderType** 要素 **の動作について** 説明します。 
  
|ReminderType** 要素の値**|**説明**|
|:-----|:-----|
|すべて  <br/> |BeginTime と **EndTime** の間で発生 **するアラーム**。  <br/> |
|Current  <br/> |**All** によって返されるアラームに加えて、イベントがまだ進行中の場合は要求されたタイム ウィンドウよりも前のリマインダーに加えて、年齢に関係なくすべての予定が返されます。  <br/> |
|Old  <br/> |All によって返される **アラーム 、** まだ完了していないイベントからすべての予定を差し引いたイベントを減算します。 **Old 値を使用** するには **、BeginTime** 要素と EndTime 要素を **設定する必要** があります。  <br/> |
   
### <a name="getreminders-operation-soap-headers"></a>GetReminders 操作 SOAP ヘッダー

**GetReminders 操作** では、次の表に示す SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**Element**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装しているユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |メールボックスへのアクセスに使用する RFC 3066「言語の識別用タグ」で定義されているカルチャを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマ バージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="getreminders-operation-request-example"></a>GetReminders 操作要求の例

**GetReminders** 操作要求の次の例は **、BeginTime** と EndTime の間に発生する最初の 5 つの予定表アイテムを取得する方法 **を示しています**。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="https://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types" 
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/">
  <soap:Header>
    <t:RequestServerVersion Version="Exchange2013" />
  </soap:Header>
  <soap:Body>
    <m:GetReminders>
      <m:EndTime>2014-04-16T21:00:00Z</m:EndTime>
      <m:ReminderType>All</m:ReminderType>
    </m:GetReminders>
  </soap:Body>
</soap:Envelope>
```

要求 SOAP 本文の例には、次の要素が含まれています。
  
- [GetReminders](getreminders.md)
    
- [EndTime](endtime-remindermessagedatatype.md)
    
- [ReminderType](remindertype.md)
    
SOAP 本文には、次の要素を含めすることもできます。
  
- [BeginTime](begintime.md)
    
- [MaxItems](maxitems.md)
    
## <a name="successful-getreminders-operation-response"></a>GetReminders 操作応答の成功

次の例は **、GetReminders 操作要求に対する** 正常な応答を示しています。 応答には、"チーム会議" 予定表アイテムのリマインダーと"会議メモを送信するタスク" タスクのリマインダーが含まれる。 
  
> [!NOTE]
> 識別子は、読みやすさを維持するために短縮されました。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRemindersResponse ResponseClass="Success"
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Reminders>
        <Reminder xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Subject>Team meeting</Subject>
          <Location />
          <ReminderTime>2014-04-15T21:00:00Z</ReminderTime>
          <StartDate>2014-04-15T21:00:00Z</StartDate>
          <EndDate>2014-04-15T21:30:00Z</EndDate>
          <ItemId Id="vQAAAA=="
                  ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAACRoV4" />
          <RecurringMasterItemId Id="K7u5AAA=" ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAACRoV0" />
          <ReminderGroup>Calendar</ReminderGroup>
          <UID>6CF2FA62</UID>
        </Reminder>
        <Reminder xmlns="https://schemas.microsoft.com/exchange/services/2006/types">
          <Subject>Task to send meeting notes</Subject>
          <Location />
          <ReminderTime>2014-04-16T14:00:00Z</ReminderTime>
          <StartDate>0001-01-02T00:00:00Z</StartDate>
          <EndDate>0001-01-02T00:00:00Z</EndDate>
          <ItemId Id="vAAAAA=="
                  ChangeKey="EwAAABQAAACOs0HEMq1WTKpI7sNu5qXNAAAIDg==" />
          <ReminderGroup>Task</ReminderGroup>
          <UID>vAAAAA==</UID>
        </Reminder>
      </Reminders>
    </GetRemindersResponse>
  </s:Body>
</s:Envelope>
```

応答 SOAP 本文には、次の要素が含まれています。
  
- [GetRemindersResponse](getremindersresponse.md)
    
- [Reminders](reminders.md)
    
- [Reminder](reminder.md)
    
- [[件名]](subject.md)
    
- [Location](location-remindermessagedatatype.md)
    
- [ReminderTime](remindertime.md)
    
- [StartDate](startdate.md)
    
- [EndDate](enddate-remindertype.md)
    
- [ItemId](itemid.md)
    
- [RecurringMasterItemId](recurringmasteritemid.md)
    
- [ReminderGroup](remindergroup.md)
    
- [UID](uid-remindertype.md)
    
## <a name="getreminders-operation-error-response-example"></a>GetReminders 操作エラー応答の例

次の例は **、GetReminders 操作要求に対するエラー応答を** 示しています。 これは、終了日が開始日より前の要求に対する応答です。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRemindersResponse ResponseClass="Error"
                          xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>EndDate is earlier than StartDate</MessageText>
      <ResponseCode>ErrorInvalidOperation</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRemindersResponse>
  </s:Body>
</s:Envelope>
```

エラー応答 SOAP 本文には、次の要素が含まれています。
  
- [GetRemindersResponse](getremindersresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
EWS に汎用的で、この操作に固有の追加のエラー コードについては [、「ResponseCode」を参照してください](responsecode.md)。
  
## <a name="see-also"></a>関連項目


- [PerformReminderAction](performreminderaction.md)
    

