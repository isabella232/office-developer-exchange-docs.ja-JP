---
title: Update (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Update
api_type:
- schema
ms.assetid: 47ed8edb-2a94-471b-b965-93f91456252e
description: Update 要素は、ローカルクライアントストアで更新する1つのフォルダーを識別します。
ms.openlocfilehash: 5c1b5b1fd87e4651125293eac431c56f732c6c02
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44467138"
---
# <a name="update-foldersync"></a>Update (FolderSync)

**Update**要素は、ローカルクライアントストアで更新する1つのフォルダーを識別します。 
  
- [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md) 
- [ResponseMessages](responsemessages.md) 
- [SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)  
- [変更 (階層)](changes-hierarchy.md) 
- [Update (FolderSync)](update-foldersync.md)
  
```xml
<Update>
   <Folder/>
</Update>
```

```xml
<Update>
   <CalendarFolder/>
</Update>
```

```xml
<Update>
   <ContactsFolder/>
</Update>
```

```xml
<Update>
   <TasksFolder/>
</Update>
```

```xml
<Update>
   <SearchFolder/>
</Update>
```

**SyncFolderHierarchyCreateOrUpdateType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Folder](folder.md) <br/> |作成、取得、検索、同期、または更新するフォルダーを定義します。  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |主に予定表アイテムを含むフォルダーを表します。  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |メールボックス内の連絡先フォルダーを表します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックスに含まれている検索フォルダーを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックスに含まれているタスクフォルダー t を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[変更 (階層)](changes-hierarchy.md) <br/> |クライアント上のフォルダーと Exchange サーバー上のフォルダーとの相違点の種類を表す、変更の種類のシーケンス配列を格納します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Microsoft Exchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空にすることができます。  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [SyncFolderItems 操作](syncfolderitems-operation.md)
- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

