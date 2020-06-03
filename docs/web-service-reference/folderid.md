---
title: FolderId
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- FolderId
api_type:
- schema
ms.assetid: 00d14e3e-4365-4f21-8f88-eaeea73b9bf7
description: FolderId 要素には、フォルダーの識別子と変更キーが含まれています。
ms.openlocfilehash: 7aa5070fa7a2c51303c7159de04fe277f909a874
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44461388"
---
# <a name="folderid"></a>FolderId

**FolderId**要素には、フォルダーの識別子と変更キーが含まれています。 
  
```XML
<FolderId Id="" ChangeKey="" />
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |Exchange ストア内のフォルダーを識別する文字列を格納します。 この属性は必須です。  <br/> |
|ChangeKey  <br/> |Id 属性によって識別されるフォルダーのバージョンを識別する文字列を格納します。 この属性は省略可能です。 この属性を使用して、適切なバージョンのフォルダーが使用されていることを確認します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |フォルダーを使用する操作を対象とするフォルダーを示します。  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |アイテムまたはフォルダーがコピーされるイベントを表します。  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |コピー操作と移動操作の宛先フォルダーを指定します。  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | 新しいフォルダーまたはアイテムを作成するフォルダーを指定します。  <br/><br/>  この要素の XPath 式は次のとおりです。<br/>  <br/> `/CreateItem/ParentFolderId` <br/><br/>  `/CreateFolder/ParentFolderId` <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |検索フォルダーのコンテンツを特定するためにマイニングされるフォルダーのコレクションを表します。  <br/> |
|[Delete (FolderSync)](delete-foldersync.md) <br/> |ローカルクライアントストアで削除する1つのフォルダーを識別します。  <br/> |
|[Folder](folder.md) <br/> |メールボックス内のフォルダーを表します。  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |メールボックス内の予定表フォルダーを表します。  <br/> |
|[FolderChange](folderchange.md) <br/> |1つのフォルダーに対して実行される変更のコレクションを表します。  <br/> この要素の XPath 式を次に示します。`/UpdateFolder/FolderChanges/FolderChange` <br/> |
|[ContactsFolder](contactsfolder.md) <br/> |メールボックス内の連絡先フォルダーを表します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックス内の検索フォルダーを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックス内のタスクフォルダーを表します。  <br/> |
|[ToFolderId](tofolderid.md) <br/> | コピーまたは移動されたアイテムまたはフォルダーの移動先フォルダーを表します。 <br/> <br/>  この要素の XPath 式は次のとおりです。 <br/> <br/>  `/MoveFolder/ToFolderId` <br/> <br/> `/CopyFolder/ToFolderId` <br/> <br/> `/MoveItem/ToFolderId`<br/> <br/>  `/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | Exchange ストア内のアイテムを更新、送信、および作成する操作のターゲットフォルダーを指定します。  <br/><br/>  この要素の XPath 式は次のとおりです。 <br/> <br/>  `/CreateItem/SavedItemFolderId` <br/><br/>  `/UpdateItem/SavedItemFolderId` <br/><br/>  `/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |同期するアイテムを含むフォルダを表します。  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |ユーザー構成オブジェクトの名前を表します。 ユーザー構成オブジェクトの名前は、ユーザー構成オブジェクトの識別子です。  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |電子メールアイテムがコピーされるフォルダーの ID を指定します。  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |電子メールアイテムの移動先フォルダーの ID を指定します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

すべての**FolderId**要素は、 **folderidtype**型です。 **FolderId**要素は、すべての場合に必要です。ただし、Type が**basefoldertype**を拡張する要素、または**FolderId**要素が選択範囲の一部である場合を除きます。 詳細については、「スキーマ」を参照してください。 
  
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
- [フォルダーの作成 (Exchange Web サービス)](https://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

