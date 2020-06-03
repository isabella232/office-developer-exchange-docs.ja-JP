---
title: タスク
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Task
api_type:
- schema
ms.assetid: 7c84927e-db28-4c5d-b0b5-cbcc2b88d869
description: Task 要素は、Exchange ストア内のタスクを表します。
ms.openlocfilehash: 669f90dfa74cd085091e9836a1d31ca53bbf165e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44458944"
---
# <a name="task"></a>タスク

**Task**要素は、Exchange ストア内のタスクを表します。 
  
```xml
<Task>
   <MimeContent/>
   <ItemId/>
   <ParentFolderId/>
   <ItemClass/>
   <Subject/>
   <Sensitivity/>
   <Body/>
   <Attachments/>
   <DateTimeReceived/>
   <Size/>
   <Categories/>
   <InReplyTo/>
   <IsSubmitted/>
   <IsDraft/>
   <IsFromMe/>
   <IsResend/>
   <IsUnmodified/>
   <InternetMessageHeaders/>
   <DateTimeSent/>
   <DateTimeCreated/>
   <ResponseObjects/>
   <ReminderDueBy/>
   <ReminderIsSet/>
   <ReminderMinutesBeforeStart/>
   <DisplayCc/>
   <DisplayTo/>
   <HasAttachments/>
   <ExtendedProperty/>
   <Culture/>
   <ActualWork/>
   <AssignedTime/>
   <BillingInformation/>
   <ChangeCount/>
   <Companies/>
   <CompleteDate/>
   <Contacts/>
   <DelegationState/>
   <Delegator/>
   <DueDate/>
   <IsAssignmentEditable/>
   <IsComplete/>
   <IsRecurring/>
   <IsTeamTask/>
   <Mileage/>
   <Owner/>
   <PercentComplete/>
   <Recurrence/>
   <StartDate/>
   <Status/>
   <StatusDescription/>
   <TotalWork/>
   <EffectiveRights/>
   <LastModifiedName/>
   <LastModifiedTime/>
   <IsAssociated/>
   <WebClientReadFormQueryString/>
   <WebClientEditFormQueryString/>
   <ConversationId/>
   <UniqueBody/>
</Task>
```

