---
title: フォルダー
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
ms.localizationpriority: medium
api_name:
- Folder
api_type:
- schema
ms.assetid: 812948d8-c7db-45ce-bb3a-77233a53a974
description: Folder 要素は、作成、取得、検索、同期、または更新するフォルダーを定義します。
ms.openlocfilehash: 5b6b8eb1d53c84bc3d0484d1c868470137db492d
ms.sourcegitcommit: 54f6cd5a704b36b76d110ee53a6d6c1c3e15f5a9
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 09/24/2021
ms.locfileid: "59530382"
---
# <a name="folder"></a>フォルダー

**Folder 要素は**、作成、取得、検索、同期、または更新するフォルダーを定義します。 
  
```xml
<Folder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <UnreadCount/>
   <PermissionSet/>
   <EffectiveRights/>
</Folder>
```

 **FolderType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |フォルダーの識別子と変更キーを格納します。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |フォルダーを含む親フォルダーの識別子を表します。  <br/> |
|[FolderClass](folderclass.md) <br/> |指定したフォルダーのフォルダー クラスを表します。  <br/> |
|[DisplayName (string)](displayname-string.md) <br/> |フォルダーの表示名が含まれる。  <br/> |
|[TotalCount](totalcount.md) <br/> |特定のフォルダー内のアイテムの総数を表します。  <br/> |
|[ChildFolderCount](childfoldercount.md) <br/> |フォルダー内に含まれる子フォルダーの数を表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーの拡張プロパティを識別します。  <br/> |
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |管理フォルダーに関する情報が含まれる。  <br/> |
|[UnreadCount](unreadcount.md) <br/> |特定のフォルダー内の未読アイテムの数を表します。  <br/> |
|[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) <br/> |フォルダーに対して構成済みのすべてのアクセス許可が含まれる。 この要素は、2007 Microsoft Exchange Server パック 1 (SP1) で導入されました。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可設定に基づくクライアントの権限が含まれる。 この要素は読み取り専用です。 この要素は、2007 SP1 Exchange導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |UpdateFolder 操作中にフォルダー プロパティに追加する [データを指定します](updatefolder-operation.md)。  <br/> |
|[Create (FolderSync)](create-foldersync.md) <br/> |ローカル クライアント ストアに作成する 1 つのフォルダーを識別します。  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |UpdateFolder 操作のフォルダー上の 1 つのプロパティへの更新 [を表します](updatefolder-operation.md)。  <br/> |
|[Update (FolderSync)](update-foldersync.md) <br/> |ローカル クライアント ストアで更新する 1 つのフォルダーを識別します。  <br/> |
|[フォルダー](folders-ex15websvcsotherref.md) <br/> |フォルダー操作で使用されるフォルダーの配列を格納します。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアント アクセス サーバーの役割がインストールされている Exchange 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |型スキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |いいえ  <br/> |
   
## <a name="see-also"></a>関連項目



[SyncFolderItems 操作](syncfolderitems-operation.md)


- [EWS XML 要素 (Exchange](ews-xml-elements-in-exchange.md)

