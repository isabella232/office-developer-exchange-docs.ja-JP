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
description: CalendarEventDetails 要素は、予定表のイベントに関する追加情報を提供します。
ms.openlocfilehash: 8df4f3ed4f66c7dcba00e1f0c5b0c383075da0a0
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759581"
---
# <a name="calendareventdetails"></a>CalendarEventDetails

**CalendarEventDetails**要素は、予定表のイベントに関する追加情報を提供します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[ID](id.md) <br/> |予定表アイテムのエントリ ID を表します。  <br/> |
|[件名 (CalendarEventDetails)](subject-calendareventdetails.md) <br/> |予定表アイテムの件名を表します。  <br/> |
|[場所 (CalendarEventDetails)](location-calendareventdetails.md) <br/> |予定表アイテムの [場所] フィールドを表します。  <br/> |
|[IsMeeting (CalendarEventDetails)](ismeeting-calendareventdetails.md) <br/> |予定表のイベントは、会議または予定かどうかを示します。  <br/> |
|[IsRecurring (CalendarEventDetails)](isrecurring-calendareventdetails.md) <br/> |予定表のイベントが定期的な予定表アイテムまたは単一の予定表アイテムのインスタンスであるかどうかを示します。  <br/> |
|[IsException](isexception.md) <br/> |マスターから定期的な予定表アイテムのインスタンスが変更されたかどうかを示します。  <br/> |
|[IsReminderSet](isreminderset.md) <br/> |カレンダー イベントのアラームが設定されているかどうかを示します。  <br/> |
|[IsPrivate](isprivate.md) <br/> |予定表アイテムがプライベートかどうかを示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CalendarEvent](calendarevent.md) <br/> |独自の予定表アイテムの出現を表します。  <br/> この要素への XPath 2.0 の式は、次のようにします。  <br/>  `/GetUserAvailabilityResponse/FreeBusyResponseArray/FreeBusyResponse/FreeBusyView/CalendarEventArray/CalendarEvent[i]` <br/> |
   
## <a name="remarks"></a>備考

発生したシーケンスは、すべての子要素の一覧です。 
  
[IsPrivate](isprivate.md)要素が**true**の場合は、 [CalendarEventDetails](calendareventdetails.md)要素内の他のすべての要素は、応答で返されません。 
  
GetUserAvailability 操作では、呼び出し元は、ターゲット ユーザーの予定表の読み取りアクセス権を持っていない限り、呼び出し元の詳細な情報は返されません。 Exchange 管理シェルを使用してアクセス許可を設定することができます。
  
MicrosoftExchange Server 2007 がインストールされているクライアント アクセス サーバーの役割を実行しているコンピューターの EWS 仮想ディレクトリには、この要素を記述するスキーマがあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[GetUserAvailability 操作](getuseravailability-operation.md)
  
[GetUserAvailabilityResponse](getuseravailabilityresponse.md)


[ユーザーの状態を取得します。](http://msdn.microsoft.com/library/d4133fcb-9b0f-4e6b-aadf-a389da83516a%28Office.15%29.aspx)

