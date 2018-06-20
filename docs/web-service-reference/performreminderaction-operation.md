---
title: PerformReminderAction 操作
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: overview
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: c597bb0e-13b0-422e-9c23-970463e2a5c3
description: 操作 PerformReminderAction EWS についての情報を検索します。
ms.openlocfilehash: 778fbb508413721f58cfcf9143a5296874e6cd1c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832722"
---
# <a name="performreminderaction-operation"></a>PerformReminderAction 操作

**PerformReminderAction** EWS の操作に関する情報を検索します。 
  
**PerformReminderAction** Exchange Web サービス (EWS) 操作では、アラームのアラームを消すか、アラームの操作を開始します。 
  
この操作は Exchange Server 2013 で導入されました。
  
## <a name="using-the-performreminderaction-operation"></a>PerformReminderAction 操作を使用します。

**PerformReminderAction**操作を使用するには消去または[GetReminders](getreminders-operation.md)操作によって返される (遅延) アラームの再通知します。 アラームの再通知、**再通知**を、[ファイアウォール](actiontype-reminderactiontype.md)に設定し、 [NewReminderTime](newremindertime.md)の値を設定、現在の[ReminderTime](remindertime.md)よりも後ろにそれ以外の場合**NewReminderTime**は、サーバーによって無視されます。 アラームでは、定期的な会議と一致すると、**再通知**に対して操作を行う次の回のアラームが**NewReminderTime**で、アラーム、アラームが消される効果的に。 
  
アラームを消すには、**アラームを消す**に**ファイアウォール**を設定します。 サーバーは、要求を処理するときサーバーは、 **false を指定**する**True**から項目の[IsReminderSet](isreminderset.md)の値を変更します。
  
### <a name="performreminderaction-operation-soap-headers"></a>PerformReminderAction 操作の SOAP ヘッダー

**PerformReminderAction**操作は、次の表に記載されている SOAP ヘッダーを使用できます。 
  
|**ヘッダー名**|**要素**|**説明**|
|:-----|:-----|:-----|
|**偽装** <br/> |[ExchangeImpersonation](exchangeimpersonation.md) <br/> |クライアント アプリケーションが偽装するユーザーを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**MailboxCulture** <br/> |[MailboxCulture](mailboxculture.md) <br/> |RFC 3066、」タグの「識別の言語」を使用してメールボックスへのアクセスに定義されているカルチャを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**RequestVersion** <br/> |[RequestServerVersion](requestserverversion.md) <br/> |操作要求のスキーマのバージョンを識別します。 このヘッダーは、要求に適用されます。  <br/> |
|**ServerVersion** <br/> |[ServerVersionInfo](serverversioninfo.md) <br/> |要求に応答するサーバーのバージョンを識別します。 このヘッダーは、応答に適用されます。  <br/> |
   
## <a name="performreminderaction-operation-request-example"></a>PerformReminderAction 操作の要求の例

**PerformReminderAction**操作要求の次の例では、現在のアラームの再通知し、新しいアラーム時刻を設定する方法を示します。 [アイテム Id](itemid.md)の**変更キー**を含めるようにする必要があり、 **NewReminderTime**は、 [GetReminders](getreminders-operation.md)操作によって返される**ReminderTime**より後の時刻に設定する必要があることに注意してください。 
  
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
> **ItemId**の値が小さすぎると読みやすさを保持します。 
  
要求 SOAP 本体にはには、次の要素が含まれています。
  
- [PerformReminderAction](performreminderaction.md)
    
- [ReminderItemActions](reminderitemactions.md)
    
- [ReminderItemAction](reminderitemaction.md)
    
- [ファイアウォール](actiontype-reminderactiontype.md)
    
- [ItemId](itemid.md)
    
- [NewReminderTime](newremindertime.md)
    
## <a name="successful-performreminderaction-operation-response"></a>PerformReminderAction 操作の成功の応答

成功した要求への応答、 **PerformReminderAction**操作の例を次に示します。 **UpdatedItemIds**要素には、更新された予定表アイテムの**Itemid**が含まれています。 
  
```XML
<?xml version="1.0" encoding="utf-8"?>
<s:Envelope xmlns:s="http://schemas.xmlsoap.org/soap/envelope/">
  <s:Header>
    <ServerVersionInfo MajorVersion="15"
                       MinorVersion="0"
                       MajorBuildNumber="921"
                       MinorBuildNumber="20"
                       Version="V2_10"
                       xmlns:h="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns="http://schemas.microsoft.com/exchange/services/2006/types"
                       xmlns:xsd="http://www.w3.org/2001/XMLSchema"
                       xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance" />
  </s:Header>
  <s:Body xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
          xmlns:xsd="http://www.w3.org/2001/XMLSchema">
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
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
    
## <a name="performreminderaction-operation-error-response-example"></a>PerformReminderAction 操作のエラー応答の例

次の例は、サーバー上で変更が行われたいないときに、 **PerformReminderAction**操作の要求への応答を示します。 これは、応答の要求は送信されましたが、 **UpdatedItemIds**はありませんでした、アラームが変更されていないことを意味します。 
  
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
    <PerformReminderActionResponse ResponseClass="Success"
                                   xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ResponseCode>NoError</ResponseCode>
      <UpdatedItemIds />
    </PerformReminderActionResponse>
  </s:Body>
</s:Envelope>
```

エラー応答 SOAP 本体にはには、次の要素が含まれています。
  
- [PerformReminderActionResponse](performreminderactionresponse.md)
    
- [ResponseCode](responsecode.md)
    
- [UpdatedItemIds](updateditemids.md)
    
EWS を汎用のエラー コードは、 [ResponseCode](responsecode.md)を参照してください。
  
## <a name="see-also"></a>関連項目


- [GetReminders 操作](getreminders-operation.md)
    

