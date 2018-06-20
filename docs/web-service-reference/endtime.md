---
title: EndTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EndTime
api_type:
- schema
ms.assetid: 82e4ef4f-a557-4044-b9b7-d91622f4ac55
description: 終了時刻の要素は、時間間隔の終了を表します。
ms.openlocfilehash: 7d3d186618a7bcc05ad82532e13e03d2e67a0e40
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/11/2018
ms.locfileid: "19760312"
---
# <a name="endtime"></a>EndTime

**終了時刻**の要素は、時間間隔の終了を表します。 
  
```xml
<EndTime>dateTime</EndTime>
```

 **dateTime**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[時間](timewindow.md) <br/> |ユーザーの可用性について照会する期間を指定します。<br/><br/> この要素への XPath 式は、次のようにします。<br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |提案された会議の時間についての詳細情報を照会する期間を指定します。<br/><br/> この要素への XPath 式は、次のようにします。<br/><br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow`.  <br/> |
|[期間 (UserOofSettings)](duration-useroofsettings.md) <br/> | Office (OOF) の状態が有効である[OofState](oofstate.md)要素は、 **[スケジュール済]** に設定されている場合、期間を指定します。  <br/><br/>  この要素に使用可能な XPath 式は、次のように。<br/><br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[出現](occurrence.md) <br/> |定期的な予定表アイテムの 1 つの変更されたアイテムを表します。  <br/> |
|[CalendarEvent](calendarevent.md) <br/> |独自の予定表アイテムの出現を表します。 可用性の照会のために使用します。 **CalendarEvent**要素では、**終了時刻**の要素が必要です。 **CalendarEvent**要素の**終了時刻**の要素は、 **CalendarEvent**の種類に固有です。<br/><br/> この要素への XPath 式は、次のようにします。<br/><br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。
  
## <a name="remarks"></a>備考

[StartTime](starttime.md)要素は、時間間隔の開始を表します。 
  
終了時刻は、クライアントの時刻を表します。
  
スキーマには、[終了時刻](endtime.md)の多くの要素が含まれています。 
  
> [!NOTE]
> MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。 
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserAvailability 操作](getuseravailability-operation.md)
- [ユーザーの状態を取得します。](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

