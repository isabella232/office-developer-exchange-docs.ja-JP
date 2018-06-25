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
ms.openlocfilehash: 2c61fca6ac85290e34f1365b0cb9e841e1fe279f
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19839655"
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

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[MimeContent](mimecontent.md) <br/> |Base64Binary の形式で表されるオブジェクトのネイティブの多目的インターネット メール拡張 (MIME) ストリームが含まれています。  <br/> |
|[ItemId](itemid.md) <br/> |Exchange ストア内のアイテムの一意の識別子と変更キーが含まれています。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |アイテムまたはフォルダーを含む親フォルダーの識別子を表します。  <br/> |
|[ItemClass](itemclass.md) <br/> |アイテムのメッセージ クラスを表します。  <br/> |
|[Subject](subject.md) <br/> |Exchange ストアのアイテムおよび応答オブジェクトのサブジェクトを表します。  <br/> |
|[Sensitivity](sensitivity.md) <br/> |アイテムの秘密度の状態が含まれています。  <br/> |
|[Body/本文](body.md) <br/> |メッセージの実際の本文の内容を表します。  <br/> |
|[添付ファイル](attachments-ex15websvcsotherref.md) <br/> |アイテムや、Exchange ストア内のアイテムに関連付けられているファイルが含まれています。  <br/> |
|[DateTimeReceived](datetimereceived.md) <br/> |メールボックス内のアイテムを受信したときの日時を表します。  <br/> |
|[Size](size.md) <br/> |アイテムのバイト単位でサイズを表します。 このプロパティは値の取得のみ可能です。  <br/> |
|[Categories](categories-ex15websvcsotherref.md) <br/> |メールボックス内のアイテムが属するカテゴリを識別する文字列のコレクションを表します。  <br/> |
|[Importance](importance.md) <br/> |アイテムの重要性をについて説明します。  <br/> |
|[InReplyTo](inreplyto.md) <br/> |このアイテムの返信するアイテムの識別子を表します。  <br/> |
|[IsSubmitted](issubmitted.md) <br/> |アイテムが [送信トレイ] 既定フォルダーに送信されたかどうかを示します。  <br/> |
|[IsDraft](isdraft.md) <br/> |アイテムはまだ送信されていないかどうかを表します。  <br/> |
|[IsFromMe](isfromme.md) <br/> |ユーザーが彼または彼女自身にアイテムを送信するかどうかを示します。  <br/> |
|[IsResend](isresend.md) <br/> |アイテムが以前送信されたかどうかを示します。  <br/> |
|[IsUnmodified](isunmodified.md) <br/> |アイテムが変更されたかどうかを示します。  <br/> |
|[InternetMessageHeaders](internetmessageheaders.md) <br/> |メールボックス内のアイテムに含まれるすべてのインターネット メッセージ ヘッダーのコレクションを表します。  <br/> |
|[DateTimeSent](datetimesent.md) <br/> |メールボックス内のアイテムが送信された日時を表します。  <br/> |
|[DateTimeCreated](datetimecreated.md) <br/> |メールボックス内の特定のアイテムが作成された日時を表します。  <br/> |
|[ResponseObjects](responseobjects.md) <br/> |Exchange ストア内のアイテムに関連付けられているすべての応答オブジェクトのコレクションが含まれています。  <br/> |
|[ReminderDueBy](reminderdueby.md) <br/> |イベントが発生したときの日時を表します。 [ReminderMinutesBeforeStart](reminderminutesbeforestart.md)要素によってアラームが表示されたときを決定する使用されます。  <br/> |
|[ReminderIsSet](reminderisset.md) <br/> |Exchange ストアのアイテムのアラームが設定されたかどうかを示します。  <br/> |
|[ReminderMinutesBeforeStart](reminderminutesbeforestart.md) <br/> |分前にアラームが表示されるときに、イベントの数を表します。  <br/> |
|[DisplayCc](displaycc.md) <br/> |[Cc] ボックスの内容のために使用される表示文字列を表します。 これは、すべての Cc 受信者の表示名の連結された文字列です。  <br/> |
|[DisplayTo](displayto.md) <br/> |ボックスの内容のために使用される表示文字列を表します。 これは、すべての受信者の表示名の連結された文字列です。  <br/> |
|[添付ファイル付き](hasattachments.md) <br/> |アイテムに表示されている 1 つ以上の添付ファイルがある場合に**true**に設定されているプロパティを表します。 このプロパティは値の取得のみ可能です。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーおよびアイテムの拡張プロパティを識別します。  <br/> |
|[カルチャ](culture.md) <br/> |メールボックス内の指定したアイテムのカルチャを表します。  <br/> |
|[ActualWork](actualwork.md) <br/> |タスクに費やされた時間の実際の量を表します。  <br/> |
|[AssignedTime](assignedtime.md) <br/> |連絡先にタスクを割り当てると時間を表します。  <br/> |
|[BillingInformation](billinginformation.md) <br/> |課金タスクの情報を保持します。  <br/> |
|[ChangeCount](changecount.md) <br/> |タスクのバージョンを指定します。  <br/> |
|[Companies](companies.md) <br/> |連絡先またはタスクに関連付けられている企業のコレクションを表します。  <br/> |
|[CompleteDate](completedate.md) <br/> |タスクが完了する日付を表します。  <br/> |
|[連絡先](contacts-ex15websvcsotherref.md) <br/> |タスクに関連付けられている連絡先の一覧が含まれています。  <br/> |
|[DelegationState](delegationstate.md) <br/> |委任されたタスクの状態を表します。  <br/> |
|[Delegator](delegator.md) <br/> |タスクを割り当てられている代理人の名前が含まれています。  <br/> |
|[DueDate](duedate.md) <br/> |タスク アイテムの期限の日付を表します。  <br/> |
|[IsAssignmentEditable](isassignmenteditable.md) <br/> |タスクが編集可能かどうかを示します。  <br/> |
|[完了](iscomplete.md) <br/> |タスクが完了したかどうかどうかを示します。  <br/> |
|[IsRecurring](isrecurring.md) <br/> |タスクが定期的なアイテムの一部であるかどうかを示します。 この要素は、読み取り専用です。  <br/> |
|[IsTeamTask](isteamtask.md) <br/> |か、タスクが、チームが所有するかどうかを示します。  <br/> |
|[マイレージ](mileage.md) <br/> |タスク アイテムの経費情報を表します。  <br/> |
|[所有者](owner.md) <br/> |タスクの所有者を表します。  <br/> |
|[達成率](percentcomplete.md) <br/> |タスクの完了状態を説明します。  <br/> |
|[定期的な予定 (TaskRecurrenceType)](recurrence-taskrecurrencetype.md) <br/> |定期タスクの頻度に関する情報が含まれています。  <br/> |
|[開始日](startdate.md) <br/> |作業項目の開始日を表します。  <br/> |
|[Status](status.md) <br/> |作業項目の状態を表します。  <br/> |
|[StatusDescription](statusdescription.md) <br/> |タスクの進捗状況の説明が含まれています。  <br/> |
|[TotalWork](totalwork.md) <br/> |アイテムに関連付けられている作業量の説明が含まれています。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可の設定に基づいてクライアントの権限が含まれています。 この要素は、読み取り専用です。  <br/> |
|[LastModifiedName](lastmodifiedname.md) <br/> |最後の項目を変更するのにはユーザーの表示名が含まれています。  <br/> |
|[LastModifiedTime](lastmodifiedtime.md) <br/> |アイテムが最後に修正された日時を示します。  <br/> |
|[IsAssociated](isassociated.md) <br/> |アイテムがフォルダーに関連付けられているかどうかを示します。  <br/> |
|[WebClientReadFormQueryString](webclientreadformquerystring.md) <br/> |Outlook Web App 内の項目を参照するのには Microsoft Office Outlook の Web アプリケーションのエンドポイントを結合するための URL を表します。  <br/> |
|[WebClientEditFormQueryString](webclienteditformquerystring.md) <br/> |Outlook Web App 内の項目を編集するのには Outlook Web App エンドポイントへの連結に URL を表します。  <br/> |
|[ConversationId](conversationid.md) <br/> |アイテムや会話の識別子が含まれています。  <br/> |
|[UniqueBody](uniquebody.md) <br/> |このスレッドの一意の本文を表すテキストまたは HTML フラグメントを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AdjacentMeetings](adjacentmeetings.md) <br/> |会議の時刻に隣接しているすべての予定表のアイテムについて説明します。  <br/> |
|[AppendToItemField](appendtoitemfield.md) <br/> |[UpdateItem 操作](updateitem-operation.md)中に、アイテムやフォルダーの 1 つのプロパティを追加するデータを識別します。  <br/> |
|[ConflictingMeetings](conflictingmeetings.md) <br/> |会議の時間と競合するすべての項目を識別します。  <br/> |
|[(ItemSync) を作成します。](create-itemsync.md) <br/> |ローカル クライアント ストアに作成する 1 つの項目を識別します。  <br/> |
|[ItemAttachment](itemattachment.md) <br/> |Exchange の他のアイテムに関連付けられている Exchange アイテムを表します。  <br/> |
|[Items](items.md) <br/> |項目の配列が含まれています。  <br/> |
|[SetItemField](setitemfield.md) <br/> |[UpdateItem 操作](updateitem-operation.md)内の項目の 1 つのプロパティには、更新プログラムを表します。  <br/> |
|[更新プログラム (ItemSync)](update-itemsync.md) <br/> |ローカル クライアント ストアで更新する 1 つの項目を識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空にすることができます。  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)
- [タスクを作成します。](http://msdn.microsoft.com/library/0ef97334-e8a0-4f67-a23a-dd9e2bbad49f%28Office.15%29.aspx)
- [タスクを削除します。](http://msdn.microsoft.com/library/a3d7e25f-8a35-4901-b1d9-d31f418ab340%28Office.15%29.aspx)

