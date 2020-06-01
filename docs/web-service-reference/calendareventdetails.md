---
title: CalendarEventDetails
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarEventDetails
api_type:
- schema
ms.assetid: 2dca0192-b91b-4154-aa09-84da74e875e9
description: CalendarEventDetails 要素は、カレンダーイベントに関する追加情報を提供します。
ms.openlocfilehash: 3e1dbba00bce4a1fdc53f3330527764c516890ab
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44459070"
---
# <a name="calendareventdetails"></a>CalendarEventDetails

**CalendarEventDetails**要素は、カレンダーイベントに関する追加情報を提供します。 
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)
  
[FreeBusyResponseArray](freebusyresponsearray.md)
  
[FreeBusyResponse](freebusyresponse.md)
  
[FreeBusyView](freebusyview.md)
  
[CalendarEventArray](calendareventarray.md)
  
[CalendarEvent](calendarevent.md)
  
[CalendarEventDetails](calendareventdetails.md)
  
```xml
<CalendarEventDetails>
   <ID/>
   <Subject/>
   <Location/>
   <IsMeeting/>
   <IsRecurring/>
   <IsException/>
   <IsReminderSet/>
   <IsPrivate/>
</CalendarEventDetails>
```

 **CalendarEventDetails**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[ID](id.md) <br/> |予定表アイテムのエントリ ID を表します。  <br/> |
|[Subject (CalendarEventDetails)](subject-calendareventdetails.md) <br/> |予定表アイテムの件名を表します。  <br/> |
|[場所 (CalendarEventDetails)](location-calendareventdetails.md) <br/> |予定表アイテムの "場所" フィールドを表します。  <br/> |
|[IsMeeting (CalendarEventDetails)](ismeeting-calendareventdetails.md) <br/> |予定表イベントが会議と予定のどちらであるかを示します。  <br/> |
|[IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) <br/> |予定表イベントが定期的な予定表アイテムまたは1つの予定表アイテムのインスタンスであるかどうかを示します。  <br/> |
|[IsException](isexception.md) <br/> |定期的な予定表アイテムのインスタンスをマスターから変更するかどうかを示します。  <br/> |
|[IsReminderSet](isreminderset.md) <br/> |予定表イベントにアラームが設定されているかどうかを示します。  <br/> |
|[IsPrivate](isprivate.md) <br/> |予定表アイテムがプライベートかどうかを示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarEvent](calendarevent.md) <br/> |一意の予定表アイテムの出現を表します。  <br/> この要素の XPath 2.0 式を次に示します。  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="remarks"></a>注釈

すべての子要素が発生する順序で一覧表示されます。 
  
[IsPrivate](isprivate.md)要素が**true**の場合、 [CalendarEventDetails](calendareventdetails.md)要素の他のすべての要素は応答で返されません。 
  
GetUserAvailability 操作は、発信者が対象ユーザーの予定表に対する読み取りアクセス権を持っていない限り、詳細な発信者情報を返しません。 アクセス許可は、Exchange 管理シェルを使用して設定できます。
  
この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[ユーザーの空き時間情報の取得](https://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

