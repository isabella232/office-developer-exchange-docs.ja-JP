---
title: 出席者
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Attendee
api_type:
- schema
ms.assetid: 393c3d7e-7416-458a-b976-270b88eaaa03
description: Attendee 要素は、会議の出席者とリソースを表します。
ms.openlocfilehash: d48dcee42292b045ffc7cdcc5fd02f70109b1853
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59531195"
---
# <a name="attendee"></a>出席者

**Attendee 要素は**、会議の出席者とリソースを表します。 
  
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
|[メールボックス](mailbox.md) <br/> |完全に解決された電子メール アドレスを識別します。  <br/> |
|[ResponseType](responsetype.md) <br/> |会議で受信する受信者の応答の種類を表します。 このプロパティは、会議開催者の予定表アイテムにのみ関連します。  <br/> |
|[LastResponseTime](lastresponsetime.md) <br/> |受信した最新の応答の日時を表します。  <br/> |
|[ProposedStart](proposedstart-attendeetype.md) <br/> |会議の出席者が提案した開始時刻を表します。 <br/> |
|[ProposedEnd](proposedend-attendeetype.md) <br/> |会議の出席者が提案した終了時刻を表します。 <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[RequiredAttendees](requiredattendees.md) <br/> |会議に出席するために必要な出席者を表します。  <br/> |
|[OptionalAttendees](optionalattendees.md) <br/> |会議に出席する必要がなされていない出席者を表します。  <br/> |
|[リソース](resources.md) <br/> |会議のスケジュールされたリソースを表します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

