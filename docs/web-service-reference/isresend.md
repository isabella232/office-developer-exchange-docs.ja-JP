---
title: IsResend
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- IsResend
api_type:
- schema
ms.assetid: 8f758b6b-dcee-4f95-9d39-e4be2bd92961
description: IsResend 要素は、アイテムが以前に送信されたかどうかを示します。
ms.openlocfilehash: ec0981ceb733389bf2755646c2a85b357a84d348
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2020
ms.locfileid: "44467852"
---
# <a name="isresend"></a>IsResend

**Isresend**要素は、アイテムが以前に送信されたかどうかを示します。 
  
```xml
<IsResend/>
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
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
|[連絡先](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[アイテム](item.md) <br/> |Exchange ストア内のアイテムを表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消しを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の応答を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メールメッセージを表します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |Exchange ストアからアイテムを削除します。  <br/> |
|[Task](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

テキスト値**true**は、アイテムが以前に送信されたことを示します。 
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

