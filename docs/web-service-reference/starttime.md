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
ms.openlocfilehash: 16bee698b65dc512a709e2af9ddfe8629347fee3
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44458566"
---
# <a name="starttime"></a>StartTime

**StartTime**要素は、時間間隔の開始を表します。 
  
```xml
<StartTime/
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
|[TimeWindow](timewindow.md) <br/> |ユーザーの空き時間情報を照会した期間を識別します。  <br/><br/> この要素の XPath 式を次に示します。  <br/><br/>  `/GetUserAvailabilityRequest/FreeBusyViewOptions/TimeWindow` <br/> |
|[DetailedSuggestionsWindow](detailedsuggestionswindow.md) <br/> |提案された会議時間に関する詳細情報について、クエリされる期間を指定します。  <br/><br/> この要素の XPath 式を次に示します。 <br/> <br/>  `/GetUserAvailabilityRequest/SuggestionViewOptions/DetailedSuggestionsWindow` <br/> |
|[Duration (UserOofSettings)](duration-useroofsettings.md) <br/> | [Oofstate](oofstate.md)要素が [**スケジュール済み**] に設定されている場合に、不在時 (OOF) の状態が有効になる期間を指定します。  <br/><br/>  この要素に使用できる XPath 式は次のとおりです。 <br/> <br/>  `/SetUserOofSettingsRequest/UserOofSettings/Duration` <br/><br/>  `/GetUserOofSettingsResponse/OofSettings/Duration` <br/> |
|[CalendarEvent](calendarevent.md) <br/> |一意の予定表アイテムの出現を表します。 これは、可用性の照会に使用されます。 **CalendarEvent**要素では、 **StartTime**要素を指定する必要があります。 **CalendarEvent**要素の**starttime**要素は、 **CalendarEvent**型に対して一意ですが、 **Duration**型の**starttime**要素に含まれているのと同じファセット値が含まれています。  <br/><br/> この要素の XPath 式を次に示します。  <br/> <br/> `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値は必須です。
  
## <a name="remarks"></a>注釈

[EndTime](endtime.md)要素は、期間の最後の部分を表します。 
  
スキーマには、いくつかの[StartTime](starttime.md)要素が含まれています。 
  
> [!NOTE]
> この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。 
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [GetUserAvailability 操作](getuseravailability-operation.md)
- [ユーザーの空き時間情報の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

