---
title: Folder
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
description: Folder 要素は、作成、取得、検索、同期、または更新するフォルダーを定義します。
ms.openlocfilehash: ecfea52d2105599372a22b78778ac0d0d066bc60
ms.sourcegitcommit: 34041125dc8c5f993b21cebfc4f8b72f0fd2cb6f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/25/2018
ms.locfileid: "19760564"
---
# <a name="folder"></a>Folder

**Folder**要素は、作成、取得、検索、同期、または更新するフォルダーを定義します。 
  
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
## <a name="attributes-and-elements"></a>属性および要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**要素**|**説明**|
|:-----|:-----|
|[フォルダー Id](folderid.md) <br/> |フォルダーの識別子と変更キーが含まれています。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |フォルダーを含む親フォルダーの識別子を表します。  <br/> |
|[FolderClass](folderclass.md) <br/> |指定されたフォルダーのフォルダー クラスを表します。  <br/> |
|[表示名 (文字列)](displayname-string.md) <br/> |フォルダーの表示名が含まれています。  <br/> |
|[TotalCount](totalcount.md) <br/> |指定したフォルダー内のアイテムの合計数を表します。  <br/> |
|[ChildFolderCount](childfoldercount.md) <br/> |フォルダー内に含まれる子フォルダーの数を表します。 このプロパティは値の取得のみ可能です。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |フォルダーの拡張プロパティを識別します。  <br/> |
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |管理フォルダーに関する情報が含まれています。  <br/> |
|[UnreadCount](unreadcount.md) <br/> |指定したフォルダー内の未読アイテムの数を表します。  <br/> |
|[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) <br/> |フォルダーに対して構成されているすべてのアクセス許可が含まれています。 この要素は、Microsoft Exchange Server 2007 Service Pack 1 (SP1) で導入されました。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可の設定に基づいて、クライアントの権限が含まれています。 この要素は、読み取り専用です。 この要素は、Exchange 2007 SP1 で導入されました。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |[UpdateFolder 操作](updatefolder-operation.md)中にフォルダーのプロパティを追加するデータを指定します。  <br/> |
|[(集合的) を作成します。](create-foldersync.md) <br/> |ローカル クライアント ストアに作成する 1 つのフォルダーを識別します。  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |[UpdateFolder 操作](updatefolder-operation.md)でフォルダーの 1 つのプロパティには、更新プログラムを表します。  <br/> |
|[更新 (集合的)](update-foldersync.md) <br/> |ローカル クライアント ストアで更新する 1 つのフォルダーを識別します。  <br/> |
|[フォルダー](folders-ex15websvcsotherref.md) <br/> |フォルダーの操作で使用されているフォルダーの配列が含まれています。  <br/> |
   
## <a name="remarks"></a>備考

この要素を記述するスキーマは、インストールされているクライアント アクセス サーバーの役割を持つ Exchange 2007 を実行しているコンピューターの EWS 仮想ディレクトリにあります。
  
## <a name="element-information"></a>要素情報

|||
|:-----|:-----|
|名前空間  <br/> |http://schemas.microsoft.com/exchange/services/2006/types  <br/> |
|スキーマ名  <br/> |タイプのスキーマ  <br/> |
|検証ファイル  <br/> |Types.xsd  <br/> |
|空に設定可能  <br/> |False  <br/> |
   
## <a name="see-also"></a>関連項目



[SyncFolderItems の操作](syncfolderitems-operation.md)


- [Exchange での EWS の XML 要素](ews-xml-elements-in-exchange.md)

