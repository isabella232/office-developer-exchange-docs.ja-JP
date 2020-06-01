---
title: GetReminders 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b56f83f-3b87-4b55-8259-fde6692da681
description: GetReminders EWS 操作についての情報を検索します。
ms.openlocfilehash: dcbe20c674d7524a7776d374fa6964899abf472f
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458307"
---
# <a name="getreminders-operation"></a>GetReminders 操作

**Getreminders** EWS 操作についての情報を検索します。 
  
**Getreminders** Exchange Web サービス (EWS) 操作は、予定表およびタスクアイテムのアラームを取得します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-getreminders-operation"></a>GetReminders 操作の使用

**Getreminders**操作は、要求で渡された要素の値に応じて、ユーザーのメールボックス内の現在の予定表と今後の予定表およびタスクアイテムの事前通知を取得します。 この操作では、アラームが設定されているタスクだけでなく、すべての現在の予定表および今後の予定表アイテムを取得することができます。 個人用の予定表アイテムは、応答に含まれます。 アラームが設定されていないタスクは、応答には含まれません。また、アラームやフォローアップフラグが付いた電子メールには含まれません。 
  
現在のすべてのアラームを取得するには、 [ReminderType](remindertype.md)を [**すべて**] に設定し、 [EndTime](endtime-remindermessagedatatype.md)を現在の時刻に設定することをお勧めします。 
  
要求に[Begintime](begintime.md)および**EndTime**要素が含まれている場合、応答には、その間に発生する予定表およびタスクアイテムのアラームが含まれています。これらのアイテムの間には、 **begintime**と**endtime**の間に発生するアラームがあります。
  
次の表では、 **Begintime**要素と**EndTime**要素が含まれている場合の**ReminderType**要素の動作について説明します。 
  
|ReminderType * * 要素の値 * *|**説明**|
|:-----|:-----|
|すべて  <br/> |**Begintime**と**EndTime**の間に発生するアラーム。  <br/> |
|Current  <br/> |**すべて**の返信と、要求された時間枠より前のアラームに加えて、保存期間に関係なくすべての予定を表示します。  <br/> |
|古く  <br/> |完了していない**すべて**のマイナスイベントによって返されるアラーム。すべての予定を差し引いた。 **前**の値を使用するには、 **Begintime**要素と**EndTime**要素を設定する必要があります。  <br/> |
   
### <a name="getreminders-operation-soap-headers"></a>GetReminders 操作の SOAP ヘッダー

**Getreminders**操作では、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアントアプリケーションが偽装しているユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは応答に適用されます。  <br/> |
   
## <a name="getreminders-operation-request-example"></a>GetReminders 操作の要求の例

次の**Getreminders**操作要求の例は、 **Begintime**と**EndTime**の間に発生する最初の5つの予定表アイテムを取得する方法を示しています。
  
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
    
SOAP 本文には、次の要素も含めることができます。
  
- [BeginTime](begintime.md)
    
- [MaxItems](maxitems.md)
    
## <a name="successful-getreminders-operation-response"></a>成功した GetReminders 操作の応答

次の例は、 **Getreminders**操作要求に対する正常な応答を示しています。 応答には、"teams meeting" 予定表アイテムの事前通知と、"会議メモを送信するタスク" タスクに関する事前通知が含まれています。 
  
> [!NOTE]
> 読みやすくするために、識別子が短縮されています。 
  
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
    
- [場所](location-remindermessagedatatype.md)
    
- [ReminderTime](remindertime.md)
    
- [StartDate](startdate.md)
    
- [EndDate](enddate-remindertype.md)
    
- [ItemId](itemid.md)
    
- [RecurringMasterItemId](recurringmasteritemid.md)
    
- [ReminderGroup](remindergroup.md)
    
- [UID](uid-remindertype.md)
    
## <a name="getreminders-operation-error-response-example"></a>GetReminders 操作エラー応答の例

次の例は、 **Getreminders**操作要求へのエラー応答を示しています。 これは、終了日が開始日よりも前の要求に対する応答です。 
  
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
    
EWS で汎用的でこの操作に固有の追加のエラーコードについては、「応答」[を参照してください。](responsecode.md)
  
## <a name="see-also"></a>関連項目


- [PerformReminderAction](performreminderaction.md)
    

