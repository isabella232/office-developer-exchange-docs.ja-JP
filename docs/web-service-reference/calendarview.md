---
title: CalendarView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- CalendarView
api_type:
- schema
ms.assetid: a4a953b8-0710-416c-95ef-59e51eba9982
description: 予定表ビューの要素は、カレンダーに表示される、一連の予定表のアイテムを返すよう FindItem 操作を定義します。
ms.openlocfilehash: 79b5ad268a8013092c1122c99bdcd10d876abf2c
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19759601"
---
# <a name="calendarview"></a>CalendarView

**予定表ビュー**の要素は、カレンダーに表示される、一連の予定表のアイテムを返すよう、 [FindItem 操作](finditem-operation.md)を定義します。 
  
[FindItem](finditem.md)
  
[予定表ビュー](calendarview.md)
  
```XML
<CalendarView MaxEntriesReturned="" StartDate="" EndDate="" />
```

**予定表ビュー**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |FindItem 応答で返す結果の最大数をについて説明します。  <br/> |
|**開始日** <br/> |予定表アイテムに対してクエリを実行する期間の開始を識別します。 終了時刻は**開始日**は返されません。 前にあるすべての予定表アイテム。 2006 のように、世界協定時刻 (UTC) 形式で**開始日**の値を指定することができます-01-02T12:00:00Z、2006年のように、ローカル時刻とタイム ゾーンのオフセットが指定されている形式で、または -01-02T04:00:00-08時 00分です。  <br/><br/>この属性は、必要があります。  <br/> |
|**終了日** <br/> |予定表アイテムに対してクエリを実行時間の範囲の末尾を識別します。 開始時刻または**終了日**の後にあるすべての予定表アイテムは返されません。 2006 のように、UTC 形式で**終了日**の値を指定することができます-02-02T12:00:00Z、2006年のように、ローカル時刻とタイム ゾーンのオフセットが指定されている形式で、または -02-02T04:00:00-08時 00分です。  <br/><br/>**終了日**が**開始日**は以上にする必要があります。それ以外の場合、エラーが返されます。 この属性は、必要があります。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索するための要求を定義します。<br/><br/> この要素への XPath 式は、次のようにします。  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>備考

FindItem 要求で、**予定表ビュー**の要素を指定すると、Web サービスは、1 つの予定表アイテムと出現する**開始日**と**終了日**に指定した範囲内での定期的な予定表アイテムの一覧を返します。
  
FindItem 要求で、**予定表ビュー**の要素を指定しない場合、Web サービスは、1 つの予定表アイテムと定期的なマスターの予定表アイテムの一覧を返します。 定期的な予定表アイテムの予定表アイテムは展開されません。 
  
予定表ビューのクエリを作成する必要がありますのみ予定表クエリを高速化をサポートするために次のプロパティを使用します。
  
### <a name="recurrence-blob-properties"></a>定期的なアイテムの blob のプロパティ
  
- MapiStartTime
    
- MapiEndTime
    
- SubjectPrefixInternal
    
- NormalizedSubjectInternal
    
- MapiSubject
    
- 場所
    
- AppointmentColor
    
- MapiIsAllDayEvent
    
- MapiHasAttachment
    
- FreeBusyStatus
    
- ReminderIsSetInternal
    
- ReminderMinutesBeforeStartInternal
    
- AppointmentState
    
- AllAttachmentsHidden
    
- ChangeHighlight
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a>主なパターン blob またはマスターからの計算
  
- ItemId
    
- IsRecurring
    
- IsException
    
- AppointmentRecurring
    
- MapiStartTime
    
- MapiPRStartDate
    
- MapiEndTime
    
- MapiPREndDate
    
- CalendarItemType
    
- GlobalObjectId
    
- TimeZoneDefinitionStart
    
- TimeZoneDefinitionEnd
    
### <a name="master-calendar-item-properties"></a>マスターの予定表アイテムのプロパティ
  
- EntryId
    
- ChangeKey
    
- ItemClass
    
- SentRepresentingEmailAddress
    
- SentRepresentingDisplayName
    
- SentRepresentingEntryId
    
- AppointmentRecurrenceBlob
    
- TimeZone
    
- TimeZoneBlob
    
- TimeZoneDefinitionRecurring
    
- CleanGlobalObjectId
    
- AppointmentRecurring
    
- IsException
    
- IsRecurring
    
- MapiSensitivity
    
- ContainerClass
    
- MapiPRStartDate
    
- MapiPREndDate
    
- カテゴリ
    
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

FindItem 要求の例を次に示します。 要求が成功するには、2006年で開始される予定表アイテムを含む応答が返されます-05-18T00:00:00-08時 00分後、2006 年以前に終了したのか -05-19T00:00:00-08時 00分です。
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="http://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="http://schemas.microsoft.com/exchange/services/2006/messages">
      <ItemShape>
        <t:BaseShape>IdOnly</t:BaseShape>
        <t:AdditionalProperties>
          <t:FieldURI FieldURI="calendar:Start"/>
          <t:FieldURI FieldURI="calendar:End"/>
          <t:FieldURI FieldURI="item:Subject"/>
        </t:AdditionalProperties>
      </ItemShape>
      <CalendarView MaxEntriesReturned="2" StartDate="2006-05-18T00:00:00-08:00" EndDate="2006-05-19T00:00:00-08:00"/>
      <ParentFolderIds>
        <t:DistinguishedFolderId Id="calendar"/>
      </ParentFolderIds>
    </FindItem>
  </soap:Body>
</soap:Envelope>
```

## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- 
  [FindItem 操作](finditem-operation.md)
- [項目を検索します。](http://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

