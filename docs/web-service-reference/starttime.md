---
title: StartTime
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- StartTime
api_type:
- schema
ms.assetid: 1fac7937-7a06-4d66-9d2a-14423bcb3b37
description: StartTime 要素は、時間間隔の開始を表します。
ms.openlocfilehash: 4346797d755bb6e577e1cacb8bec656a7562bf1f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19833560"
---
# <a name="starttime"></a>StartTime

**StartTime**要素は、時間間隔の開始を表します。 
  
```xml
<StartTime/
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
|[時間](timewindow.md) <br/> |ユーザーの可用性について照会する期間を指定します。  <br/><br/> この要素への XPath 式は、次のようにします。  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |提案された会議の時間についての詳細情報を照会する期間を指定します。  <br/><br/> この要素への XPath 式は、次のようにします。 <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[期間 (UserOofSettings)](duration-useroofsettings.md) <br/> | Office (OOF) の状態が有効である[OofState](oofstate.md)要素は、 **[スケジュール済]** に設定されている場合、期間を指定します。  <br/><br/>  この要素に使用可能な XPath 式は、次のように。 <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[CalendarEvent](calendarevent.md) <br/> |独自の予定表アイテムの出現を表します。 可用性の照会のために使用します。 **CalendarEvent**要素の**開始**要素が必要です。 **CalendarEvent**要素の**開始時刻**の要素は、**期間**の種類の**開始時刻**の要素が含まれているのと同じファセット値が含まれていますが**CalendarEvent**の種類に固有です。  <br/><br/> この要素への XPath 式は、次のようにします。  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。
  
## <a name="remarks"></a>備考

[終了時刻](endtime.md)の要素では、期間の終了を表します。 
  
スキーマには、[開始時刻](starttime.md)の多くの要素が含まれています。 
  
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

