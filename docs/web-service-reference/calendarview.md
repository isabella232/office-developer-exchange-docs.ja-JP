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
description: CalendarView 要素は、カレンダーに表示されているように、セット内の予定表アイテムを返す FindItem 操作を定義します。
ms.openlocfilehash: e547a4b2db5c09ebefd9a072da6cc4733818002e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44462263"
---
# <a name="calendarview"></a>CalendarView

**CalendarView**要素は、カレンダーに表示されているように、セット内の予定表アイテムを返す[FindItem 操作](finditem-operation.md)を定義します。 
  
[FindItem](finditem.md)
  
[CalendarView](calendarview.md)
  
```XML
<CalendarView MaxEntriesReturned="" StartDate="" EndDate="" />
```

**CalendarView**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|**MaxEntriesReturned** <br/> |FindItem 応答で返される結果の最大数を表します。  <br/> |
|**StartDate** <br/> |予定表アイテムを照会する期間の開始日を識別します。 終了時刻**が開始日より前**のすべての予定表アイテムは返されません。 **StartDate**の値は協定世界時 (UTC) 形式で指定できます。2006年-01-02T12:00: 00z、または現地時刻とタイムゾーンオフセットが指定されている形式 (2006-01-02T12:00:00-08:00) で指定できます。  <br/><br/>この属性は必須です。  <br/> |
|**EndDate** <br/> |予定表アイテムを照会した期間の終わりを識別します。 開始時刻が終了日になっている予定表**アイテムは、** すべて返されません。 **EndDate**の値は、2006年-02-02T12:00: 00z のように UTC 形式で指定することができます。また、2006-02-02T12:00:00-08:00 のように、現地時刻とタイムゾーンオフセットが指定されている形式で指定することもできます。  <br/><br/>**EndDate**は**StartDate**以上である必要があります。それ以外の場合は、エラーが返されます。 この属性は必須です。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索するための要求を定義します。<br/><br/> この要素の XPath 式を次に示します。  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>注釈

**CalendarView**要素が FindItem 要求で指定されている場合、Web サービスは、開始**日と終了**日で指定**された**範囲内の予定表アイテムの1つおよび定期的なアイテムのリストを返します。
  
**CalendarView**要素が FindItem 要求で指定されていない場合、Web サービスは、1つの予定表アイテムと定期的なマスター予定表アイテムの一覧を返します。 定期的な予定表アイテムの予定表アイテムは展開されません。 
  
CalendarView クエリでは、より高速な予定表クエリがサポートされているため、次のプロパティのみを使用してください。
  
### <a name="recurrence-blob-properties"></a>定期的な blob プロパティ
  
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
    
- ChangeHighlight 表示
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a>主要な定期的なアイテムの blob またはマスターから計算されます。
  
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
    
### <a name="master-calendar-item-properties"></a>マスター予定表アイテムのプロパティ
  
- EntryId
    
- ChangeKey
    
- ItemClass
    
- SentRepresentingEmailAddress
    
- [文] 表示 Displayname
    
- [文]
    
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

次の例は、FindItem 要求を示しています。 成功した要求は、2006年-05-18T00:00:00-08:00 または after and 終了された予定表アイテムを含む応答を返します。これは2006年から 05-19T00:00:00-08:00 です。
  
```xml
<?xml version="1.0" encoding="utf-8"?>
<soap:Envelope xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
               xmlns:xsd="http://www.w3.org/2001/XMLSchema"
               xmlns:soap="http://schemas.xmlsoap.org/soap/envelope/"
               xmlns:t="https://schemas.microsoft.com/exchange/services/2006/types">
  <soap:Body>
    <FindItem Traversal="Shallow" xmlns="https://schemas.microsoft.com/exchange/services/2006/messages">
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

## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/messages  <br/> |
|スキーマ名  <br/> |メッセージスキーマ  <br/> |
|検証ファイル  <br/> |メッセージ .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [FindItem 操作](finditem-operation.md)
- [アイテムの検索](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

