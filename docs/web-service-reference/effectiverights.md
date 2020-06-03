---
title: EffectiveRights
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- EffectiveRights
api_type:
- schema
ms.assetid: bf5278eb-3a1a-4d27-9d16-b8be043bb023
description: EffectiveRights 要素には、アイテムまたはフォルダーのアクセス許可の設定に基づいてクライアントの権限が含まれています。 この要素は値の取得のみ可能です。
ms.openlocfilehash: 3055eb73056750508b48ead29136b56e7ce97ee9
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44459245"
---
# <a name="effectiverights"></a>EffectiveRights

**EffectiveRights**要素には、アイテムまたはフォルダーのアクセス許可の設定に基づいてクライアントの権限が含まれています。 この要素は値の取得のみ可能です。 
  
```XML
<EffectiveRights>
   <CreateAssociated/>
   <CreateContents/>
   <CreateHierarchy/>
   <Delete/>
   <Modify/>
   <Read/>
   <ViewPrivateItems/>
</EffectiveRights>
```

 **EffectiveRightsType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[CreateAssociated](createassociated.md) <br/> |クライアントが関連するコンテンツテーブルを作成できるかどうかを示します。 このプロパティは、folder オブジェクトに対してのみ使用されます。  <br/> |
|[CreateContents](createcontents.md) <br/> |クライアントがコンテンツテーブルを作成できるかどうかを示します。 このプロパティは、folder オブジェクトに対してのみ使用されます。  <br/> |
|[CreateHierarchy](createhierarchy.md) <br/> |クライアントが階層テーブルを作成できるかどうかを示します。 このプロパティは、folder オブジェクトに対してのみ使用されます。  <br/> |
|[Delete](delete.md) <br/> |クライアントがフォルダーまたはアイテムを削除できるかどうかを示します。  <br/> |
|[Modify](modify.md) <br/> |クライアントがフォルダーまたはアイテムを変更できるかどうかを示します。  <br/> |
|[読み取り](read.md) <br/> |クライアントがフォルダーまたはアイテムを読み取ることができるかどうかを示します。  <br/> |
|[ViewPrivateItems](viewprivateitems.md) <br/> |プライベートアイテムを表示できるかどうかを示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Folder](folder.md) <br/> |メールボックス内のフォルダーを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックス内のタスクフォルダーを表します。  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |メールボックス内の連絡先フォルダーを表します。  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |メールボックス内の予定表フォルダーを表します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックス内の検索フォルダーを表します。  <br/> |
|[CalendarItem](calendaritem.md) <br/> |Exchange の予定表アイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[Item](item.md) <br/> |汎用の Exchange アイテムを表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消しを表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の応答を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メールメッセージを表します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
|[PostItem](postitem.md) <br/> |Exchange ストア内の投稿アイテムを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

**EffectiveRights**は、Getfolder、GetItem、Findfolder、FindItem、SyncFolderHierarchy、および Syncfolderhierarchy 応答でサポートされています。 **EffectiveRights**プロパティは、フォルダーとアイテムの**allproperties**図形に公開されます。 
  
この**EffectiveRights**プロパティは、 **PR_ACCESS MAPI**プロパティで提供されるものと同じ情報へのアクセスを提供します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)
- [フォルダーレベルのアクセス許可を設定する](https://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

