---
title: IsRecurring
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- IsRecurring
api_type:
- schema
ms.assetid: f4df6997-8d5b-4893-a4a5-fc7047e0a9c3
description: IsRecurring 要素は、予定表アイテム、会議出席依頼、またはタスクが定期的なアイテムの一部であるかどうかを示します。 この要素は読み取り専用です。
ms.openlocfilehash: ea910b78e962906285a73c869e394147c324372c
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59532727"
---
# <a name="isrecurring"></a>IsRecurring

**IsRecurring 要素** は、予定表アイテム、会議出席依頼、またはタスクが定期的なアイテムの一部であるかどうかを示します。 この要素は読み取り専用です。 
  
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
|[CalendarItem](calendaritem.md) <br/> |予定表アイテムのExchangeを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |ユーザー ストア内の会議出席依頼Exchangeします。  <br/> |
|[タスク](task.md) <br/> |ストア内のタスクをExchangeします。  <br/> |
   
## <a name="text-value"></a>テキスト値

ブール値を表すテキスト値が必要です。
  
## <a name="remarks"></a>注釈

次の表は **、IsRecurring** プロパティが、開催者と出席者、および会議出席依頼と更新に対して異なる予定表アイテムの種類に対して設定される方法を示しています。 
  
|**CalendarItem の種類**|**オー  <br/> ガナイザー (IsRecurring)**|**Attendee  <br/> (IsRecurring)**|**会議出席依頼/更新  <br/> (IsRecurring)**|
|:-----|:-----|:-----|:-----|
|単一オカレンス  <br/> |**FALSE** <br/> |**FALSE** <br/> |**FALSE** <br/> |
|定期的なマスター  <br/> |**FALSE** <br/> |**TRUE** <br/> |**TRUE** <br/> |
|定期的な例外  <br/> |**TRUE** <br/> |**TRUE** <br/> |**TRUE** <br/> |
   
オー **ガナイザーの定期的な** マスター 予定表アイテムに設定されている IsRecurring プロパティの値が正しくありません。この 値 は TRUE に設定する **必要があります**。 
  
> [!NOTE]
> GetUserAvailability 操作にも [IsRecurring (CalendarEventDetails) 要素](isrecurring-calendareventdetails.md) があります。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[TaskType.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurring.aspx)
  
[CalendarEventDetails.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarEventDetails.IsRecurring.aspx)
  
[CalendarItemType.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurring.aspx)
  
[MeetingRequestMessageType.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurring.aspx)
  
[CalendarItemType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurringSpecified.aspx)
  
[MeetingRequestMessageType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurringSpecified.aspx)
  
[TaskType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurringSpecified.aspx)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

