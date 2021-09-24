---
title: ReminderMessageData
manager: sethgros
ms.date: 03/9/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
ms.assetid: 04dd4987-baaf-4ebe-ae58-ad962c2f8fa1
description: ReminderMessageData 要素は、アラーム メッセージ内のデータを指定します。
ms.openlocfilehash: d916e1526f11795efa54cdf186d606bc293656e0
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59512451"
---
# <a name="remindermessagedata"></a>ReminderMessageData

**ReminderMessageData 要素** は、アラーム メッセージ内のデータを指定します。 
  
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
  
ビルド番号 15.00.0913.09 から始まる Exchange のバージョンには **、ReminderMessageData** 要素の子要素として **AssociatedCalendarItemId** 要素を含めできます。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |正解  <br/> |
   
## <a name="see-also"></a>関連項目



[Message](message-ex15websvcsotherref.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

