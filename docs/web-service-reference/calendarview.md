---
title: CalendarView
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- CalendarView
api_type:
- schema
ms.assetid: a4a953b8-0710-416c-95ef-59e51eba9982
description: CalendarView 要素は、FindItem 操作を、予定表に表示されるセット内の予定表アイテムを返すとして定義します。
ms.openlocfilehash: 5e0180bb5e8a6d9fcbe42380abbe32820117ae29
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59518828"
---
# <a name="calendarview"></a>CalendarView

**CalendarView 要素は**[、FindItem 操作](finditem-operation.md)を、予定表に表示されるセット内の予定表アイテムを返すとして定義します。 
  
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
|**MaxEntriesReturned** <br/> |FindItem 応答で返される結果の最大数を示します。  <br/> |
|**StartDate** <br/> |予定表アイテムに対してクエリを実行する期間の開始を識別します。 **StartDate** より前の終了時刻を持つすべての予定表アイテムは返されません。 **StartDate** の値は、2006-01-02T12:00:00Z のように協定世界時 (UTC) 形式で指定するか、2006-01-02T04:00:00:00:00:00 のように現地時間とタイム ゾーンのオフセットを指定する形式で指定できます。  <br/><br/>この属性は必須です。  <br/> |
|**EndDate** <br/> |予定表アイテムに対してクエリを実行した期間の終了を識別します。 **EndDate** 以降の開始時刻を持つすべての予定表アイテムは返されません。 **EndDate** の値は、2006-02-02T12:00:00Z のように UTC 形式で指定するか、2006-02-02T04:00:00:00-08:00 のように現地時間とタイム ゾーンのオフセットを指定する形式で指定できます。  <br/><br/>**EndDate** は StartDate 以上である **必要があります**。それ以外の場合は、エラーが返されます。 この属性は必須です。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[FindItem](finditem.md) <br/> |メールボックス内のアイテムを検索する要求を定義します。<br/><br/> 次に、この要素の XPath 式を示します。  <br/>  `/FindItem` <br/> |
   
## <a name="remarks"></a>注釈

**CalendarView** 要素が FindItem 要求で指定されている場合、Web サービスは **、StartDate** と **EndDate** で指定された範囲内の単一の予定表アイテムと定期的な予定表アイテムの一覧を返します。
  
**FindItem 要求で CalendarView** 要素が指定されていない場合、Web サービスは単一の予定表アイテムと定期的なマスター 予定表アイテムのリストを返します。 定期的な予定表アイテムの予定表の出現は展開されません。 
  
CalendarView クエリは、より高速な予定表クエリをサポートするために、次のプロパティのみを使用する必要があります。
  
### <a name="recurrence-blob-properties"></a>定期的な BLOB プロパティ
  
- MapiStartTime
    
- MapiEndTime
    
- SubjectPrefixInternal
    
- NormalizedSubjectInternal
    
- MapiSubject
    
- Location
    
- AppointmentColor
    
- MapiIsAllDayEvent
    
- MapiHasAttachment
    
- FreeBusyStatus
    
- ReminderIsSetInternal
    
- ReminderMinutesBeforeStartInternal
    
- AppointmentState
    
- AllAttachmentsHidden
    
- ChangeHighlight
    
### <a name="calculated-from-the-primary-recurrence-blob-or-master"></a>プライマリ定期的な BLOB またはマスターから計算される
  
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
    
### <a name="master-calendar-item-properties"></a>マスター 予定表アイテムのプロパティ
  
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
    
- Categories
    
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="example"></a>例

次の例は、FindItem 要求を示しています。 成功した要求は、2006-05-18T00:00:00-08:00 以降で開始され、2006-05-19T00:00:00:00-08:00 より前に終了した予定表アイテムを含む応答を返します。
  
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
|スキーマ名  <br/> |メッセージ スキーマ  <br/> |
|検証ファイル  <br/> |Messages.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [FindItem 操作](finditem-operation.md)
- [アイテムの検索](https://msdn.microsoft.com/library/63af1f9c-464b-4fca-9ae3-3d60f24ca93c%28Office.15%29.aspx)

