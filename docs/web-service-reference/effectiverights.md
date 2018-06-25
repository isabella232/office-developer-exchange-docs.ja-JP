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
description: EffectiveRights 要素には、アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。 この要素は、読み取り専用です。
ms.openlocfilehash: 610d9e214a8de648ece667799bb5e67dfcc358f7
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760204"
---
# <a name="effectiverights"></a>EffectiveRights

**EffectiveRights**要素には、アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。 この要素は、読み取り専用です。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[CreateAssociated](createassociated.md) <br/> |クライアントが、関連付けられている内容のテーブルを作成できるかどうかを示します。 Folder オブジェクトに対してこのプロパティは使用のみ。  <br/> |
|[CreateContents](createcontents.md) <br/> |クライアントに内容テーブルを作成できるかどうかを示します。 Folder オブジェクトに対してこのプロパティは使用のみ。  <br/> |
|[CreateHierarchy](createhierarchy.md) <br/> |クライアントが階層テーブルを作成できるかどうかを示します。 Folder オブジェクトに対してこのプロパティは使用のみ。  <br/> |
|[Delete](delete.md) <br/> |クライアントがフォルダーまたはアイテムを削除できるかどうかを示します。  <br/> |
|[変更](modify.md) <br/> |クライアントがフォルダーまたはアイテムを変更できるかどうかを示します。  <br/> |
|[Read](read.md) <br/> |クライアントがフォルダーまたはアイテムを読み取ることができるかどうかを示します。  <br/> |
|[ViewPrivateItems](viewprivateitems.md) <br/> |プライベートなアイテムを表示できるかどうかを示します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Folder](folder.md) <br/> |メールボックス内のフォルダーを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックス内のタスク フォルダーを表します。  <br/> |
|[メッセージ](contactsfolder.md) <br/> |メールボックスの連絡先フォルダーを表します。  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |メールボックスの予定表フォルダーを表します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックス内の検索フォルダーを表します。  <br/> |
|[カレンダー項目](calendaritem.md) <br/> |Exchange 予定表アイテムを表します。  <br/> |
|[Contact](contact.md) <br/> |Exchange の連絡先アイテムを表します。  <br/> |
|[DistributionList](distributionlist.md) <br/> |配布リストを表します。  <br/> |
|[アイテム](item.md) <br/> |一般的な Exchange アイテムを表します。  <br/> |
|[MeetingCancellation](meetingcancellation.md) <br/> |Exchange ストア内の会議の取り消し通知を表します。  <br/> |
|[MeetingMessage](meetingmessage.md) <br/> |Exchange ストア内の会議を表します。  <br/> |
|[MeetingRequest](meetingrequest.md) <br/> |Exchange ストア内の会議出席依頼を表します。  <br/> |
|[MeetingResponse](meetingresponse.md) <br/> |Exchange ストア内の会議の返信を表します。  <br/> |
|[Message](message-ex15websvcsotherref.md) <br/> |Exchange 電子メール メッセージを表します。  <br/> |
|[タスク](task.md) <br/> |Exchange ストア内のタスクを表します。  <br/> |
|[PostItem](postitem.md) <br/> |Exchange ストア内の投稿アイテムを表します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

**EffectiveRights**は、GetFolder、GetItem、FindFolder、FindItem、SyncFolderHierarchy、および SyncFolderItems の応答でサポートされています。 **EffectiveRights**プロパティは、フォルダーおよびアイテムの [ **AllProperties** ] 図形内に公開されます。 
  
この**EffectiveRights**プロパティは、 **MAPI の PR_ACCESS**プロパティで提供されている同じ情報へのアクセスを提供します。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)
- [フォルダー レベルのアクセス許可の設定](http://msdn.microsoft.com/library/c7530e86-5112-401c-b10a-9c054ae59f07%28Office.15%29.aspx)

