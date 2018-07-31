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
description: フォルダーの要素には、フォルダーの操作で使用されているフォルダーの配列が含まれています。
ms.openlocfilehash: 34372f2480825c7a9977eeae8e730c201307f36b
ms.sourcegitcommit: 9061fcf40c218ebe88911783f357b7df278846db
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/28/2018
ms.locfileid: "21353589"
---
# <a name="folders"></a>フォルダー

**フォルダー**の要素には、フォルダーの操作で使用されているフォルダーの配列が含まれています。 
  
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

**ArrayOfFoldersType**または**NonEmptyArrayOfFoldersType**

## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[Folder](folder.md) <br/> |作成、取得、検索、同期、または更新するフォルダーを識別します。  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |主に予定表のアイテムを含むフォルダーを表します。  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |メールボックスの連絡先フォルダーを表します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックスに含まれている検索フォルダーを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックス内のタスク フォルダーを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[CopyFolder 操作](copyfolder-operation.md)を要求します。  <br/> |
|[CreateFolder](createfolder.md) <br/> |Exchange ストア内のフォルダーを作成する要求を定義します。  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[CreateFolder 操作](createfolder-operation.md)を要求します。  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[CreateManagedFolder 操作](createmanagedfolder-operation.md)を要求します。  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |[GetFolder 操作](getfolder-operation.md)要求の結果ステータスを格納します。  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |[MoveFolder 操作](movefolder-operation.md)要求の結果ステータスを格納します。  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |新しいフォルダーの作成先フォルダーを識別します。  <br/> |
|[RootFolder (FindFolderResponseMessage)](rootfolder-findfolderresponsemessage.md) <br/> |[FindFolder 操作](findfolder-operation.md)中に単一のルート フォルダーの検索結果が含まれています。  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |状態および 1 つの結果が含まれています[UpdateFolder 操作](updatefolder-operation.md)を要求します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は、 [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)の要素の必須の子要素です。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目

- [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)

