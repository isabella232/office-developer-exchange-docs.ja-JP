---
title: 参加者
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Attendee
api_type:
- schema
ms.assetid: 393c3d7e-7416-458a-b976-270b88eaaa03
description: 出席者要素は、会議の出席者とリソースを表します。
ms.openlocfilehash: f376e59b27017e0a9d27692cb1a4ae759cd1af0e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44457649"
---
# <a name="attendee"></a>参加者

出席**者**要素は、会議の出席者とリソースを表します。 
  
```xml
<Attendee>
   <Mailbox/>
   <ResponseType/>
   <LastResponseTime/>
</Attendee>
```

 **AttendeeType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[メールボックス](mailbox.md) <br/> |完全に解決された電子メールアドレスを識別します。  <br/> |
|[ResponseType](responsetype.md) <br/> |会議の受信者の応答の種類を表します。 このプロパティは、会議開催者の予定表アイテムにのみ関連しています。  <br/> |
|[LastResponseTime](lastresponsetime.md) <br/> |受信された最新の応答の日付と時刻を表します。  <br/> |
|[ProposedStart](proposedstart-attendeetype.md) <br/> |会議の出席者が提案した開始時刻を表します。 <br/> |
|[ProposedEnd](proposedend-attendeetype.md) <br/> |会議の出席者が提案した終了時刻を表します。 <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RequiredAttendees](requiredattendees.md) <br/> |会議に出席するために必要な出席者を表します。  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |会議に出席する必要がない出席者を表します。  <br/> |
|[リソース](resources.md) <br/> |会議のスケジュールされたリソースを表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

