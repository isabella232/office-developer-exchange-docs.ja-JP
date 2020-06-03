---
title: 件名
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Subject
api_type:
- schema
ms.assetid: c140d6c2-deb1-4f67-a908-9397197c4ae7
description: Subject 要素は、Exchange ストアアイテムの subject プロパティを表します。 件名は255文字に制限されます。
ms.openlocfilehash: c4d7c21ab70c21ceb63e53d008d25aebf8e22270
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458972"
---
# <a name="subject"></a>件名

**Subject**要素は、Exchange ストアアイテムの subject プロパティを表します。 件名は255文字に制限されます。 
  
```XML
<Subject/>
```

 **string**
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
|[CancelCalendarItem](cancelcalendaritem.md) <br/> |予定表アイテムの応答の取り消しオブジェクトを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[FindMessageTrackingReport](findmessagetrackingreport.md) <br/> |検索するメッセージの種類の条件を指定します。  <br/> |
|[Forwarditem と](forwarditem.md) <br/> |転送アイテムのスマート応答オブジェクトを表します。  <br/> |
|[Item](item.md) <br/> |Exchange ストア内のアイテムを表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消しを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議メッセージを表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の応答を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange ストア内の電子メールを表します。  <br/> |
|[および search-messagetrackingreport](messagetrackingreport.md) <br/> |[Getmessagetrackingreport 操作](getmessagetrackingreport-operation.md)で返される1つのメッセージを格納します。  <br/> |
|[MessageTrackingSearchResult](messagetrackingsearchresult.md) <br/> |[Findmessagetrackingreportresponse](findmessagetrackingreportresponse.md)要素の単一メッセージ結果を格納します。  <br/> |
|[RemoveItem](removeitem.md) <br/> |アイテムの削除応答オブジェクトを表します。  <br/> |
|[Replyalltoitem と](replyalltoitem.md) <br/> |応答のすべてのスマート応答オブジェクトを表します。  <br/> |
|[ReplyToItem](replytoitem.md) <br/> |返信先アイテムのスマート応答オブジェクトを表します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

Exchange アイテムの件名を含むテキスト値が必要です。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[GetMessageTrackingReport 操作](getmessagetrackingreport-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

