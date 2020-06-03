---
title: フォルダー
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folders
api_type:
- schema
ms.assetid: 8e71cb44-1df6-444a-add7-0c1363863f65
description: Folders 要素には、フォルダー操作で使用されるフォルダーの配列が含まれています。
ms.openlocfilehash: b087be0501f04390b80458458e7e7ccc24bf27bd
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44530980"
---
# <a name="folders"></a>フォルダー

**Folders**要素には、フォルダー操作で使用されるフォルダーの配列が含まれています。 
  
```xml
<Folders>
   <Folder/>
</Folders>
```

```xml
<Folders>
   <ContactsFolder/> 
</Folders>
```

```xml
<Folders>
   <TasksFolder/>
</Folders>
```

```xml
<Folders>
   <CalendarFolder/>
</Folders>
```

```xml
<Folders>
   <SearchFolder/> 
</Folders>
```

**Arrayoffolderstype**または**Nonemptyarrayoffolderstype**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Folder](folder.md) <br/> |作成、取得、検索、同期、更新を行うフォルダーを指定します。  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |主に予定表アイテムを含むフォルダーを表します。  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |メールボックス内の連絡先フォルダーを表します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックスに含まれている検索フォルダーを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックス内のタスクフォルダーを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |1つの[Copyfolder 操作](copyfolder-operation.md)要求の状態と結果を格納します。  <br/> |
|[CreateFolder](createfolder.md) <br/> |Exchange ストア内にフォルダーを作成するための要求を定義します。  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |単一の[CreateFolder 操作](createfolder-operation.md)要求の状態と結果を格納します。  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |単一の[CreateManagedFolder 操作](createmanagedfolder-operation.md)要求の状態と結果を格納します。  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |[Getfolder 操作](getfolder-operation.md)要求の状態と結果を格納します。  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |[Movefolder 操作](movefolder-operation.md)要求の状態と結果を格納します。  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |新しいフォルダーを作成するフォルダーを指定します。  <br/> |
|[RootFolder (FindFolderResponseMessage)](rootfolder-findfolderresponsemessage.md) <br/> |[Findfolder 操作](findfolder-operation.md)中に1つのルートフォルダーを検索した結果が格納されます。  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |1つの[Updatefolder 操作](updatefolder-operation.md)要求の状態と結果を格納します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は、 [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)要素の必須の子要素です。 
  
この要素を記述するスキーマは、Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあり、クライアントアクセスサーバーの役割がインストールされています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目

- [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)

