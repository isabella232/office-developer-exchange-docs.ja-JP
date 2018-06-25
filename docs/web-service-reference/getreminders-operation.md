---
title: GetReminders 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 1b56f83f-3b87-4b55-8259-fde6692da681
description: 操作 GetReminders EWS についての情報を検索します。
ms.openlocfilehash: 803dabf51b94dbd8fb01f2709a42ff59a597bfd1
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760843"
---
# <a name="getreminders-operation"></a>GetReminders 操作

**GetReminders** EWS の操作に関する情報を検索します。 
  
**GetReminders** Exchange Web サービス (EWS) の操作は、予定表および仕事アイテムのアラーム機能を取得します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-getreminders-operation"></a>GetReminders 操作を使用します。

**GetReminders**操作は、要求で渡される要素の値によって、ユーザーのメールボックスで、現在および将来の予定表および仕事のアイテムのアラームを取得します。 操作には、すべての現在および将来の予定表アイテムにアラームを設定するタスクを取得できます。 応答には、プライベートの予定表アイテムが含まれます。 タスク アラームなしの応答に含まれないもアラームを設定した e メールまたはフォロー アップ フラグ。 
  
現在のすべてのアラームを取得するには、**すべて**を[ReminderType](remindertype.md)と現在の時刻に[終了時刻](endtime-remindermessagedatatype.md)の設定をお勧めします。 
  
[BeginTime](begintime.md)と**終了時刻**の要素が要求に含まれている場合、応答には、任意の予定表のアラームが含まれています、**形式の BeginTime**と**終了時刻**の間に発生するアラーム設定している間に発生する作業項目。
  
**BeginTime**と**終了時刻**の要素が含まれる場合、次の表は**ReminderType**要素の動作を説明します。 
  
|* ReminderType * 要素値 * *|**説明**|
|:-----|:-----|
|All  <br/> |**BeginTime**と**終了時刻**の間で発生するアラームです。  <br/> |
|現在の  <br/> |アラームは**すべて**、によって返されるとイベントが、継続中の場合、要求された時間ウィンドウよりも前のアラームと期間に関係なくすべての予定です。  <br/> |
|古い  <br/> |アラームが-すべての予定はまだ完了していないイベント-**すべて**が返されます。 **BeginTime**と**終了時刻**の要素は、**古い**値を使用して設定してください。  <br/> |
   
### <a name="getreminders-operation-soap-headers"></a>GetReminders 操作の SOAP ヘッダー

**GetReminders**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装するユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="getreminders-operation-request-example"></a>GetReminders 操作の要求の例

**GetReminders**操作要求の次の使用例は、**形式の BeginTime**と**終了時刻**の間で発生する最初の 5 つの予定表アイテムを取得する方法を示します。
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" 
               xmlns:m="http://schemas.microsoft.com/exchange/services/2006/messages" 
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types" 
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

例要求 SOAP 本体にはには、次の要素が含まれています。
  
- [GetReminders](getreminders.md)
    
- [終了時刻](endtime-remindermessagedatatype.md)
    
- [ReminderType](remindertype.md)
    
SOAP 本体には、次の要素を含めることも。
  
- [BeginTime](begintime.md)
    
- [MaxItems](maxitems.md)
    
## <a name="successful-getreminders-operation-response"></a>GetReminders 操作の成功の応答

成功した要求への応答、 **GetReminders**操作の例を次に示します。 応答には、「チーム ミーティング」の予定表アイテムのアラームを設定し、"会議ノートを送信するタスクの「タスクのアラームが含まれています。 
  
> [!NOTE]
> 識別子は、読みやすさを保持するために短縮されています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRemindersResponse ResponseClass="Success"
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <Reminders>
        <Reminder xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
        <Reminder xmlns="http://schemas.microsoft.com/exchange/services/2006/types">
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
    
- [Subject](subject.md)
    
- [場所](location-remindermessagedatatype.md)
    
- [ReminderTime](remindertime.md)
    
- [開始日](startdate.md)
    
- [終了日](enddate-remindertype.md)
    
- [ItemId](itemid.md)
    
- [RecurringMasterItemId](recurringmasteritemid.md)
    
- [ReminderGroup](remindergroup.md)
    
- [UID](uid-remindertype.md)
    
## <a name="getreminders-operation-error-response-example"></a>GetReminders 操作のエラー応答の例

**GetReminders**操作の要求に対してエラー応答の例を次に示します。 これは、終了日が開始日より前の要求に応答します。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="918"
                       MinorBuildNumber="7"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <GetRemindersResponse ResponseClass="Error"
                          xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <MessageText>EndDate is earlier than StartDate</MessageText>
      <ResponseCode>ErrorInvalidOperation</ResponseCode>
      <DescriptiveLinkKey>0</DescriptiveLinkKey>
    </GetRemindersResponse>
  </s:Body>
</s:Envelope>
```

エラー応答 SOAP 本体にはには、次の要素が含まれています。
  
- [GetRemindersResponse](getremindersresponse.md)
    
- [MessageText](messagetext.md)
    
- [ResponseCode](responsecode.md)
    
- [DescriptiveLinkKey](descriptivelinkkey.md)
    
EWS を汎用的なこの操作に固有のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。
  
## <a name="see-also"></a>関連項目


- [PerformReminderAction](performreminderaction.md)
    