**TaskType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Base64Binary 形式で表されるオブジェクトのネイティブな汎用インターネットメール内線 (MIME) ストリームが保存されています。  <br/> |
|[ItemId](itemid.md) <br/> |Exchange ストア内のアイテムの一意識別子および変更キーが含まれています。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |アイテムまたはフォルダーを含む親フォルダーの識別子を表します。  <br/> |
|[ItemClass](itemclass.md) <br/> |アイテムのメッセージクラスを表します。  <br/> |
|[件名](subject.md) <br/> |Exchange ストアアイテムおよび応答オブジェクトの件名を表します。  <br/> |
|[Sensitivity](sensitivity.md) <br/> |アイテムの秘密度の状態を格納します。  <br/> |
|[Body](body.md) <br/> |メッセージの実際の本文の内容を表します。  <br/> |
|[Attachments](attachments-ex15websvcsotherref.md) <br/> |Exchange ストア内のアイテムに添付されているアイテムまたはファイルが保存されています。  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |メールボックス内のアイテムが受信された日付と時刻を表します。  <br/> |
|[Size](size.md) <br/> |アイテムのサイズ (バイト単位) を表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。  <br/> |
|[Importance](importance.md) <br/> |アイテムの重要度について説明します。  <br/> |
|[InReplyTo](inreplyto.md) <br/> |このアイテムが返信であるアイテムの識別子を表します。  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |アイテムが送信トレイの既定フォルダーに送信されたかどうかを示します。  <br/> |
|[IsDraft](isdraft.md) <br/> |アイテムがまだ送信されていないかどうかを表します。  <br/> |
|[IsFromMe](isfromme.md) <br/> |ユーザーが自分にアイテムを送信したかどうかを示します。  <br/> |
|[IsResend](isresend.md) <br/> |アイテムが以前に送信されたかどうかを示します。  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |アイテムが変更されたかどうかを示します。  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |メールボックス内のアイテムに含まれるすべてのインターネットメッセージヘッダーのコレクションを表します。  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |メールボックス内のアイテムが送信された日付と時刻を表します。  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |メールボックス内の特定のアイテムが作成された日付と時刻を表します。  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Exchange ストア内のアイテムに関連付けられているすべての response オブジェクトのコレクションを格納します。  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |イベントが発生した日付と時刻を表します。 これは、アラームがいつ表示されるかを決定するために[ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によって使用されます。  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Exchange ストア内のアイテムにアラームが設定されているかどうかを示します。  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |アラームが表示されるイベントの前の時間 (分単位) を表します。  <br/> |
|[DisplayCc](displaycc.md) <br/> |[Cc] ボックスの内容に使用される表示文字列を表します。 これは、すべての Cc 受信者表示名の連結された文字列です。  <br/> |
|[DisplayTo](displayto.md) <br/> |[宛先] ボックスの内容に対して使用される表示文字列を表します。 これは、すべての受信者の表示名の連結文字列です。  <br/> |
|[HasAttachments](hasattachments.md) <br/> |アイテムに少なくとも1つの添付ファイルがある場合に**true**に設定されるプロパティを表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーとアイテムの拡張プロパティを識別します。  <br/> |
|[Culture](culture.md) <br/> |メールボックス内の特定のアイテムのカルチャを表します。  <br/> |
|[ActualWork](actualwork.md) <br/> |タスクに費やした実績時間を表します。  <br/> |
|[AssignedTime](assignedtime.md) <br/> |仕事が連絡先に割り当てられている時間を表します。  <br/> |
|[BillingInformation](billinginformation.md) <br/> |タスクの請求情報を保持します。  <br/> |
|[ChangeCount](changecount.md) <br/> |タスクのバージョンを指定します。  <br/> |
|[Companies](companies.md) <br/> |連絡先またはタスクに関連付けられている会社のコレクションを表します。  <br/> |
|[CompleteDate](completedate.md) <br/> |タスクが完了する日付を表します。  <br/> |
|[連絡先](contacts-ex15websvcsotherref.md) <br/> |タスクに関連付けられている連絡先の一覧が含まれています。  <br/> |
|[DelegationState](delegationstate.md) <br/> |委任されたタスクの状態を表します。  <br/> |
|[Delegator](delegator.md) <br/> |タスクを割り当てた委任者の名前が含まれます。  <br/> |
|[DueDate](duedate.md) <br/> |タスクアイテムの期限の日付を表します。  <br/> |
|[Is割り当て編集可能](isassignmenteditable.md) <br/> |タスクが編集可能であるかどうかを示します。  <br/> |
|[IsComplete](iscomplete.md) <br/> |タスクが完了したかどうかを示します。  <br/> |
|[IsRecurring](isrecurring.md) <br/> |タスクが定期的なアイテムの一部であるかどうかを示します。 この要素は値の取得のみ可能です。  <br/> |
|[IsTeamTask](isteamtask.md) <br/> |タスクがチームによって所有されているかどうかを示します。  <br/> |
|[Mileage](mileage.md) <br/> |タスクアイテムのマイレージを表します。  <br/> |
|[Owner](owner.md) <br/> |タスクの所有者を表します。  <br/> |
|[PercentComplete](percentcomplete.md) <br/> |タスクの完了状態を表します。  <br/> |
|[定期的なアイテム (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |定期的なタスクの定期的なアイテムの情報が含まれています。  <br/> |
|[StartDate](startdate.md) <br/> |タスクアイテムの開始日を表します。  <br/> |
|[状態](status.md) <br/> |タスクアイテムの状態を表します。  <br/> |
|[StatusDescription](statusdescription.md) <br/> |タスクの進捗状況の説明を格納します。  <br/> |
|[TotalWork](totalwork.md) <br/> |アイテムに関連付けられている作業量の説明を格納します。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。 この要素は値の取得のみ可能です。  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |アイテムを最後に変更したユーザーの表示名を含みます。  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |アイテムが最後に変更された日時を示します。  <br/> |
|[IsAssociated](isassociated.md) <br/> |アイテムがフォルダーに関連付けられているかどうかを示します。  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Outlook Web app のアイテムを読み取るために Microsoft Office Outlook Web App エンドポイントに連結する URL を表します。  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Outlook web app エンドポイントに連結して Outlook Web App のアイテムを編集するための URL を表します。  <br/> |
|[ConversationId](conversationid.md) <br/> |アイテムまたは会話の識別子が含まれています。  <br/> |
|[UniqueBody](uniquebody.md) <br/> |この会話の一意の本文を表す HTML フラグメントまたはプレーンテキストを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |会議の時刻に隣接しているすべての予定表アイテムを説明します。  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |[Updateitem 操作](updateitem-operation.md)中に、アイテム/フォルダーの1つのプロパティに追加するデータを識別します。  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |会議の時間と競合するすべてのアイテムを識別します。  <br/> |
|[Create (ItemSync)](create-itemsync.md) <br/> |ローカルクライアントストアに作成する単一のアイテムを識別します。  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |別の Exchange アイテムに関連付けられている Exchange アイテムを表します。  <br/> |
|[Items](items.md) <br/> |項目の配列を格納します。  <br/> |
|[SetItemField](setitemfield.md) <br/> |[Updateitem 操作](updateitem-operation.md)のアイテムの1つのプロパティに対する更新を表します。  <br/> |
|[Update (ItemSync)](update-itemsync.md) <br/> |ローカルクライアントストアで更新する単一のアイテムを識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
- [タスクの作成](https://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
- [タスクの削除](https://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

