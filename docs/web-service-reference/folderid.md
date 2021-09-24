---
title: FolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- FolderId
api_type:
- schema
ms.assetid: 00d14e3e-4365-4f21-8f88-eaeea73b9bf7
description: FolderId 要素には、フォルダーの識別子と変更キーが含まれる。
ms.openlocfilehash: 7348fb7342bf33d487591a9daf93a9570f7552f4
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59513683"
---
# <a name="folderid"></a>FolderId

**FolderId 要素には**、フォルダーの識別子と変更キーが含まれる。 
  
```XML
<FolderId Id="" ChangeKey="" />
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |フォルダー ストア内のフォルダーを識別する文字列Exchangeします。 この属性は必須です。  <br/> |
|ChangeKey  <br/> |Id 属性によって識別されるフォルダーのバージョンを識別する文字列が含まれます。 この属性は省略可能です。 フォルダーの正しいバージョンが使用されていることを確認するには、この属性を使用します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |フォルダーを使用するアクションの対象となるフォルダーを示します。  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |アイテムまたはフォルダーがコピーされるイベントを表します。  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |コピーおよび移動アクションの移動先フォルダーを示します。  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | 新しいフォルダーまたはアイテムが作成されるフォルダーを識別します。  <br/><br/>  この要素の XPath 式を次に示します。<br/>  <br/> `/CreateItem/ParentFolderId` <br/><br/>  `/CreateFolder/ParentFolderId` <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |検索フォルダーの内容を決定するためにマイニングされるフォルダーのコレクションを表します。  <br/> |
|[Delete (FolderSync)](delete-foldersync.md) <br/> |ローカル クライアント ストアで削除する 1 つのフォルダーを識別します。  <br/> |
|[Folder](folder.md) <br/> |メールボックス内のフォルダーを表します。  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |メールボックス内の予定表フォルダーを表します。  <br/> |
|[FolderChange](folderchange.md) <br/> |1 つのフォルダーに対して実行する変更のコレクションを表します。  <br/> 次に、この要素の XPath 式を示します。  `/UpdateFolder/FolderChanges/FolderChange` <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |メールボックス内の連絡先フォルダーを表します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックス内の検索フォルダーを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックス内のタスク フォルダーを表します。  <br/> |
|[ToFolderId](tofolderid.md) <br/> | コピーまたは移動したアイテムまたはフォルダーの移動先フォルダーを表します。 <br/> <br/>  この要素の XPath 式を次に示します。 <br/> <br/>  `/MoveFolder/ToFolderId` <br/> <br/> `/CopyFolder/ToFolderId` <br/> <br/> `/MoveItem/ToFolderId`<br/> <br/>  `/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | アイテムを更新、送信、および作成する操作のターゲット フォルダーを、Exchangeします。  <br/><br/>  この要素の XPath 式を次に示します。 <br/> <br/>  `/CreateItem/SavedItemFolderId` <br/><br/>  `/UpdateItem/SavedItemFolderId` <br/><br/>  `/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |同期するアイテムを含むフォルダーを表します。  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |ユーザー構成オブジェクトの名前を表します。 ユーザー構成オブジェクト名は、ユーザー構成オブジェクトの識別子です。  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |電子メール アイテムをコピーするフォルダーの ID を識別します。  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |電子メール アイテムを移動するフォルダーの ID を識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

**すべての FolderId 要素** は **、FolderIdType 型** です。 **FolderId 要素は****、BaseFolderType** を拡張する型を持つ要素、または **FolderId** 要素が選択肢の一部である要素を除くすべての場合に必要です。 詳細については、スキーマを確認してください。 
  
この要素を記述するスキーマは、Exchange Web サービスをホストする IIS 仮想ディレクトリに置かれています。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目

- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)
- [フォルダーの作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

