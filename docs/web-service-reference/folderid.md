---
title: フォルダー Id
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
description: フォルダー Id 要素には、フォルダーの識別子と変更キーが含まれています。
ms.openlocfilehash: 5764a164d5af183b8f313955ace5274dc6023a6a
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760567"
---
# <a name="folderid"></a>フォルダー Id

**フォルダー Id**要素には、フォルダーの識別子と変更キーが含まれています。 
  
```XML
<FolderId Id="" ChangeKey="" />
```

 **FolderIdType**
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

|**属性**|**説明**|
|:-----|:-----|
|ID  <br/> |Exchange ストア内のフォルダーを識別する文字列が含まれています。 この属性は、必要があります。  <br/> |
|ChangeKey  <br/> |Id 属性によって識別されるフォルダーのバージョンを識別する文字列が含まれています。 この属性は、省略可能です。 フォルダーの正しいバージョンを使用するかどうかを確認するには、この属性を使用します。  <br/> |
   
### <a name="child-elements"></a>子要素

なし。
  
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[ContextFolderId](contextfolderid.md) <br/> |フォルダーを使用する操作を対象としているフォルダーを示します。  <br/> |
|[CopiedEvent](copiedevent.md) <br/> |アイテムまたはフォルダーのコピー先のイベントを表します。  <br/> |
|[DestinationFolderId](destinationfolderid.md) <br/> |コピー先のフォルダーを指定し、アクションを移動します。  <br/> |
|[ParentFolderId (TargetFolderIdType)](parentfolderid-targetfolderidtype.md) <br/> | 新しいフォルダーまたはアイテムを作成するフォルダーを識別します。  <br/><br/>  この要素への XPath 式は、次のように。<br/>  <br/> `/CreateItem/ParentFolderId` <br/><br/>  `/CreateFolder/ParentFolderId` <br/> |
|[BaseFolderIds](basefolderids.md) <br/> |検索フォルダーの内容を判断するためにマイニングするフォルダーのコレクションを表します。  <br/> |
|[(集合的) を削除します。](delete-foldersync.md) <br/> |ローカル クライアント ストアで削除するのには 1 つのフォルダーを識別します。  <br/> |
|[Folder](folder.md) <br/> |メールボックス内のフォルダーを表します。  <br/> |
|[CalendarFolder](calendarfolder.md) <br/> |メールボックスの予定表フォルダーを表します。  <br/> |
|[FolderChange](folderchange.md) <br/> |1 つのフォルダーで実行される変更のコレクションを表します。  <br/> この要素への XPath 式は、次のようにします。`/UpdateFolder/FolderChanges/FolderChange` <br/> |
|[メッセージ](contactsfolder.md) <br/> |メールボックスの連絡先フォルダーを表します。  <br/> |
|[SearchFolder](searchfolder.md) <br/> |メールボックス内の検索フォルダーを表します。  <br/> |
|[TasksFolder](tasksfolder.md) <br/> |メールボックス内のタスク フォルダーを表します。  <br/> |
|[ToFolderId](tofolderid.md) <br/> | 先のフォルダーにコピーまたは移動されたアイテムまたはフォルダーを表します。 <br/> <br/>  この要素への XPath 式は、次のように。 <br/> <br/>  `/MoveFolder/ToFolderId` <br/> <br/> `/CopyFolder/ToFolderId` <br/> <br/> `/MoveItem/ToFolderId`<br/> <br/>  `/CopyItem/ToFolderId` <br/> |
|[SavedItemFolderId](saveditemfolderid.md) <br/> | 更新、送信、および Exchange ストア内の項目を作成する操作のターゲット フォルダーを識別します。  <br/><br/>  この要素への XPath 式は、次のように。 <br/> <br/>  `/CreateItem/SavedItemFolderId` <br/><br/>  `/UpdateItem/SavedItemFolderId` <br/><br/>  `/SendItem/SavedItemFolderId` <br/> |
|[SyncFolderId](syncfolderid.md) <br/> |同期する項目を含むフォルダーを表します。  <br/> |
|[UserConfigurationName](userconfigurationname.md) <br/> |ユーザーの構成オブジェクトの名前を表します。 ユーザーの構成オブジェクトの名前は、ユーザーの構成オブジェクトの識別子です。  <br/> |
|[CopyToFolder](copytofolder.md) <br/> |電子メール アイテムをコピーするフォルダーの ID を識別します。  <br/> |
|[MoveToFolder](movetofolder.md) <br/> |電子メール アイテムに移動するフォルダーの ID を識別します。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>備考

**フォルダー Id**のすべての要素は、 **FolderIdType**タイプです。 **BaseFolderType**を拡張する型を持つ要素を除くすべての場合に**フォルダー Id**の要素が必要か、**フォルダー Id**要素は、選択肢の一部です。 詳細についてはスキーマを参照してください。 
  
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
- [フォルダー (Exchange Web サービス) を作成します。](http://msdn.microsoft.com/library/3b15b0ec-8691-45ed-9a24-a91ff732d6cf%28Office.15%29.aspx)

