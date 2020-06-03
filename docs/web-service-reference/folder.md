---
title: フォルダー
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- Folder
api_type:
- schema
ms.assetid: 812948d8-c7db-45ce-bb3a-77233a53a974
description: Folder 要素は、作成、取得、検索、同期、更新を行うフォルダーを定義します。
ms.openlocfilehash: 156813b3f7ecc6a2e1437f473ae1daa76b138e6e
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44457250"
---
# <a name="folder"></a>フォルダー

**Folder**要素は、作成、取得、検索、同期、更新を行うフォルダーを定義します。 
  
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
|[FolderId](folderid.md) <br/> |フォルダーの識別子と変更キーが含まれています。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |フォルダーを含む親フォルダーの識別子を表します。  <br/> |
|[FolderClass](folderclass.md) <br/> |指定したフォルダーのフォルダークラスを表します。  <br/> |
|[DisplayName (文字列)](displayname-string.md) <br/> |フォルダーの表示名を含みます。  <br/> |
|[TotalCount](totalcount.md) <br/> |指定したフォルダー内のアイテムの合計数を表します。  <br/> |
|[ChildFolderCount](childfoldercount.md) <br/> |フォルダー内に含まれる子フォルダーの数を表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーの拡張プロパティを識別します。  <br/> |
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |管理フォルダーに関する情報を格納します。  <br/> |
|[UnreadCount](unreadcount.md) <br/> |指定したフォルダー内の未読アイテムの数を表します。  <br/> |
|[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) <br/> |フォルダーに対して構成されているすべてのアクセス許可が含まれます。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。 この要素は値の取得のみ可能です。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |[Updatefolder 操作](updatefolder-operation.md)中に folder プロパティに追加するデータを指定します。  <br/> |
|[Create (FolderSync)](create-foldersync.md) <br/> |ローカルクライアントストアに作成する1つのフォルダーを識別します。  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |[Updatefolder 操作](updatefolder-operation.md)のフォルダーの1つのプロパティに対する更新を表します。  <br/> |
|[Update (FolderSync)](update-foldersync.md) <br/> |ローカルクライアントストアで更新する1つのフォルダーを識別します。  <br/> |
|[フォルダー](folders-ex15websvcsotherref.md) <br/> |Folder 操作で使用されるフォルダーの配列が含まれています。  <br/> |
   
## <a name="remarks"></a>注釈

この要素を記述するスキーマは、クライアントアクセスサーバーの役割がインストールされている Exchange 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素の情報

|||
|:-----|:-----|
|Namespace  <br/> |https://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |Types スキーマ  <br/> |
|検証ファイル  <br/> |型 .xsd  <br/> |
|空に設定可能  <br/> |正しくない  <br/> |
   
## <a name="see-also"></a>関連項目



[SyncFolderItems 操作](syncfolderitems-operation.md)


- [Exchange の EWS XML 要素](ews-xml-elements-in-exchange.md)

