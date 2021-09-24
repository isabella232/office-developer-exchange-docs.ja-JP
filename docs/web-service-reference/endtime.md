---
title: EndTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- EndTime
api_type:
- schema
ms.assetid: 82e4ef4f-a557-4044-b9b7-d91622f4ac55
description: EndTime 要素は、期間の終了を表します。
ms.openlocfilehash: 9b7dde6c318bb198e1ec25df19cf3a053feff5cf
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59540056"
---
# <a name="endtime"></a>EndTime

**EndTime 要素** は、期間の終了を表します。 
  
```xml
<EndTime>dateTime</EndTime>
```

 **dateTime**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[TimeWindow](timewindow.md) <br/> |ユーザーの可用性情報に対してクエリを実行した期間を識別します。<br/><br/> 次に、この要素の XPath 式を示します。<br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |推奨される会議時間に関する詳細情報を照会する期間を識別します。<br/><br/> 次に、この要素の XPath 式を示します。<br/><br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.  <br/> |
|[Duration (UserOofSettings)](duration-useroofsettings.md) <br/> | [OofState](oofstate.md)要素が Scheduled に設定されている場合Office (OOF) 状態が有効になっている期間を **指定します**。  <br/><br/>  この要素で使用できる XPath 式を次に示します。<br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[Occurrence](occurrence.md) <br/> |定期的な予定表アイテムが 1 回変更された場合を表します。  <br/> |
|[CalendarEvent](calendarevent.md) <br/> |一意の予定表アイテムの出現を表します。 これは、可用性に関する問い合わせに使用されます。 **EndTime 要素** は **CalendarEvent 要素で必要** です。 CalendarEvent **要素の** **EndTime 要素は、CalendarEvent** 型に **固有** です。<br/><br/> 次に、この要素の XPath 式を示します。<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。
  
## <a name="remarks"></a>注釈

[StartTime 要素](starttime.md)は、期間の開始を表します。 
  
終了時刻は、クライアントの時刻を表します。
  
スキーマには多数の [EndTime 要素が含](endtime.md) まれています。 
  
> [!NOTE]
> この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserAvailability 操作](getuseravailability-operation.md)
- [ユーザーの可用性の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

