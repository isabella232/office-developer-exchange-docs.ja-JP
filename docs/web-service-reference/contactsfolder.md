---
title: ContactsFolder
manager: sethgros
ms.date: 09/17/2015
ms.audience: Developer
ms.topic: reference
ms.prod: office-online-server
localization_priority: Normal
api_name:
- ContactsFolder
api_type:
- schema
ms.assetid: 6c299de8-2087-4aeb-8e66-2bc7586509a6
description: ContactsFolder 要素は、メールボックスに格納されている連絡先フォルダーを表します。
ms.openlocfilehash: 997b4f603198e6d05a011c4ef6bac7fe4dfbfe52
ms.sourcegitcommit: 88ec988f2bb67c1866d06b361615f3674a24e795
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/03/2020
ms.locfileid: "44529435"
---
# <a name="contactsfolder"></a>ContactsFolder

**ContactsFolder**要素は、メールボックスに格納されている連絡先フォルダーを表します。 
  
```xml
<ContactsFolder>
   <FolderId/>
   <ParentFolderId/>
   <FolderClass/>
   <DisplayName/>
   <TotalCount/>
   <ChildFolderCount/>
   <ExtendedProperty/>
   <ManagedFolderInformation/>
   <EffectiveRights/>
   <SharingEffectiveRights/>
   <PermissionSet/>
</ContactsFolder>
```

 **ContactsFolderType**
## <a name="attributes-and-elements"></a>属性と要素

以下のセクションで、属性、子要素、親要素について説明します。
  
### <a name="attributes"></a>属性

なし。
  
### <a name="child-elements"></a>子要素

|**Element**|**説明**|
|:-----|:-----|
|[FolderId](folderid.md) <br/> |連絡先フォルダーの識別子と変更キーが保存されています。  <br/> |
|[ParentFolderId](parentfolderid.md) <br/> |連絡先フォルダーを含む親フォルダーの識別子を表します。  <br/> |
|[FolderClass](folderclass.md) <br/> |連絡先フォルダーのフォルダークラスを表します。  <br/> |
|[DisplayName (文字列)](displayname-string.md) <br/> |連絡先フォルダーの表示名を含みます。  <br/> |
|[TotalCount](totalcount.md) <br/> |連絡先フォルダー内のアイテムの合計数を表します。  <br/> |
|[ChildFolderCount](childfoldercount.md) <br/> |連絡先フォルダー内に含まれる子フォルダーの数を表します。 このプロパティに値を設定するには、 SetExtrusionDirection メソッドを適用します。  <br/> |
|[ExtendedProperty](extendedproperty.md) <br/> |連絡先フォルダーの拡張プロパティを識別します。  <br/> |
|[ManagedFolderInformation](managedfolderinformation.md) <br/> |管理フォルダーに関する情報を格納します。  <br/> |
|[EffectiveRights](effectiverights.md) <br/> |アイテムまたはフォルダーのアクセス許可の設定に基づいたクライアントの権限が含まれています。  <br/> |
|[SharingEffectiveRights (PermissionReadAccessType)](sharingeffectiverights-permissionreadaccesstype.md) <br/> |共有されている連絡先データに対してユーザーが持っているアクセス許可を示します。  <br/> |
|[PermissionSet (PermissionSetType)](permissionset-permissionsettype.md) <br/> |フォルダーに対して構成されているすべてのアクセス許可が含まれます。  <br/> |
   
### <a name="parent-elements"></a>親要素

|**要素**|**説明**|
|:-----|:-----|
|[AppendToFolderField](appendtofolderfield.md) <br/> |[Updatefolder 操作](updatefolder-operation.md)中に folder プロパティに追加するデータを指定します。  <br/> |
|[Create (FolderSync)](create-foldersync.md) <br/> |ローカルクライアントストアに作成する1つのフォルダーを識別します。  <br/> |
|[SetFolderField](setfolderfield.md) <br/> |[Updatefolder 操作](updatefolder-operation.md)のフォルダーの1つのプロパティに対する更新を表します。  <br/> |
|[Update (FolderSync)](update-foldersync.md) <br/> |ローカルクライアントストアで更新する1つのフォルダーを識別します。  <br/> |
|[フォルダー](folders-ex15websvcsotherref.md) <br/> |Folder 操作で使用されるフォルダーの配列が含まれています。  <br/> |
   
## <a name="text-value"></a>テキスト値

なし。
  
## <a name="remarks"></a>注釈

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

