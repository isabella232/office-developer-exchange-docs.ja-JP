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
description: IsRecurring 要素では、予定表アイテム、会議出席依頼、またはタスクの定期的なアイテムの一部であるかどうかを示します。 この要素は、読み取り専用です。
ms.openlocfilehash: dfb0c28fe225792c7128409a8cf010627c624fe0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19832104"
---
# <a name="isrecurring"></a>IsRecurring

**IsRecurring**要素では、予定表アイテム、会議出席依頼、またはタスクの定期的なアイテムの一部であるかどうかを示します。 この要素は、読み取り専用です。 
  
```xml
<IsRecurring/>
```

 **ブール型 (Boolean)**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

ブール値を表す文字列値は、必要があります。
  
## <a name="remarks"></a>備考

次の表は、開催者と出席者と会議出席依頼と更新プログラムの別の予定表アイテムの種類に対して、 **IsRecurring**プロパティを設定する方法を示します。 
  
|**カレンダー項目の種類**|**オーガナイザー <br/> (IsRecurring)**|**出席者<br/>(IsRecurring)**|**会議の更新の要求/ <br/> (IsRecurring)**|
|:-----|:-----|:-----|:-----|
|1 回  <br/> |**FALSE** <br/> |**FALSE** <br/> |**FALSE** <br/> |
|定期的なマスター  <br/> |**FALSE** <br/> |**場合は TRUE。** <br/> |**場合は TRUE。** <br/> |
|定期的な例外  <br/> |**場合は TRUE。** <br/> |**場合は TRUE。** <br/> |**場合は TRUE。** <br/> |
   
開催者の定期的なマスターの予定表のアイテムに設定されている**IsRecurring**プロパティの値が正しくありません。この値を**TRUE**に設定する必要があります。 
  
> [!NOTE]
> GetUserAvailability 操作では、 [IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md)の要素もあります。 
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[TaskType.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurring.aspx)
  
[CalendarEventDetails.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarEventDetails.IsRecurring.aspx)
  
[CalendarItemType.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurring.aspx)
  
[MeetingRequestMessageType.IsRecurring](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurring.aspx)
  
[CalendarItemType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.CalendarItemType.IsRecurringSpecified.aspx)
  
[MeetingRequestMessageType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.MeetingRequestMessageType.IsRecurringSpecified.aspx)
  
[TaskType.IsRecurringSpecified](https://msdn.microsoft.com/library/ExchangeWebServices.TaskType.IsRecurringSpecified.aspx)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

