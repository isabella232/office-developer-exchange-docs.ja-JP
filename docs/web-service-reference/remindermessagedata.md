---
title: ReminderMessageData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
ms.assetid: 04dd4987-baaf-4ebe-ae58-ad962c2f8fa1
description: ReminderMessageData 要素は、アラームメッセージのデータを指定します。
ms.openlocfilehash: f2632062cd02581c426f7dbfa2a33d53e5594d72
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458552"
---
# <a name="remindermessagedata"></a>ReminderMessageData

**ReminderMessageData**要素は、アラームメッセージのデータを指定します。 
  
```XML
<ReminderMessageData>
   <ReminderText></ReminderText>
   <Location></Location>
   <StartTime></StartTime>
   <EndTime></EndTime>
   <AssociatedCalendarItemId></AssociatedCalendarItemId>
</ReminderMessageData>

```

 **ReminderMessageDataType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

[ReminderText](remindertext.md)  | [場所](location.md)  | [StartTime (ReminderMessageDataType)](starttime-remindermessagedatatype.md)  | [EndTime (ReminderMessageDataType)](endtime-remindermessagedatatype.md)  | [AssociatedCalendarItemId](associatedcalendaritemid.md)
  
### <a name="parent-elements"></a>親要素

[Message](message-ex15websvcsotherref.md)
  
## <a name="remarks"></a>注釈

この要素は Exchange Server 2013 Service Pack 1 (SP1) で導入されました。
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
ビルド番号15.00.0913.09 以降のバージョンの Exchange では、 **ReminderMessageData**要素の子要素として**AssociatedCalendarItemId**要素を含めることができます。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しい  <br/> |
   
## <a name="see-also"></a>関連項目



[Message](message-ex15websvcsotherref.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

