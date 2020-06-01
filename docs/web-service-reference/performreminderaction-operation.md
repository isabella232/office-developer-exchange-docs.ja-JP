---
title: PerformReminderAction 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c597bb0e-13b0-422e-9c23-970463e2a5c3
description: PerformReminderAction EWS 操作についての情報を検索します。
ms.openlocfilehash: 4c069d541e9a42167c447a50c405399958d3608d
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44462291"
---
# <a name="performreminderaction-operation"></a>PerformReminderAction 操作

**PerformReminderAction** EWS 操作についての情報を検索します。 
  
**PerformReminderAction** Exchange Web サービス (EWS) の操作によって、アラームの [消去] または [再通知] アクションが開始されます。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-performreminderaction-operation"></a>PerformReminderAction 操作の使用

**PerformReminderAction**操作を使用して、 [getreminders](getreminders-operation.md)操作によって返されるアラームを消去または再通知 (遅延) することができます。 アラームを再通知するには、「再**通知**」に「 [NewReminderTime](newremindertime.md) [」の値](actiontype-reminderactiontype.md)を設定し、現在の[ReminderTime](remindertime.md)より後の時刻に設定します。それ以外の場合は、 **NewReminderTime**はサーバーによって無視されます。 アラームが定期的な会議の発生を対象としていて、アラームに対して次の発生のアラームを過ぎている**NewReminderTime**を使用して再**通知**が行われる場合、アラームは実際には消去されます。 
  
アラームを消すには、 **ActionType**を [**消去**] に設定します。 サーバーは、要求を処理するときに、アイテムの[IsReminderSet](isreminderset.md)値を**True**から**False**に変更します。
  
### <a name="performreminderaction-operation-soap-headers"></a>PerformReminderAction 操作の SOAP ヘッダー

**PerformReminderAction**操作では、次の表に示す SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアントアプリケーションが偽装しているユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066 で定義されているように、メールボックスへのアクセスに使用されるカルチャ (言語の識別用のタグ) を識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答したサーバーのバージョンを識別します。 このヘッダーは応答に適用されます。  <br/> |
   
## <a name="performreminderaction-operation-request-example"></a>PerformReminderAction 操作要求の例

次の**PerformReminderAction**操作要求の例は、現在のアラームを再通知し、新しいアラーム時刻を設定する方法を示しています。 [ItemId](itemid.md)の**changekey**を含める必要があります。また、 **NewReminderTime**は、 [Getreminders](getreminders-operation.md)操作によって返される**ReminderTime**より後の時刻に設定する必要があります。 
  
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
    <m:PerformReminderAction>
      <m:ReminderItemActions>
        <t:ReminderItemAction>
          <t:ActionType>Snooze</t:ActionType>
          <t:ItemId Id="vwAAAA=="
           ChangeKey="DwAAABQAAACOs0HEMq1WTKpI7sNu5qXNAAAUDA=="/>
          <t:NewReminderTime>2014-04-16T17:00:00Z</t:NewReminderTime>
        </t:ReminderItemAction>
      </m:ReminderItemActions>
    </m:PerformReminderAction>
  </soap:Body>
</soap:Envelope>
```

> [!NOTE]
> **ItemId**の値は読みやすいように短縮されています。 
  
要求 SOAP 本文には、次の要素が含まれています。
  
- [PerformReminderAction](performreminderaction.md)
    
- [ReminderItemActions](reminderitemactions.md)
    
- [ReminderItemAction](reminderitemaction.md)
    
- [ActionType](actiontype-reminderactiontype.md)
    
- [ItemId](itemid.md)
    
- [NewReminderTime](newremindertime.md)
    
## <a name="successful-performreminderaction-operation-response"></a>成功した PerformReminderAction 操作の応答

次の例は、 **PerformReminderAction**操作要求に対する正常な応答を示しています。 **Updateditemids**要素には、更新された予定表アイテムの**itemids**が含まれています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="921"
                       MinorBuildNumber="20"
                       Version="V2_10"
                       xmlns:h="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="https://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds>
        <ItemId Id="vwAAAA=="
                ChangeKey="DwAAABYAAAB4to43JyybTYwHLBM1k8MxAAAJKP+S"/>
      </UpdatedItemIds>
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

応答 SOAP 本文には、次の要素が含まれています。
  
- [PerformReminderActionResponse](performreminderactionresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [UpdatedItemIds](updateditemids.md)
    
- [ItemId](itemid.md)
    
## <a name="performreminderaction-operation-error-response-example"></a>PerformReminderAction 操作エラー応答の例

次の例は、サーバーで変更が行われていない場合の**PerformReminderAction**操作要求への応答を示しています。 これは、要求が送信されたものの、 **Updateditemids**が返されなかったこと、つまりアラームが変更されなかったことを示す応答です。 
  
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
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds />
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

エラー応答 SOAP 本文には、次の要素が含まれています。
  
- [PerformReminderActionResponse](performreminderactionresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [UpdatedItemIds](updateditemids.md)
    
EWS に汎用的なその他のエラーコードについては、「/」を[参照して](responsecode.md)ください。
  
## <a name="see-also"></a>関連項目


- [GetReminders 操作](getreminders-operation.md)
    

