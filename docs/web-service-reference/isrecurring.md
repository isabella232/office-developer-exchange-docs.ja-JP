---
title: IsRecurring
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsRecurring
api_type:
- schema
ms.assetid: f4df6997-8d5b-4893-a4a5-fc7047e0a9c3
description: IsRecurring 要素は、予定表アイテム、会議出席依頼、またはタスクが定期的なアイテムの一部であるかどうかを示します。 この要素は値の取得のみ可能です。
ms.openlocfilehash: 72c71c1955b69f1c0df855ce4bd0ed02d4c89122
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44526488"
---
# <a name="isrecurring"></a>IsRecurring

**Isrecurring**要素は、予定表アイテム、会議出席依頼、またはタスクが定期的なアイテムの一部であるかどうかを示します。 この要素は値の取得のみ可能です。 
  
```xml
<IsRecurring/>
```

 **Boolean**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

ブール値を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

次の表は、開催者と出席者、および会議出席依頼と更新について、さまざまな予定表アイテムの種類に対して**Isrecurring**プロパティを設定する方法を示しています。 
  
|**CalendarItem 型**|**開催者 <br/> (isrecurring)**|**出席者 <br/> (isrecurring)**|**会議出席依頼/更新 <br/> (isrecurring)**|
|:-----|:-----|:-----|:-----|
|単一の発生  <br/> |**FALSE** <br/> |**FALSE** <br/> |**FALSE** <br/> |
|定期的なマスター  <br/> |**FALSE** <br/> |**FALSE** <br/> |**FALSE** <br/> |
|定期的な例外  <br/> |**FALSE** <br/> |**FALSE** <br/> |**FALSE** <br/> |
   
開催者の定期的なマスター予定表アイテムに対して設定されている**Isrecurring**なプロパティの値が正しくありません。この値は**TRUE**に設定する必要があります。 
  
> [!NOTE]
> GetUserAvailability 操作には、 [Isrecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md)要素もあります。 
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[TaskType IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurring.aspx)
  
[CalendarEventDetails](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarEventDetails.IsRecurring.aspx)
  
[CalendarItemType](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurring.aspx)
  
[会議の要求の Messagetype。 IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurring.aspx)
  
[CalendarItemType](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurringSpecified.aspx)
  
[会議の IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurringSpecified.aspx)
  
[IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurringSpecified.aspx)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

