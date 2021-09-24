---
title: Update (FolderSync)
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Update
api_type:
- schema
ms.assetid: 47ed8edb-2a94-471b-b965-93f91456252e
description: Update 要素は、ローカル クライアント ストアで更新する 1 つのフォルダーを識別します。
ms.openlocfilehash: 460d1d9efb3f5dde34bfbb85c332ed150fe4d17a
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59517491"
---
# <a name="update-foldersync"></a>Update (FolderSync)

**Update 要素は**、ローカル クライアント ストアで更新する 1 つのフォルダーを識別します。 
  
- [SyncFolderHierarchyResponse](syncfolderhierarchyresponse.md) 
- [ResponseMessages](responsemessages.md) 
- [SyncFolderHierarchyResponseMessage](syncfolderhierarchyresponsemessage.md)  
- [Changes (Hierarchy)](changes-hierarchy.md) 
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
|[SearchFolder](searchfolder.md) <br/> |メールボックスに含まれる検索フォルダーを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックスに格納されているタスク フォルダー t を表します。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[Changes (Hierarchy)](changes-hierarchy.md) <br/> |クライアント上のフォルダーとサーバー上のフォルダーの違いの種類を表す、変更の種類のシーケンス配列Exchangeします。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている MicrosoftExchange Server 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空の場合  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [SyncFolderItems 操作](syncfolderitems-operation.md)
- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

