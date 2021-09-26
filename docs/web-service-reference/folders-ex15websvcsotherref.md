---
title: フォルダー
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Folders
api_type:
- schema
ms.assetid: 8e71cb44-1df6-444a-add7-0c1363863f65
description: Folders 要素には、フォルダー操作で使用されるフォルダーの配列が含まれます。
ms.openlocfilehash: 77442965c9d372a2895404cf1c919be38e98abb5
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59546435"
---
# <a name="folders"></a>Folders

**Folders 要素** には、フォルダー操作で使用されるフォルダーの配列が含まれます。 
  
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

**ArrayOfFoldersType** または **NonEmptyArrayOfFoldersType**

## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[Folder](folder.md) <br/> |作成、取得、検索、同期、または更新するフォルダーを識別します。  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |主に予定表アイテムを含むフォルダーを表します。  <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |メールボックス内の連絡先フォルダーを表します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックスに含まれる検索フォルダーを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックス内のタスク フォルダーを表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[CopyFolderResponseMessage](copyfolderresponsemessage.md) <br/> |単一の CopyFolder 操作要求の状態と [結果を格納](copyfolder-operation.md) します。  <br/> |
|[CreateFolder](createfolder.md) <br/> |フォルダーストアにフォルダーを作成する要求をExchangeします。  <br/> |
|[CreateFolderResponseMessage](createfolderresponsemessage.md) <br/> |単一の CreateFolder 操作要求の状態と [結果を格納](createfolder-operation.md) します。  <br/> |
|[CreateManagedFolderResponseMessage](createmanagedfolderresponsemessage.md) <br/> |1 つの CreateManagedFolder 操作要求の状態 [と結果を格納](createmanagedfolder-operation.md) します。  <br/> |
|[GetFolderResponseMessage](getfolderresponsemessage.md) <br/> |GetFolder 操作要求の状態と [結果を格納](getfolder-operation.md) します。  <br/> |
|[MoveFolderResponseMessage](movefolderresponsemessage.md) <br/> |MoveFolder 操作要求の状態と [結果を格納](movefolder-operation.md) します。  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> |新しいフォルダーが作成されるフォルダーを識別します。  <br/> |
|[RootFolder (FindFolderResponseMessage)](rootfolder-findfolderresponsemessage.md) <br/> |FindFolder 操作中に 1 つのルート フォルダーを検索した結果 [を格納します](findfolder-operation.md)。  <br/> |
|[UpdateFolderResponseMessage](updatefolderresponsemessage.md) <br/> |単一の UpdateFolder 操作要求の状態と [結果を格納](updatefolder-operation.md) します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素は [、ParentFolderId (TargetFolderIdType) 要素の必須の子要素](parentfolderid-targetfolderidtype.md) です。 
  
この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Microsoft Exchange Server 2010 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md)

